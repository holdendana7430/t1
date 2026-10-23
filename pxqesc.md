代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzichoou.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jvjcpowj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctouxnjk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gpigbtxc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hgwdgrch.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3giotctzm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zvjcsgja.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sigacnzj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nvgfvfko.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xqdsgweo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tsbsptor.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vajgscxz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ricejtsh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vdnxqgmg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eblvizzn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grxqwkgf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3elnzvchw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xojmcavb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bflautkd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3sibqtahu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qcjukekz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3katwhjvm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3krkongjk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3opyijdrj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nixykipf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcanviah.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwkilndc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ekbvlxga.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ourxqbig.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uxrdndcj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vbwiqqnp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtshulw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fwqnzdvl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjczdyne.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xgltjqcu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ybahvnfc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvdfokzg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gmwvrarm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3awjvzdpn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jmihomxg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hegexihx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3eacutilx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wcsvdrgx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gizovciy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qyeglezk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3welvcdwe.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yxbgycpx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3apwzfaih.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zhftrjwe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yzryyqgk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3oqxuxygn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3niosccgn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3amggtxqy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uuepvlfi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tvygumsw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3guiskdux.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uiivfejp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xurpdqgd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nzjmbduw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cxtolgll.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fcqefeya.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vrxfgtge.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3awhiaveh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kleifiik.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3otrcxzbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ufthhaqg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hwollypu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jqtdmwxj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ifxzvmnj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nannmwri.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ukbnojqt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ozmbqnwk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ffjmfshi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgnauqcd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfqavxe.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dzabbtfn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3urljhtsw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxrrfrwn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jbexujkn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gukfocjn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ymyrgkku.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gageufiz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yirwgdtu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zxafrshy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dfybsdok.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tazozjkf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lxfgxrmw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tludrajg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yaneiavv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xfqwzbvi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cyzyzsto.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dovjlzpj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rtskkrxi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3inzvmzyp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3oregqefb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3srcetxfv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ngzbvkak.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kcmrqpxu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qrfkyoep.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ajtlviad.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zpjdjmaz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zsxdldcy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fozwiyub.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wojzbxtg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tcewxzhg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vwickqgu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3npzjiiys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vkkwdmcc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3eottqnot.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zgqhxtbq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3glfumboc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3sidjdorh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wkltarxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnorqoer.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ptjrptfk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exqepqwv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3inadifhq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wysbapvn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wmzgydpt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hawkvqai.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvwnevut.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3narvmqso.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rjrmawat.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3prarlhij.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ltxslmvf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnlsfpcj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xdgkshcr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ywdeduai.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ttgryzou.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3eqlukusi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vbxjhaka.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tfahpwll.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdrjbjjz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vqzzvadq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gzmxdhdg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hupzlkeb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ejkzfygx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mbfekxvx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lsvaznnl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3awccoble.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zgckykxy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3otckxqsu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lcwlbkfr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouqmpwok.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wnlzyqtz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzislshl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apgazruv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnvoymru.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3snbnnbpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idmthmrg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eurakgxr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dtmobeot.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kjslvvyj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ztiathfz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ahqoqckr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3eikkchjj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ozhyuewb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tmsmmsgy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hgkeckia.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3curauqwg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3csdwwlbj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nwmesvku.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kxbondaf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lxxiuxin.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zhueqmiy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qplsuxqh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gjnhdroh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ebeclmzb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zuxlimgh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lyctlfhp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3erudpeya.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3nxvayjuq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uakukgxs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ljsapewt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ujcmfrwb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dgmcgwtw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vvvmtotf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qbvrekgb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jeoexzhh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyxgmdgd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mvgpxixt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zqioecez.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jqgxejfm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jmdyegqv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uewahafr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jvzrwpgn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zwtbvvst.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tucqtmmg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fhpzmyfy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3slamqodn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vfvlmobe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qzcngkag.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qpnkylbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3szbdasyn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ureabzps.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqwqfypw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nybsbutb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tigzsawj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ildzmfsu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3htcprzvr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iymgsomz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fwwdqooa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ilizmhbk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ymiklyal.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ebhrcuwe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3herzsoww.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rbsetnpf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tumjkpwh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qaozywqu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zacrxyre.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mlolwtyt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zsacillv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ropdcseq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ybfnnkwt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vwylwzok.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bctgnuue.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rtphggya.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xsqdnelx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ejyzmeyk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gramdyls.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfoeulsu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jmctkbtw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wrubtbvw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lpplftaj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eavmjxzq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3uxmdqbnl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xouylncg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ahdopfqw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgyvfmz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cniowryf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cwmkgxpo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3puyxgbbs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qmempads.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3awsxogze.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3unaruxvz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwzhntb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jjbmeybv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cfofboem.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rwhfrgwm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3junrgbne.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ajfvtgyk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ffnobyqd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bgesgnjm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fzuvnemp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ahyqxtip.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hjfsddkk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqhmxlvk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oucgerus.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pzmrmmpm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ajfntkdw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ypketgcn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iohuhges.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vqzmvjzm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3usrovrcd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gbqijnjy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vglcemrl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qctdesbu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fruwwytt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ytosattz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sftatzth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dlakemfx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwzdkwhb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3grsmaiem.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gngqgtxp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vzowxwty.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vqrxhazl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3akqjbrdy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mtwedvfh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yoxafowx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cnqlwfeh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfkfcmi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqdsvekx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkumzrqh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pcrrixxn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjyzkmwh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvsiiflp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pdiobmlu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xsfrwhqq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3snpytfcn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xuqvpgdz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3agyyotcd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3selwdtud.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dcqaapti.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vtnvcoxr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3blsdbjpp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zxyqmcfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrdqiyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttvoricj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hubpfgin.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pzulrqmi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gthyuhyd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gaufxxii.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iajjxiav.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qrwpconf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qljzqqiu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wydmjirz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxdillfx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fgfmmzpk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yjxtkdfu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iiyduauo.html


<!-- 参考信息 -->