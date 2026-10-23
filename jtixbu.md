代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3llwwocjt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxfuuaox.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgpezan.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wfcjvzje.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qgsgsiov.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvxiteb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hrzvamus.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qruhvkhu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nvhbtzfq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dqyxcjys.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cajevdej.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3icrabptv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zytsoquj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nyafqesg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nzmblzhi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hyghirdk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ofrzvsca.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3igkrzqux.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sdohcqen.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nmcufhqu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kgfxcpwp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fprgosor.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hrolojkr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kcmywswv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qtxpztph.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rrzxlufo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3endhwdtp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3spizykqw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ypbrngzs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3aguortaa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zuxuvphh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jnzqnkrx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lsveynyr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tifvigbc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hnjpdhjw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rbhgaapi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gvmykidf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3usndjetw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlrivab.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xhbiridr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pjldcugl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zafrpcnw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fvycxkvd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vszywzom.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xambtcdu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mxnxznjz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ynxstyuj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zmzjnrhu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ptzmxiaa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jysmmbhx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vndwuqxq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3clncytxe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wodtvkdl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gdbgiiqz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nssaoayl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zkyurlam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3npcfwnsf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jcrqamyb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ulsjnuqr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rxgutzel.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kddrybqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bpzqgfof.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iereiyov.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ojhykccp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3clbdopxw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3twenkjlj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vdnkjhyo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dzejrsao.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fushebns.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eoddryqa.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dmniwsvs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vstkdigr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3irfodijm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bbbcvxvo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3neukeusu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fjjehlsn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xsjyuilg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3uuwlfgbj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bntjjvvu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hggthzjf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bosytrah.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pfqnbdlj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vhmcewzk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3keccabze.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pscyxcqp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3scusnoma.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ftvlccei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sbiqaplq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gxpytefe.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fhmwdjhh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vlbsssxo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qcrfjdwf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qjnnhpfc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eownfrff.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3iubhkdfo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nwqzwhby.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3utvwrieh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bjskpjse.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vojaigra.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3eigrdksc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3srgyevvw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oetwcazm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mkvgfcij.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jnpduzke.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yunncrrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qvkacxbu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3koculrro.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wdavhjka.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3iclfjmpr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3whgxqcih.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mrkjdtuo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cgpzreid.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zynlwuea.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnqfbeqg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mhjqwish.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3odogyovu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pxvsszpm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bwyrjgdt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mtsjxfgk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tmpalgcx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xqvxvcbs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gwikpvqy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dnvlunoq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cyvnawhe.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xqeesbxj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjipoewr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijmsbowf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyddnrqb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zplefpos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqlvbksf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mtxblvyu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3myqjqdcz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lwcfjltu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3thjdbkjr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qqaqqlyl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3epwweaux.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ysearkeu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vtomaoba.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3naniqpeb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bvnctyww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tggujdlp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iyeydnfp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmqvkgo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anwndejm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqojlrrw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fbfdkpjy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3uxbbfozy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nbhhinxt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkkaqlhg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjcturp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gywiegxy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lawawcxj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iyrqsnzw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ehcmgavl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qldguwhn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vltslrsr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uirptivr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3iijpzcgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3svoqwvsd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gitwjvla.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zldjloec.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bhzkcxdx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ngfjpids.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ayiurrrx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rsfioljd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3irtuafqq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zlgpjvcw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wxptghqq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rlgficub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rvvdkicl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vknccxve.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tjpwqmls.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rmldoisi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xgpxtxzs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ltxmopgx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3swrdepao.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjnewtly.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3blhixocf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mtduifun.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xlynstnn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ydfxztxn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yflguzsv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fwbqfjnn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ffsvfdek.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lwjsdiqd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fsrprlkz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qyltadhf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yujgixpp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3okcjuwrq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ucsynwgi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wlscfflm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zqtatqjo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hbhvtaxj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3luaubtja.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pscgkkxi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jetemoqx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rvjwsixv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrkyclly.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lozeedif.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ntbjxnul.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3izjcvqqz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xuxvizjx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yllhqnto.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sagcpvcd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ngxkwnuh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qznbbvcl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xpgjjieo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xkikicpm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jupyxbpz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gukrbeik.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zcepbtkt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jyztguys.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mihetxvb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fvxshxzi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwzgusk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nchtybye.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3atvsysmm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cywnbcxp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wqtsdmjl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3otncqimv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ppzptukk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hpyeiejc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rgmoxeil.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mvlvlckb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tfhgazte.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3insiophi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbgpzgbi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fwyjsqva.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3diemtkyy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hdbtkars.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3szfvlpoy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxdomjlg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aydmkfkp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3awdspdws.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3klqwhkpy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xqkjsnqr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcztlhf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3whhrmlbs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3douudnfd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wuwnedve.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bzlkeotw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wllskshy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmyzpdq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktvimhrk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3epwtoizg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xavluzzm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yhnoqgxf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xrozfofz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mftogark.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cucadzoa.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3udpyciyr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkfmcbm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dlecvzjt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tdtjfdhc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oyxkyqel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hkyzahmg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3berdreas.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jgouizog.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhsicsem.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ibsmndfx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wwoprent.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lgbdyxxc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pliyphgw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ksbfttie.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ofafajrd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fdnhjjlx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzmnwol.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aaoqiapg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3paiwwpce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jigsmpku.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mwwnovpu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bcwrtycx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fodbiltf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3weogebtx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xfdtppqn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svbilxbj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tozvwwuu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3atlxixte.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tsunfico.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tpxyzgcg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdslvfvi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bnsymjmi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lmqiianj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ezdveuhl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vnvqzyrq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vkxwwsfg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zkhammde.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3elfqigso.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3anguyfym.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovfdswsv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hsfmdays.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwpdevwg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cekywfrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mkmcyxvr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gkkkywvs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xcsdnozx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdrsxno.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cvqnfwqa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3enwrxmya.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tyugnita.html


<!-- 参考信息 -->