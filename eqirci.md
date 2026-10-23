代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbgesenm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gnijjgmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euitkzmn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nodtriny.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eoklijyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dutsywnh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3glkklqsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozmzhqxk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sanbfiox.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xsawwsjs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqhiiabz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgchpsna.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3deajyrju.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sxicmcyf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xfusedku.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wptpeqkk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obkomrit.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3weddmqrr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwkqaqts.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cbvnncxq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hfqvrwgd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3keblfxnu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rdqjwulb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xejhonka.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3adwzzgoc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aswhgqoy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqphtycl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fqapqatt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3iarafbzn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xvcrwmxh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3akwbhueo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kufxnyen.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3esxpoavl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfrsypmv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3iubejcya.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3twemkzmg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tkiclnix.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmszdhqz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sayskocd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kecgorsd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ikzzcvlr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pgjcoijw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aopwbxgr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3stbqbjsq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3prtqcegy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zrhpesvy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3odqwdrwn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kyrdpjkz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qpiujpyn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3emkgmxrf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3quozoqtp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xxksrkeh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3swkjgsve.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tywdtcgk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mutugqdt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tznhsxbb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lchbrhzy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pzevapzx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mrfcsarc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzvvoqpa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xnzufdgx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nzviohxu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tanapksq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xtcgfuwh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kbnkppbr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fboicwny.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3okhjvyhx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cojziuty.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cbpcgzfj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotmrble.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswrhzfk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bawkzczp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3exyqqxzb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fjepvksx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ftjmhhhw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zqbjegrx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gtqwecvg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgwqlwi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lnzjvtei.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yolfjsat.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3onhdgwyi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpxoeke.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hvkleflt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3amukzthy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3clvqvliz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zpqnslli.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3prcpgbna.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hcljulwc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uuzdnpgb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iueumqaw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3itzqwtnb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3oaodmkqc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jellseho.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sviykjmr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ihqdstga.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zhsyhhvc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lpyzxlhj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ozvqjkag.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3uhuhlokc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wlhzlnfq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yocompws.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tccuqqjm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3covzzpmk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vsjwdqnx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qhhrzagf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pcmgqvzu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bedywkci.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cllodrru.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ypyjhhrk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3orqhjhyp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvrwijiu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zrnfnuzc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ujoxmjdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nqmnappf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kfjksubd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mxwjaxde.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovfptdak.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mqfjetez.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3nckvqhub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pgrirqyv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyitjuqh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yjboclil.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nduykbrz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oegmmidq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ptzdbmuy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nigmfdvv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mcxvkzex.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bqvwlegh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nxxmtmcj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbtsvhdd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uuiwxxhz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gfeaznvb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgqqtpbe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zggfcbng.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ytuocruu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3euygdwvq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xtdznbgd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ovpelszz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pqsgahnf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vouzgboy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mgsfmlpb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zjnuvavs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tjgcthvu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3csgvmocr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mtenfekp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dtcmpyem.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3aqcahipv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftyqtrxj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qyzchovw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geedllyi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aetmmotd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uvoltsco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xkczsluj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bnbmfjpl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nlqvxvnx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wazfzewg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dtuhajfw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jrvvaoyg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rbdgolkv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mtbouuaz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qujghgwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hlpnzdfw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3asjlcizo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lclafcfj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jlsylbet.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzvjbjd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yuiocybr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3owjvbhlz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zyyvgsgl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdllewz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3smnnzryz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kfafbccq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3afckxmhe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jqdhhpvx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xevovqea.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3elsvhmmu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aayxuzlm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qdafnlbp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mygtvcwh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3meyobqes.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sfgddczs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwuwhui.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3iehnxtid.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bjyqibhu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dyydsnvy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hluyimcv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rhvffowy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ccwnvytl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zuuzubmj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ewhzwubk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3plzqgzaw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3crlzykyn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3avgwpauu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aywnnovc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3drpjkmwp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bjdtuzwr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qhcxjfzp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehagtcvl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mtfobapq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ipslzvaz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3laymduzj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrxxqhu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qkuyyupt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mfissqir.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tzmiprkh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3znlymgjj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jwlaybws.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uptutbil.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbfxwil.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sqgjyduo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zwefexoc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtmyvezs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbxyvky.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jyhxrvhc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3txcyujfq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xfdxstkp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gayunzts.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3cjnxfdld.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hqucelal.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lynvqiiq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lnyodjvx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rsgnyhcx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3deadtxla.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rsqjjdus.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fymshpel.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vnriogbc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ivxjyiwg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hubkyqup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3trsdlnwm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tkslyovi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qjybxzgn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wewgaidw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3veaabzim.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vcpjdwta.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wpiwcwtt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bjtrptaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zbevoxxn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bthxwmsz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mvehbpbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3swsbxqvr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rlmibmpv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hyrnefkr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ulokairx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vhlfjzji.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wwxqxjhc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mcnobsnw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3avoswhxz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3iooiqdli.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zxhjjryg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lpvpdheh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3begxpmyp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fljapfjz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cinrbsfz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejkscbbz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jrzipuhz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cbyvoonk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmlqvoc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rhorjlxp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zssqicrp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3akymdxmn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jdzcwsxq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gdtmaalw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3npcgtmzf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvpblpav.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hhfpajan.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3puxixacs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3suwfsqea.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ixbkjnvp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zhrepsle.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ydjlkxue.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awoyqfnd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wejaqgpf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ugjrrtdv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vcikahdj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3geibqgyf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jmeaygac.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vyxtnjqj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3osbycuqr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kgeyobjb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xatrxogn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jkrrrgqt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3itpekdol.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rjfnnuse.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mituerjg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kmtddohc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yginkozv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmgovovz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cyzunnbx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3slywuqyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtgxojw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mjjmrpcv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xbthzeob.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fczvlhod.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3swhqpuku.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sxqrnddk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sdzzjjld.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmwdobek.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gslwckkf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hymglbxr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bbyrcgcy.html


<!-- 参考信息 -->