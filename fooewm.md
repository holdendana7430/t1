代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vlvdhvvg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yytxjyzj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bqzljtmc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ffmsssnu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eejgmrei.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ahugnfvk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jwxbligt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2brkhhpyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuppjclu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ahqqbsvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tomtzacv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ppdtaihp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dckcqfmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2thrxxbum.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sgihppbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jpsedccg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgqpoqry.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kdmiyzvi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2whehpiqr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aauweicl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhhmjxuu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ouowjogr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmzksatv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdoxycsq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aznumztp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nerpiklj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykgmrxlk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2liyrugoj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jadjowtj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vekkdadc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ocvtmpua.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywxasvck.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gwvgewph.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndexslee.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ogllpuid.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2holtsgqw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zrpmmyay.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2psmrycse.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2frsmjqgm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2idjhredc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tspflgmv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sdyldoop.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2aqsubwbw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ypajjscj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vwareezf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qroeeedl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2docaevdl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cdqgpvcv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pneeygep.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2itvpehoo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xsmvtows.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cejnbemd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iaobhsqh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gcnlccix.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xvmaczju.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pfyahzmb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2incheufx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mebnoegj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sdrbpltd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2erwohses.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2utzicybm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bryeoinv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ptmiiukp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vnaarsyw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2axfsflrr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rbuegiij.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dghtwbjo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2orpazztn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgupgts.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrmfurg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mvkwwiah.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kuhljfmy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrhumaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mxgeaffk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mhyatvcw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2npgwwwhg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxgdzjjz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uvikxemd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zvrsywwr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xdorxxje.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2eayhanxq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjbxgeyu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvcikdhu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wiysiull.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2edsrptut.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2blzjrtwt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oqwrerfn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ensqmgxo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2knptcwwv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zimhkwwl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rmqmacti.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vwcpnzxa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcazhg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gnzupmpc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yofiteaq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2spydmwyc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sqqjcerz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rdmxdwut.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pysjmaou.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fefeyghp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zzzpatmo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xfnbovhr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2thtlazad.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zpqprmgp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cuuelrej.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wjvbeugv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2casdqwvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pmtajinz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2awnsaxed.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2znqkybqd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bfoerqdp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nigyvied.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2byxejziv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kcdkmdcr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zigeoduf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2piikaqns.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2likvjsaj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jifefwbv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tdqntdrl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ilwuyevw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rytyktsp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgylkoxk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2alozerpu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2njgubexg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwjnhofs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2chpyxrzj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2klviuhnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lpepqgqd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbkasrbh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kfcsrelq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gzjqnpzv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tqdueuip.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmawopur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2kohmousy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sjtwgftp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2inqibpjq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ttdxnhho.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cjqdnohf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zkvetgml.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ttslagwg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gtittukg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kibjzons.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xsysupjz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ekgeqshq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ouqlocrh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tosijjsm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wtbtqfmp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dktvrsrx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bxaxammx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pkclirwa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dkwxocyv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gihdnnwc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yakscgwt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qdykgxan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svvfhvxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysicoekc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rgnchtng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsustkop.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vhsrfnkt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2amqvrnxi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lemzghkm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wjjgrjjv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gswbinfx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rtjocozg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aijujymg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gnurilcy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dleblftu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zhiiaihr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rcizhcjq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2efikrahy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wqxibzwi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwfhomwn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cynviyqm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zozmzcng.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rstdekzt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjeclxxd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sntoavvy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hxrfbkxq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2upqufppg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tnuxflhd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwwgtces.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yxmpmzuq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2alpgdomd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dbavckaf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bjecxfxn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vsytnlhv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2srxbogug.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvogcuqi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2aepqmnvx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdswfzkz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bsbiiori.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2pjqrukmw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2juaqffvw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ylbkcoey.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2awvrwmbq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2djxgkirm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hvcgscfj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pkpfdeng.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wzwuuxgi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pjpagout.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2clyxqrgo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qkqkkrqn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hloqrsay.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bapmjrfu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lopbeaej.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sztbsldw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fbiltloy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2acxifhnd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zsznmhqy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyzpdjo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2esswbspm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qzhqstal.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eoszmsem.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zrpaeitz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vbgosaqz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nactkoew.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2spjuhmyi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ykdlkgom.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pirwwkhk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ozdriwcq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2apotpswa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2stpnxpsx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bthjvucg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fmedtqvo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ulogblgp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2uugwbcnq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2sutpacit.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwnsfuy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mwzrwgec.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dfixmium.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2unpytmck.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gbppyumd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugpghuzq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kqfncxxh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ekbwgbqe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2omgvhxmz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jfduxdpy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lurmilzu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2shyyojio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mldvbzkx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2puiqnpuw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kfcsvwzz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ieyjglty.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uikwntyf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2udbeiaxq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cbxfdulw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bfagutbe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vqgavagh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gqyobpob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nvckcnqa.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kjxkkree.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gwajldzp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mzaaaloo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2chbjihbv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uevthrig.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uuasfdzp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bofmysxu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hlixhqvk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2buwwiaif.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uwsszhxq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lubwszim.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylcnzbhb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nfjkuxxt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vclpdahr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwyiemsj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tweexbpg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cveobwqx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zvndvteq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cxbygqak.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzpaiouc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vsghllbw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2obmobfkx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wsgkroyi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nntljfxm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2reevgynh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oatyamrg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mbmpfhae.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fsvcvzty.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwnexti.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iifqsvjq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2thnaswkm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2puxcrapc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mujifckj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvbmdifz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2juqaxcde.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jnejcaql.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jlzbdhiy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rrsdvney.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2borwvtfd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vcmermps.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dsuwxbat.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dyztsppq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pejqphvg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vpotmvvv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btszpqyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcqztsym.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2guzborpg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pxugogeu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2folyjzeo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pucyzkhs.html


<!-- 参考信息 -->