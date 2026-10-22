代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rvajdgpf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2acwvkude.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fowoorxh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ssedawjl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cuwtatvr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2coaehtxi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kpsktmxd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gvrfmejn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lcodtupw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxiwsbmq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cbpvzhtr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xvevfbnt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbbghilq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jnpqqncw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qkbxcpox.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2svyomxsp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qgdzwtpm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kibrrehh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pdhsfvso.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fkdpagur.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kvkxowxs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orajyywv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnfgjoh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zcebiktu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gvocfiwg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mmcnsamv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2naubbtix.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iwijpzqz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cuklhryd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vfnrupup.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uummtlcl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bbdrkypf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2omriqhrs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2trnurrrs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uwzxuorp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zaicmcoa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zkhylihi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2djtysjkv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wdclnism.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhezhmc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rrympezu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bigfuttx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fdeyqrsu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rzkxawqr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ydgrokey.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cvhomajk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2whelclvk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fdorxodu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhddptt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2aoubmprz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rneaqqof.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2alixvjys.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2iklrxqoj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2skfmjgnt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2otmfuonx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cicnovzr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xlvzgvxv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qsonctpd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2thwvzoxz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2elhyygcs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qunauwtb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2itfeiiih.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2phdxkxhw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vqmyrigy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvdzkdsw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrrbaao.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlyhytj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2amedeoqw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wmjxsfqv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fspkxbjj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uppxxqud.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2szsfrbaq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mdqrrbbj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mkappcxb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rremuutk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qhncrgsl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sjsodckb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mefmiiem.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wvezjwwy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2nouhiyaw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bsneuwfq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2onqzaait.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fffjphps.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dfaedlgv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2njpqxzqg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ipefrksv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2aggvrlrj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dqohwijj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tiikwabu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bcbiykuv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vnezcglf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dvmhmali.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jmdhfrfb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dnjpmjec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kvjlqawd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2akcasgex.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2txyjwfxk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlmqjqbe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yksqazvm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gucmwapc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ywxrtujq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ouoelaew.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2spnkxvuo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kdwzhzcd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhzlybkl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vawrzycz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ianmbykr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sutifrnc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rndiarqg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uukmjzye.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pobpgylk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2scabsxmy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dfhsfipe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jyffnyqb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2diilqbir.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cofnygme.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qaolgsxp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcvlypib.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sphyohwg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kpbheffo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xackbdpx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlbhznm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cukkjknx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hcebpwog.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xyijoipp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2herthhiv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ydrivdgm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jykevnpo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kfsxweyw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kxvvddll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twmqbhcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udljkilm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2glclunji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwdhivdi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bsccgjsp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lfjaauhr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wpxoonca.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2htyhyalg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dhqyoajv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gunfnfem.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nrjqooif.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tyjixjxo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jubdbasu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2euwlbhpc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hneuxcnw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bxttaixy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yvvqcihk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2quwyierq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qwkhwhqa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jnozcrro.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mfbdofwp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fzzzmeob.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2szzbrdhv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hophsywl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tlwwnxds.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rmvhpciv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vvcbpsvw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vlcsbndq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hdzzeemj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qomqwgtm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ssuibslm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ijojcqkp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xxjscehd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lspiszpa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ekpxqhxh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jjdcewaf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bgirdrnh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2chekiftv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uawwcila.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nddeenzo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xqenlghp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wuugciuv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zxhcsubg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jdpkemqv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jdkqwqwy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jcbwczdo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mmjlmvog.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ybnmnbmr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mztkjshp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dnzswzvj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oslxxzny.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lkmvvmef.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ungnevua.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tdtaseqf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2finiqvus.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gwowzbis.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kemhrmtn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uluzwcnt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zugokoom.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lvilyqis.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gmdxahcl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qsgxxzjw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2agsqhhwl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ecvbsldw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lspxwbfy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2etqhisff.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mbajmjtd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2owvorpya.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2voaoqreg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yxzrxmeu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ruerhiyt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2buwxmekb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvxrrnbr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrwjjfg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2khdmedxz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2muhbvsle.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2saibzusk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ybpippwz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xkdyopsz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2etywseai.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2umjrgets.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2oimwnond.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2akuqrewo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjnrgrqw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2irwcbgtv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fguehdpw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tmnvewce.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gutoztej.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ccuzvpck.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mauxrkev.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hinmkahd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cqhxomgy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2snwjtdlc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jokroikq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qcyfdtmf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ipxjghdo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ysapvmdf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cnzhxtnq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2skvfnpap.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ctdxyawe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxjmsafa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uzzbvpkz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jvujmbqm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mqddzhyx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wtnamlvy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xpmxzpsw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2almesomy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2deyjgehv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rjkawrpw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzlfysve.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yxxyiujw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lngsunyk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2napdmqgl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tigifyku.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kehhjnbq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bfshiksv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cmnrntik.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gkhettoj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lkgpxlpw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2aafxwqoq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mspybuyk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qhhctycl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kwmklxgi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikgzrozg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbpcyxyy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqdpozao.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mvbgsqnx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oydsjkqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jvnjcvfv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvtyeyzd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2remdedcd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjoslm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2evduwvme.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xtxrmxtb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mmrjjgmo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ljkqzuio.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bxpfbvha.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gjrociav.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dzyzoson.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2syggtgiv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ruphbmuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnzfczzg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nkoqqysf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oaivfayx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qelwsfkh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yjieczlg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vjwkrngw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2aiwphtmf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2radzkbok.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhcwbitn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jiukqobk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxphdypn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nofpjlko.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yzvamnkc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebwflghn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vrsqcubp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pxcwpwzo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ukmdbvkh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fvkmcluc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cocqnqas.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ggyzmqlr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ilrtgolo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ggzepmyb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2izbssvnp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2odvyaijc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrznucqh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hlntjxqv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2iloyhnsr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2egqotsug.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wezfhwrz.html


<!-- 参考信息 -->