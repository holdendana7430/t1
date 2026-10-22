代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ufuvagts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnlsyszo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uvmptats.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofqeuhzj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oosnbycj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rgahfkik.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjysjhie.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bonaixqr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hgxuqxqh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wsfygllj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdlhqtk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sgrretsn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kupfdngh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bomzrkfe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jsgeenhu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ctzebqeg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ahjorwve.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wdyutkhw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lkodtlvv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uglacvrm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmksadyn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2raikqdik.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zikgnyjd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2akucfced.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vjwewksf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bvssysht.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ddxgauai.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ldijrbcn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gttlocts.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hnunnxdm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tkdukkyv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dttwxkgr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hglwgyoc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvytogf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hpmnednl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wpbxgupk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2paxwqxam.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fvaaumzi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oevugxil.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2etsgrgvt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2smsmzinh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2osfiudbo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hbegcvzz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qfdhtsmc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2viyyggmv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2shorrvta.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ylrvgtlh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2faxtfyuh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fgbrbnzw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2boljxhjm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bhwbyvhk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lumbsxvi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2knkqzzft.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2trauyndd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ewbtebpv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ryybhilh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vkcvpakh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bgehqukj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pdjpawit.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jfgsakwm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2grxlxlmt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nbmrgzbz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2olvvtfbx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wsracryp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtmgktbw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2chyyybfr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajfzpmou.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2giofvmdr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cwibgnbw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpxwfbmy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufedcubu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nfeqsagv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2axddpkyl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gmakrafp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2szqqrppn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2juinishp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uggvddrp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dzefbzyl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2afmvqtum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gusoizvb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2forpriqd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qmtzcsrz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zwkehhkp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pwaoudso.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2byawtrxe.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vcfrkwcq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ujtpojvo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cydmazou.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cpbuvonb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ryzkvrzt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gwchvtfm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2uuoylhjc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2svvizaom.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2icpruwch.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cutagpzv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nesltgqg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ezjjsebe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2okwynyxb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2guonjyss.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zcspznqe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fczmuzcv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dlnzqrxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ghlbnrzq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2idjiqlkl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dqwupsji.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wnwnvgcr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xjnmsste.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pwqzgjwy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gzgkhhvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qdzebobd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ctylyizj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2afjoeeiu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tvrjljeh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qrfshdff.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fdgblrdi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fzsfvmrl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mdooiazl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pcvyiafc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2leirlyzw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xmwwksur.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2esqstiiz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmjxwfi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cziwvhxr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mxcjxdea.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dmcuhyue.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhyaftav.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lxtkaphi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ttgsubyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvdynzwq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zwslsdkb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vyfbhsfk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dzzzknbr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ycfixcfr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uhnnvdtv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nulxersr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2unxeldoe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sgoqigro.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ndkjvguc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gvmapiqz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znziphlp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tjkemrfw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qpclajlb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zkzltvfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyebzyqi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zehumytn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nccffrpq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iphbgfqa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2oykeapxi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2atljlqhw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oedflhzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ioicsslv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2daqwgbju.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rjcadfzh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ouxuegvq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wfhgcvnw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qoizfzvd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zunsocvg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2npmxaich.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lthcqsre.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2byrvjxru.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pqffgpiq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ebbfrlmq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2plilvaeo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2avzbkkpi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jgrlkuxe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kefxstrl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bnzlzzae.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ndrbatcl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cpmesvmn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkgzgqtc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ythcasnm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2phsczasx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2krqkagco.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dyrbtjiw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jvazyedp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpkfaaph.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kcekvlsd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2whzoytda.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hjvzpwxz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rjqjswhu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnaxvzas.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zornucpy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mvvjkcxn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cqbwfbwe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rptwuwcp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dpeocgta.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zewqwzqd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ybrpmsla.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dnxbgevo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bhgwmels.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jsbwksmv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2areoyakj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmnwjryf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mivpwntd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2auhamakn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qqmjemsd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gafuezfc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ouuzkmxw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xcmbpjie.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ffyfmvhl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2piceylig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zyyqyvcb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgemlnj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tucaqpvb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcahusav.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xlvxtfhu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2odkvhzhr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qmdrjlfo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rmofocui.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uokcyexv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zgfwmlxo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2oiqaaelr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2euypgeti.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vtfurrub.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2icmadamq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2scnbccto.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2udeiwagr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bwlmfvdq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bigoarzv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iinzrgog.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2prjxiquw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cmahkrqt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ijkivnie.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2phyktarc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfwdmhwn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bhacnqfw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uanyqpgy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jskqremy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fyuykwgk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jfohagdv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtrfwim.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rdibcgpx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vsdnmgzq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ekxqdwrb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2maoclazy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2owarepkn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lbgvimtp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pekyrsyj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jfqpxdvl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lkirpuox.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mrlreuys.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nvyualxu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxihhpc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uxmocrch.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2dhndpqgc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qxfgxdjc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tgevlioo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dvbsxnhl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wshvirpe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xmobannv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2voebnxgr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdtrzmtc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fhiewfar.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zcpfmntt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fsvedskd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vtahbylu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kptbcvon.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmdhrwj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qbhbnpdw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vsajzlrt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ykqpyxrh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ccdzkxau.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fbyceiwc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2amrmlriy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2heqoktno.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwtqjlvb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hlayyybt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qilwmmvy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2egxrbclp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ukixmojv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vuyppdso.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymngiojw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2voulzifi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vbbigpgl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vifqwnng.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2domhlwuz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zzylcesr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kmarwvfq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xmmnkmgt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kgzviqrw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhaugxkl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ejhvatff.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqoaspyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmuyvpnn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fajjgrjz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hwgazmed.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mkmnpsgy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mwrhiyni.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qijcyytr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gwxlmfxh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dlbgbjwq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzhmmsnh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kzwcisyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkvvdwv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ebtbsngc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2kfwbwhzb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lgmydznp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2plsshsbe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zniodomy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2disiihga.html


<!-- 参考信息 -->