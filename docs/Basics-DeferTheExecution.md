# defer程序执行

我们有事需要执行一些耗时特别久的工作，特别是调用一些第三方接口的时候。比如发送email，在这一课里，我们看一下如何高效地做这些工作。

我们时常需要在Meteor应用里面发送email，我们一般如下操作，这个操作会使得程序更慢，可以做一些改进

	Meteor.methods({
  		"submitVote": function () {
    			// some other activities
    			Email.send({
     				to: "hello@meteorhacks.com",
      				subject: "Thanks for your vote!"
    			});
  		}
	});


## Setting Up

首先我们clone如下程序，并加入kadira支持

	git clone https://github.com/bulletproof-meteor/bullet-defer.git


