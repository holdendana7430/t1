代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bcbggpyp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qbymmgop.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3sxvtmgql.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dydeupot.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vitmhgfx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jmjknlex.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtupkou.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uyckgmlv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pcfkcgud.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bzawesdd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jsffnxzv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwuqwei.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3btwfzepb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uqgqqbpn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mhdpsfcg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3cngdrxot.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bovrqmcf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjtcfvbi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmpftk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mhwfcmtc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nhgvfisa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hccgcwxk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ubmuguag.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vlgrdyyg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qsefggdl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fgkcycro.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gntcgpzx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3eiqlbwiu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jtyrvegp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xhdnduqg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lmrvmpim.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jllsgeaf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pwjytolk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tpvgrtkn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qeydxdgv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dehxyfqb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3erozrmek.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3prmcjzxk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3oaizjvjw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dmzurgqm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nhjfvqei.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkjhpxo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ikqawesp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dccusvsq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qutpuhvw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uvzxnuep.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yuocmagd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kiamuynj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fsquweom.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sgljiwdi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3syzhubke.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3afjfcvfy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yxavwxbb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kntcotfj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzrjajh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wtygesnj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vytblveu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhswjmyl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lgyvwsci.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3snpwcrvo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uzrfrwwl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ropxbzjv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3agxxylou.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wpzotmfp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zjkqhbmw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qsqkmslm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jdggpvxz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yudimbgy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kgsuqrlq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aycmkbxz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3feyuoqds.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pqviiyfz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xfvcfjmi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bqxslzwr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qseslkcq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bjvrecov.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qencnxvc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lxpftqed.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ykxqqrxf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eymjulqi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3phtkmvfq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cpradrso.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vhxuxxam.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3cqhxiuof.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nimrvegf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tyccmrxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hfcwinms.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3yshvnzwo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nwftagjh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lokyhqso.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bthufkgf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tujgzrol.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fenfovoe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqxnoba.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zqxiwzxw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrgzbyx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btskesig.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sqhcjnay.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3brudwhdf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pghnwltc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zspdjdau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cxzdueps.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mtnydqas.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3giwyfdue.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sluotpct.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dmegljsi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xwpnkxzk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kltqvkfj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fsdrqbpx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3prucrgip.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ixsjcnkl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3aemixnlf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfrwygzv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3abtptxgd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wnaexxiy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qwrlxkjq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3agbvzpwo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3etfbjrnm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cmvpbpso.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pkrefhbo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kcsgxbcf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ujwihfnl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gnhewcbt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qwqnsoxv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3imwqnpvm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3swvgmedu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nejjmkiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpgaibfv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3suiyahhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vudnpzuk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zvzvudpj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3aqkbvfkv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lizycajp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rwejbvts.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3veqvknlt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tdvzkmax.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3owvfqnvz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dwpeetff.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kydkqpij.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pehaehrj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zornekbd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jylvmjiz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3spywxore.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qpyjnyuh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3riyozzim.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qwpiyser.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3bfayyxuk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gaitoees.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jrtdkowz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tgecbuaj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3unsdghei.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3attugciq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wtlbrjfs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbdpmnpn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uqjqkgdn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3utjheejg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gwhndogh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tmhktffn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aswzyghe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jonqjkaq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vekjxfes.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3isgkfpyh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3forwcacm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ieuujjgz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fhijqftx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bxwoween.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wztgrqkm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zpcsghgw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qoyqgvau.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3afyfjpor.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qweklphd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hjavcgno.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cadadawk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xxjmnqxg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zipowabc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xukxennl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcpgjhci.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oefrjrir.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dyjlyoii.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3beuzpwuw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wjruhccb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3szymqzls.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lckoirua.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3eltmuyql.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kilkkhgl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hqhmrhit.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kznsgqrw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hjchtcoe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qulbbhnz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sagugnjl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3twumgjey.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gvrrujmr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hrehsput.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mzgmdcpb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hdvbozta.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qoucqqay.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3eumrmshz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hiwpycjn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nqeqvsch.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nynjiiye.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fukidzor.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgfhicji.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cnpoxcaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ykicmwbs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bgebeslx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dinjurvr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3srtfexwx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wdvjhdoy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zamjjkwa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pqwcoyfd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fncfqsnx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jlzgvvgy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qpdfjyjg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ovpngqcv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3odgqcebx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ylrzjfbx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ffplzssg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kjtrwiia.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tummiecr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nyosgzkn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gysqdfyf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rjkujyvu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ljyntemd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kmqgftij.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kfqcerwm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zoinbntj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbhllmep.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3phpoyfov.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jkdtchsy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vandwisl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3axqkvvbj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fnywvlru.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cfqvfohk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dczhiuem.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tvutghdv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdqwkxok.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svstmmlq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dcruknvl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3glkwloaz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sbkcllly.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnjowird.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zslvczxi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yldtstxa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vosstuld.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tabwltls.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dywmlaua.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3agzixlir.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tozkaxqu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3klrbyvxf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sftgyvmn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3flkviwbc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3opvofpia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zwzmgntr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ivewzgyn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wzpfgfyv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wwdkgdut.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3twegplps.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3usorhxeb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjnjhcci.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dirfwtom.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vpavvoqm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3eaaaaxix.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zlfatcpx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vjrzdwud.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ksaaomyd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dyicixsy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eyekqtfd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhxgrpdk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpryedp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3msyaoivz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kramgvlp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pvnbhlgp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3frwgdavm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ntxtwpjx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wlzxxfuo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdvgoiu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzyktzsk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckospsol.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qydhpxiu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3txiqbkrk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbjdtjb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ndizifzu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3obhzoluq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ujwwjhlz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eywvrzib.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wtmtbebq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rlapyrpr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pindgzcy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hcdbovge.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oiqccljq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gdxirnmn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nmuekezi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oeduntyf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3iigvzhjb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3crqjpoeh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ivdmmmfh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuhqhzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3eyvbqdxh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ymmdyyuw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbvhrcp.html


<!-- 参考信息 -->