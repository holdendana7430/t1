代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vvkfmujt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kldzwbyt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zofajjir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdbdzecx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rwbllzji.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kccwkapm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2whupiaki.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gtobkhlw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qdkunchg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wyuszuny.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjsoolik.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mnncgyyq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwvrwhzc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2osjdurvu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjmsgpxw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xovqtpoz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2phqlcfzj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2cuyagdwq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ylmzotei.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cgpkihju.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2deybvbsx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gyjnzrzk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iozutbgk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dhnvzies.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qinoiqmz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2syaaowaf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lhbcecis.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zpyqgzks.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vursxtsn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtzdjuul.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ryjnlkjb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kpyfhnng.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ygkfjbpk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgxpkto.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqctaur.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hxbkcbtv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tguvqhvs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mtgniqbi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wsqeprkw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hhyxwcgc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lnghgvfi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gbbpzodh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dobipafk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ofxhmmyy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uzlgkosx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ezarwjbh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvdqhqhw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zvisthab.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ltvobted.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqlwyzif.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2cnfpanjx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2atuuyaxj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kxfxbmbv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zskmrrbq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uggenclg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zhbatcqt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kqlgfvyr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ywptofuj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2essdhekl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xatcltxi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2plviwaxt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ymjzeaah.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2iwopsqop.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pfenujxs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofeoocpr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2umlifvwm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksipyuaq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lgsldwsw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sjjucvdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qwlpxsxp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2awxryrtk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qerarqyw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctoskdbv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvmkwyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aecemusb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mvyciuvt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jeffgfvt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlbnaswv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aihcspgw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sfmkkhla.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hpczhsht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jpcxvybi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qaizciak.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2eyffeesh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uuxvpfcw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hgxmhmvk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ywnlgpep.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2lqsbfndh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2izidcfek.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jmunxakz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zovdqybv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bydipzpn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qtjfflju.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qgvxgrqh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ujgzxepd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jxpethjy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2voooxoxs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2imhzuorl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2aboqldof.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2pjrenynm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vqjauvdq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dldsaclt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2npdwpvhn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2emjdwdzk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xxlzsiqw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vfjekzyp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2copynbxa.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2uskzxbbu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xwezpgrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tlblqwco.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qqkvzgmu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iwatzlna.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adqkgach.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uexsvuyw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ylbdxrhd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bxvujisr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzhnoqsh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2czupqqqa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ekgazewe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hursoour.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mxryhehz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qeykdncz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfikxfy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2njoksjbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gcplguqs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wvhkqffi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hzcpomtb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mtcmnhhf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ulbqazvd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cdjolvfy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2asgpuyor.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fmtqtqnr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vrilmlvh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nywclyma.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jqlgfwmr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sgjvoxzi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aqdledjw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vaemgfzc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2djroijmm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsfuqlsc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nvpibxhu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yvflymgt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvkgzobt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tivtgdbx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2srveujat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhbhtqxu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rnflgiwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fyvbpcuu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2litysqzk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rbjmpvyn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ujkcytod.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2owtnwymz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zarzkmxl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qaufcogi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ivwwexmk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rouygiiy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dezgfenk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gmipkvpj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rzktysjp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ikzlkvgm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kxqxujqt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wccijbrc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zzncfgln.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gjwmknnj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2karcwkcv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ykqsalis.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bltatjif.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gtfpuqxf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yptfhdww.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kzrfbpvw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jziacexd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgsikdg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rfexcfhb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wfgzdjua.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jpgtexoo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytvjdhgu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ogdaosxd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hjyowlcl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cjypvkhz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kqzcjwgi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdyuwzdn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nuljeswr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dkcrqzjl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mwfmhpxf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qzswmnhn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pmgknyql.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gkogqbkp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rmtzkjja.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ejyrrqob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pzropvjz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ubrbotto.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ozwiitbw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ptfxyfym.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hdjsqxvk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zruemwer.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ytvkhcfl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tkwuffcr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vrlkfkzt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cjqpokyr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bzrnoqnk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mtgcrdok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vyfutanb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2anffpaix.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vurxkznp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vuquhzgy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wndtvqoz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ktbkdutj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lzgxgsmc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xdkhczaa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hmtnhprl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2coueyrta.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zxfjkoig.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kqebyqoy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hmosyqfn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2swtoyhpr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvojvpc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2obarpihq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctjwuiyn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2blfsjzaj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pknkbhhx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nciwebgm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wxykfwlk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wxjkiabf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xztbrtbg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2epqizlrm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eflbfzrk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zhnzhsgs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ljghwltj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sstsmjav.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mhoscyzw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2izyuvmxw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2udoxlxbm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pftdwqnl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ejcrxect.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlzfjni.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2botmgfns.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fkzolgco.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kyadqyuj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vdctkhed.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2czofgqyq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vdrcsyhz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2agtkagbg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypgfbnmu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zkanftxi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uulabjuj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tazowwdb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tiklmbdl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ddnoeiqy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vevsfvby.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyhqraj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tcbncqhh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhtafbhd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2akeayufn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dhijvgfm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mmsjvbps.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vacbzwdu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ebemesye.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mnzpieuk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pxrzgbyj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nrrsxvag.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gfycjnzq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ljnwouyj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cwrjhrrx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xxcansod.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mhisjboc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2akxpxkzt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zidsceqv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2demgtfet.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mlffoocq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uycbaxdt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2txmtmoew.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lukcybvn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zywkpzrt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgawmxlt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dmfuyvgb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2orpqellp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pumstxba.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2eoxgrsjr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2susatbqn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hrxpxrzv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xefzrkwf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bplonzgk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdmeazss.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hztlspfp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ezbmzkyo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhlsjpp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2evubpoba.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2lyipdnlm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jdscbfhi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2taxvzbav.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2brawhnoy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aklipzob.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2adxjmdwx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ycxykhaf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qlofwhhp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xqcchmya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcyblec.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kmvumtao.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2svmfzdqf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2albikhyy.html


<!-- 参考信息 -->