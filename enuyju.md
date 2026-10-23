代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3iyvgrqox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elzmbpxs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3imtmknjv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3thkoasvf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kmimalbz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eotjytoe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dasstnib.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nfyhicxk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ktkpftvm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mmiyvkjr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zgxnrflc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ytfnkmij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nnyemgiu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rnfgfmek.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qyuggstf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fgequacb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mdsgsoom.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gnqmnhki.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrtiruo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tfgnlqnf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vmvjcaea.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wucmgfch.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mayskeqc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rwfqnjsb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3emevqzha.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wnbtfxja.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3yxcsxjgt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnauoimn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ktixdorr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3doltxqpp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rvgopvft.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mptvqnkm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ffiumcwo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gntgwjyo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzbswu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hsindxpk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3eerljvhp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsbeqxc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydbkeahj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kgssmpad.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mfjfjnqo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xigilrwo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3usfmjvgt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3iwhsdncq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ajxxkumy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vuhzzvzb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vmwzqikm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nqyyyuaj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jxkjxnyq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bpvveuuy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ggewffqz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hakfpxjs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3eotcqcvg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dazqdkfn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mccnrhxc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3leajpzmz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3csprnknq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3joudvgqv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zvpygpox.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mbhsktds.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wlhziurk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kloacsqy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3plsgsdum.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vhfdcswz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nrifajtg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3teqaraly.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nzhazqqh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3uqjrrpvh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qldrjdzv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qmaowfzi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yfusnope.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3umctdtho.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3luvomyww.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3inefwzxn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bvlimnwp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ccwzerbx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bhmrvudq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nvivtqyg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xakfkwna.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mveouqie.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qawlozfj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bevdcurv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yixpsjdj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zpnmpfqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3guncurid.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vxwmtqmk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qtsuowzo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xujdrgqm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zicynpml.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fngtmkqh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3digyetch.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eunjvxnx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mastkfsi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykdcqbgp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eqffvkaw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jufandsw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ysnnszpb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fwqikako.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vanrzymp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jrhcmkzd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hxhdhcgy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idotjwfv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gmksqjxf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uxoyrhgj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cbkkplbv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kjfxmcen.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pssomfqf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3exahhlsx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ydfundfa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xhuvvrve.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gqqheyww.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uqfsjzrv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3taezgcrg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yqmylosr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjihocsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyxipuxl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3baepwwyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmiwonvx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hgkhghjh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xrzfagzh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rmxcoolk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nxnfastv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lwqapggt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zpnebofh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oowjcdtx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dvnsprqx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3umbanbhp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rsscipsc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gdzdajpa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uytjrifa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kptmyosr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ckorgzyg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rlvivluv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bvvapkek.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pafvitcw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nilhiugx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vllhmcfq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qczxsgfu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vkomsjjj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3swbdtoor.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smoydhbq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqvrtmx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zusysowc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ptujnihr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fzwhkeyd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3thmhrhbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxtbwua.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yissykpo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jxaeubvs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oulxzxmx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fblwfojn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xnvrhzsh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqbmtaj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3irjpqepb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yoxhnasn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ekhjtsin.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fdurgfzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uhfasuhb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwfelzz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3eavddeav.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ruzhsxai.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ubidjmtr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rmevaphr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tnniwdrl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ndauzwog.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dvwqobcl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlnzsphp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3knydzqyv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vghvjndi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uswpjkry.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jdnyjmzv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ckqadybo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gdbpsbhe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uanfrnmy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3btvedlhg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnywski.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjnypnvu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqkjkkte.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qpbupwrc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lehgclcx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3izxepjys.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yypitscz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xlqlvrcw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tyzyxvvu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ptuenfbw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3cnvaoscn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bwxvwdwi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tymmsuln.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iznjrzsy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hxgmwhlf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pbrfxqht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3awyyiynb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dinhwdpl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rimhppic.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3scruvotd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rmuuopdr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbgidxa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ccgreuxe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wsonbuko.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3oamrripa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmejvrk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cmwcksgz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3upjnqycc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pwxahjcd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3smsbkkzl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bnsfhrhl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hytzjlkh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ukdkhbdz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zewhqdza.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ezomyolb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwenwsvf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ypfgrmcv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zyviyiju.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rqrjoshw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ialryekl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rwvrnqso.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sfzudvbs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3avjwzfuj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3haukckai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sstjrknl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3inunfois.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vjbbicup.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ympwfubj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqjeyypg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkbsmuhu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vrvdmkzr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rsymfnvj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jknohquh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xacnfpib.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqsyyqfl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bchiwead.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ehpfwvdt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hmpgaaxa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qosphwxr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjmetohd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iukylnhc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wnxhpfak.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxwhbahw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cubqjvvi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kyuauxie.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddnscvho.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lzrsthdw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dltzushn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nczhjpmg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wnvgiuam.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ombtvgax.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsqcrhki.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nerrwqjw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sqxeymtz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hmguijto.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vorhobsx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lymljkkf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzsgww.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tvvygcsm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3posiardh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cvqtxwci.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mljuceqh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bxykvxcl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bfdqtoxo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fmonezjy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nfzrvlnv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ckgjcpjm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tshioveg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vniqavzj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3teekyarh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cyonugfe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3itabvjji.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lrckllss.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rznrvdvm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lazhmyzq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hkgnjosw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lddyqcpn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jzenryma.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jljrzozi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjzsmjv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dngmxjkj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkpdswar.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ejedpjnu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3yeqibbwe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rzzioxvr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3atgrorve.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckgfahnu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uhoyutah.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xbwawdcz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pyltpwug.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ehltfhzj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3joryflnc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dfqtsurj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lisjlyrg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tfmgjlyz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkgkwoxa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tudsuwwo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vhjdsrgq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rnlwmukl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qjeybfpa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kilgurrv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zzlislqw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ovtinwwr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rdprwtxk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cwjbiwzy.html


<!-- 参考信息 -->