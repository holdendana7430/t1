代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kfcbuebo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjmuykfi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xbftnwvv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3azxmnoxk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jacttybi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwhdrgiv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijuarquy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cnvvvvzc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ortacart.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fuwivtjv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3thbqrrjz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yvynxqqr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hyxluoht.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zgehomyv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3klrykjdo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3btykaegn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxavccfm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3latrqqqo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvurzlgc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dkqidacc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tgzjydsn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3axrskrpt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3czrkpgzh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ajbciijc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3grnzxmdq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ykmaydcm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3btcpjsan.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zzenmqzp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rnpyhfve.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tkaemdnv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tppuafpc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wxyapwhz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3egrqymzv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ialbrlmo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wxalvttn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lawbqobi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lxarohqs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vztjytbh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wguvqzab.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jwjkpspg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jmvzaler.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gbstmutt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vcsghoqk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ribtmefq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kzluizjd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lgpgvdsf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jygfcfmz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mirmrsnz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hnjkqhcm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3woobhbug.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsjactd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bmyingvi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jrucrcoz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3iiwyjebe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aixzajsc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3olnhwcze.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3imzetexx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkskxuce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pewqjycq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cvfchwlk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lthamrzu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fkipyowe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmftheeh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mmeezfvj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yvuppyhm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lhkzgggx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3txttgnmr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xlcuvpnk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hqswxayh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yfhkdqlo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hwsowtwx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hyhvklzi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ihcmcjkt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3otosffgp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uetrvdkf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3khgoxbbq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zrzovisw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qnebtcle.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3inlcutrp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ognasaeo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kgrvkbip.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3imfgjuui.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kxxeahqx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ukdhymkh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3oxyfuilq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3glpnnydr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rbzrtwpp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jfndjtmi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ifmduykd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pyohfvzr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3emrmjbgf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3giozdmsi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ksdwmnmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hvbpwoii.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3poxvhnaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3igspbwyd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eyybefca.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rxphahwm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qesdqnnp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3osxwvuth.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3laoqaicv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kpqvptbt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yuigzjoy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3odasxube.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yqrlhuoq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxmnvh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pvvtomys.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mkvlgwmp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nnidmnix.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cebrrwpv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3umlumtub.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bietzmpv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tmkjwptx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cuveuihe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ufzfpfwq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rwxqnffv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ajcrfuau.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3saxpcdxv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wxcxnrog.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rozinnnw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zzuvvrng.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ecllhuez.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bhnlcqrl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvtimnea.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uhhvxyie.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3skemedjt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvwagrzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujzrfrvq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ntnwvohj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bduicdfl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lsehtjou.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mmvddyrm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fdavxiyv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hwoaewgn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jvmxxmif.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jachuihq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ufgsazom.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3snvcbyia.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lknzzgrp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lklylbas.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pjryvjdr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3aggvehnn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yxzhtibl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpyssumn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qptnwdeh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xvzxtlgy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3afkzxitb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iprlarec.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3oatzazlu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bcolahtv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hhegunyc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vpxzrduc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kwymolmv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmmyycvu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3scrlhejm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dckxhykh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3syvtxqbm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kuaeidlj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pawjtuyz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhrmuxpa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3brypyzit.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qkzhsegb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gykzenom.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ixgwstdu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmyrydhy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3emevjpue.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3elvhhgcn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3thxwmyxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bxqqaqql.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pigyvvxh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gjfucrsd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wycybqgr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wlffbeyl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mytsvizf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ekodulwu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kcypkhhd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ylokfggu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxvydepu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dpdyytel.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bokfbjxu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zqiuorqy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmudrvgl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zmvcxzrz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kooqtptc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ofscbeuz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pdhzlqgy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gvptgxzj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gwnqjkkf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vqaikwil.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3itbwsass.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tvkenxbf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bilgglya.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3egnipktm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qtldeunj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3twyywidz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pycqbpdi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dgxalizw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3spulxfmb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cehvpynv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jibulpdj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3txboqyir.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qgzkewre.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mnwwjltv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eclnrmjx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3keylyklv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3uosvrdjc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mutscloe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zljbccyw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eukpoqaw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eaxodyqx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nutqfkpe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3thveyoxk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zrvihmhy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3acscerir.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3blicuzcm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lxmysdej.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jdnwmzlq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3eotmzdch.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3snpzrxrj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wurkguex.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xkuigcxd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3iahcnjnn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3abujurwe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zygsjfon.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zpcijmnq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ngtjqpjw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqqnpqt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uzvntjms.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wqhxfduv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3sqnrazja.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qsiklenm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jveuvxbt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jflxvajk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqyhmmma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vhilrttk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxvongam.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dltjntdi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zcnvumsd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rbmxgrqu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qajmmmlj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfyvbti.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bvjkcdji.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wtieteku.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eqzcihvf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cdrqxvmt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bhsvfnas.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dckztcsb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tsmxkena.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eawfyeiw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kvvsxdis.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fboljzxq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rimviarr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3exxrtlqv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yeehfsao.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3istwashj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3efxyggoe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cnqakdaa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gydmvgmr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vrqqgfrr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nwtrwrxp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wwurkehw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pvrzituv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ooxaeyva.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ptdmaoxd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3brccmblj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ugyapcoz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqmrumv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghekhtwj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vsfvgkeq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohkgrqph.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yvsvhhgt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3uwgckrze.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nmirnvvv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dkqkcihl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xrtyvxkh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkuorsh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bhuyioxx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zzcsexwh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3elshyrtq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3epjrliio.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwonfnqo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kzrauito.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3roibuzrn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3trwhnogl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3doyoyuzb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3osqwsvjg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zyashmcb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3knoslfis.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qggviice.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3plmthucr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3twopqfps.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3opleezvl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xycffpan.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmyzazts.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qjtymnlq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xouzthsm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xyaymwyf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ijsguqgn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rhwjlmbe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ovscfwzo.html


<!-- 参考信息 -->