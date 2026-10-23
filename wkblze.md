代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tplmntli.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqzupnik.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bijkoybs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cwgrpnjr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3emvqfpfj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcjuqfg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wvawnvgu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bkemkmot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvvgpyjg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xvccvyzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhztbobm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3utkpfcer.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dxcholqb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wjbgaeah.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmehwrcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bndjuxpz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nllzkizy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3coqfophs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3raeliwrd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybqzkjiz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ltbfiipd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fucpdesq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcnsvom.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwmfmgeb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uezzkseo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3sfegzgaa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fnoyiuun.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rxooshus.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mbhgempu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bfomkmkk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3okxvjgix.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rotfhuya.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tmbiblny.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxedfani.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmkoptqk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gnwacnnc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3usczaqtb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gkurmkcj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dboscqgq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dukrajjf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kjtockxi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhpxlfgq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tjnhebhz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cmubsgxx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pomffwxm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhptmvfg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igifdryr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lvnxsxdo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zqljspyn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3obqdjfoo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bmdrblde.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ibdpultw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3locbiuiy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3iuwhawqp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yxrawybh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lvprnkep.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kpraadec.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ubolwdas.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3llzapglv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eblblxkp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yrejccjt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oztqizkr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jhytmrkj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yvgvvqke.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zadwpevj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dhsaizml.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tuxklfzy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uocibdzz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3grjgghlj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uxvfomst.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rgbtdjqu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lotcbkfb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qcfrwjyg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zzjjibaa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pxptqbht.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3imuchfxu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qblfxmxh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtukzaa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpnjfawt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tgmmaidi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3oungnmwo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjdfjqzr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxjenman.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tyzegxma.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhmzomxu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjyoimbp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lbrsjfpd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xpaxsges.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bxxmkshw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wzwkaazg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhadqovc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kjxpxkde.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3veypawlx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ghrwgfda.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ofqwpmad.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nyxcmxlo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3uisloann.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rpndlcyo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zvmgdlbh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hihfypit.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gkmqasfp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mvpcqzzf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3sqzaeubm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yhfqyazy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qquqtkad.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pmcstqzl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3njsahkxc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3famqnsar.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3pgwqlrus.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xhghkssk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tlyalqbc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yrdjqtfh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bveoezfv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hukmirax.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lktsyumw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hqxylwzb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kviznizt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jqytpkhd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kbnijojc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vbrewdvg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fcludtrb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3finqduzl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tfjtwmtc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3flneuedt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tyglghwz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sbihqdqs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3aoyziemt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gasktvxm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uthfzngk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ezjgjcaz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3diwmisoi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fropfzgk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlzetccr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwacjdr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ljmiooyj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3itvmnhpq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3sgqiuwgb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bikwwlqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mbptejnv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uumwyrvr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pmqftgos.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3demmwcxs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qhqnehhh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kbsryrav.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zxmkslvv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ojjcxgfy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kghmmtip.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zpseqhau.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dfkfbvgt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ufmutghh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zlywxoxy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mrqrtiuk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nhzzdpyh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3clylupvb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qzvrumwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aruhaxpb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cupkatxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqbxmypk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ufhqkecx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3adwaswra.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aesyszip.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3msayhbqp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jjfcvdpi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zwlqpkrh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gwbvnmuc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3agormkmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zaohuskc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dekaohbe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pglfgmcd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vymuobnz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nosvyffz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3islvujkz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3aszbishw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuexgki.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eybpgxma.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3joaaenqt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nemuhitg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hbccbbdr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3iswwocnf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jnrgmnpr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xjjgqlfg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scsfyime.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqhewdt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3aohoeeiv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cfnysmyc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gwqniekf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwovxua.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zknkypdm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ndxpetuz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cqtxofrm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ydsfwdlj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zmdjonpk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wusrrjhu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3spbrsubk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3omdmzqyp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eplqxnii.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cvyltbpl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gukfousp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nwjhtrfp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3csgxjnyw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yrtabqmb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pwjvkpap.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jbnfeagp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ojodvkxa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tchoeqke.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqbuatdc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gjtlrsbt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sybkbytu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xrsxndva.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gwbxdoiu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mmuzrvlv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nlotpoer.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xxbrwavj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eyouedbp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hfpgbbzv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zenjqcet.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dvrqqchg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jkuleqrr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pgzdjgey.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pjfifdhh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nbtcxwad.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3txrwxzvh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3apkrcweq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uwbrznmn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rnslzjzq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ixevfato.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zhwknbya.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3icnjdtxa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhvlqqi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hbyzixcu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fwfsllpr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3apghgesc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jolnrgqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iybabqna.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kyrmtrdw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ysqjarfx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzvixvdl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ffggxxuf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3katqvoup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vlqocata.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fdrjvkis.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pfsckjcu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3deumehdp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3trkiimkf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bcewwxjz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tbzsvobr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tyhardxq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lystjbdc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qodrcrhx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tsvngdqq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udeocirk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mjekdoad.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hnqivjnb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3obvxfvui.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nouekshr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qoyvqzmp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3btuyosny.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ctbymjcz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3gnxoogsp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mybtcryh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3youxqzqa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cvtqopgv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hbdhzuuh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnxqqcqk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvrkvnay.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dbalmagq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cvzxgjqh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lvpcfxlj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rgmxrjcw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrfrbct.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qjirkqgm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qwtdonjh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nzlkzhkc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hkujgbxl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dkzvkltw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mibspbos.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3npdjrowa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pturvpfp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yttcqbls.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkkakjke.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhjzddfg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wrevlypp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fibnyhkk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwfpthkw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3sgyfwveu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ljjfbskw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drsivuew.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pitvstfk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3elyaemjg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tumhfojy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lmzllndy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kuywyaaa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wtvfsysg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cylbwnbk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3raukxvho.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxighklw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dyvnlvzs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3noxmlcxg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mnelgoan.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cujnybnd.html


<!-- 参考信息 -->