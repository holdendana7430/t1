代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ggsrdwqr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xwvciuma.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tmiedswu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxdfvbi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvngvxzp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3oywvukqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dvbaywga.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ncoplxaq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wzkrecna.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fqksvlbj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3lflwsxko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dolxmzfp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rydglfyv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtyyrfx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nflxrfzj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jpctszmy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpswlqgu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vljalkaw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tsrzohll.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bmxnjjsf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dkffmgmp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqdfteqf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfdbbr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xfpvhlwh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3sdnhousc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtuhxqde.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ieahhilz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cmgxuosk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jvkbjqez.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3emlmdawq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oyzxnfvz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ypwuhmxe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wllfpbvm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3iapreope.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bdibeted.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hipswnau.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kladbjyw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xuptbrjh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lrdfafnh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mtoqrjkl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fekkzcfn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rtkknacs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qneerpya.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tblsumgm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfhkilyz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dehvowib.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbbtikx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hqjqjuwb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3knusntgd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3crvblwlf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jdutcyry.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yrxwvcja.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3myfntztp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3szfpitgl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ckanalbw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sybgkwer.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3whqsiylb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3krsngopn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qlfjvqsu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hwurkuqp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kflybinj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ixhhxepo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqqmurb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3heiqwzbu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vqfterxq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xenmbgly.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3opcfnbyt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lfvsshjo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpstlmfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3oloyawml.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wpfsidlx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zcrhuyex.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zugpbyfy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rwcgdwue.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cxiugngy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vhpbcrqh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ecwpnwlx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sncvfvft.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rqyexlvs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlapqh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cbhfaisy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3upshbgbu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yfeauysn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ljgjjcia.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sqzbszww.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3chonefqv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ugmhqpvf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wqjqhpcj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rdzagyge.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3dceyrxcp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cjlzkmth.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3foitsxgg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nysjnyuq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ablzxiuk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3surqpufl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bonaqtpk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3htzqgaax.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hoelhlit.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dkuxjeuc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ienqksuf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3akfseohx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3awzssenv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yasbrlxm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaklvtgh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvhdlllk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ahccivlf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3iiiwenco.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dulrjkwu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jqndpuek.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ljgdbbtm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jiymdrib.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xivxuzcn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnuaotgg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryiiyrpj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3oghcuzmq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3whdlyafj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3snmsgcyh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kskpjvau.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3blsmjere.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sqfgkewp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfddnujh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whmskhpu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xgceejns.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3otftnsxh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ybttodei.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3poikgkrp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3aoudfkka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3brrburym.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yarkwoon.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rxgdrymy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3teqpviho.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sdhvrhpf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rdaojhzv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nrjcgeux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuvnlhcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oftvfnkk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3klvslqhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbtfbazj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mddlrrib.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3didmncsy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fnggeinw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3inlfbhsx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rmdffbtd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uzuyccaf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vxktprru.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3reoupluw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xdscmtgh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xgavbyrn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mtlsimeg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3npnbgfmj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jahdhltd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3suahnzuv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zmdldnoh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3todpheva.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wrnzimgz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3isdutbjx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tzntsgus.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyflgbic.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3obiztqfg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3aplunrms.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lrsnolrf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wvlezucm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iyxfhmlp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3osuzlzbx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pcmpvtmv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3umqevxtu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ejbxfdjn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rcclvufg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ngvtuxbx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vubbsmcw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tvlgcojo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kbdiasyv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qzugekcm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ubxlcnzb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ihpnuvbe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rbwqydtm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qpnitjeo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bifnwfza.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ripxvzec.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwroztk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mvjmlvgm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jtidaazl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nlirpssq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ubsnohre.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjnbgczp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcvdllyz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zmyewfqn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3totsbzae.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wgulylfp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3icmbvrss.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rwktnauj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kzsabtbj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3llgovdoh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ijwwhwxw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cirddxgs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxtzwp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iftutgsx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wntldvqe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3djrogfgu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3saepthrc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aheolmbx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hxrjjzvq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nlepbhqp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rbguuyon.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jjiyvoqd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3roizbxmo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hnprhaum.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xjgddfpd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntaxirou.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kxooibgo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mkhdaezj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3symoyjcy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fazezytc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ckgyvjtx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ktymslhk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3buahngxg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mifjaplo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oqarlpcf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tmxkeces.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cxcfnplk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ogvppuzk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gisgfcsw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zpvvdxwn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vuwwzgas.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vqjeonlm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yqvcaldq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3scxbjdxn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3orlgjbuw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lmxkzxov.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yuvzdvgn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkjfwgte.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hvuxidpk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3riillgjp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fgqetfkd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aipupalp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fuxzqgnf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kmhhgdru.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hieedsml.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pdfiurpd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqsusugm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3shjjqtye.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xxnohsec.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3epkhonvw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kwgkxcgh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jqvzlnad.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uzdzpoxk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3izwbtefr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tqjfcufd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jwuugqvc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rkgokvfd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlamnza.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3akghbscw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zcfvcies.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvjxcgvf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mvzcjpfs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hequkuyv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uindnmqp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ncikkeay.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvieumli.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oyijmxwk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wnnvoevn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cnlrvvuq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhdfwof.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tdgvkmzq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3svhsozqk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hwcwsuup.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hntzjjba.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fcdulibs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kkauuhfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kpxjgkur.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cimqbjlv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lrlpuasj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mehtaasd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ztbnmrko.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3droalhof.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3obhnuluh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uzselmpl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3brtddeyl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zhjjknyj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rwwxhkcv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xqeguneh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mxeljwjr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vqmgnjje.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3adeqfddy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ejrnjski.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ekdlagna.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lwgzozse.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qszyuszg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihpviyjm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pndrhdxr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qyztdnlk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bbwyfcwr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ybxobhmi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rpynuerv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhpehwf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wrmczzns.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3icvpbhtt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fqluqsay.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jbimmbzz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3olilbvtw.html


<!-- 参考信息 -->