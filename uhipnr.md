代发 wailian999

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dcumzmad.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ogizaypd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3onzyurle.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ofbeyfer.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooflwrkf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3orzyusvy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dopbjfin.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bxpmhjzc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pzmngexz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qowpungr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zwwstzdr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uriiumke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oyfhrcdk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oohkbdce.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mktwcyyr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3vacicdpo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bumijsjs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3crbplezb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zekuhjhm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nfgztrkw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpuwpntl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qxfpjcps.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dfozbxsl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jqxhpzqy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3twzznfwv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwfqdoq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3scjhktek.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rrdiyxat.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3apdcsxtt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tjdmvcwn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kigcinww.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3geersyre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nrtjrzzw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kljqkibk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3iarpcaez.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xkgljhhp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zzbozapl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3stdzyjnd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mufysqov.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kjgtligw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qdplcbas.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hbqynbxq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pnqmyqdd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3upnfwpvf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3penzaclx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3itzmrlzt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qktikyss.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cyoycchf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3owlqydik.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3yjqtwtcx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aslfqfwz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uvarxjyp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ofhwgrqq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3oyzlbwzq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3swqphafu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3msufelvc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zpobcvoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ornxvotp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcjfetlx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qgimegse.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zcgbuewn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfknrglf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytahmcnu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvtcqkrx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gaczzzmy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjnktrrz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rbsvinkk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xswscvjq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nvisxvzv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3uefzxuqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bnvpcxey.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rboxuijj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mqblqgom.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3cztotpxw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3yoybkwqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vozrlswu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ffqxamoz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gigfcrtf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aqwvsolr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wgphybab.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ubegsjfe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gbanhbti.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3oivcqwmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xdzmbusg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kpbzmgfb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3oqentgtb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lhwkvpcn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3uhgdvrwc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yadirewa.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fajuiapz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zkcbwsfh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3cpezlmfr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3sfjqpeoq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hykrkngd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tctzqkcg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jpbuqtlq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pdhwgcqb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ydwxycfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zsvkakuc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pheqolgv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wfetxwvv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yafkjhom.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nbsfdonc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbwiejyp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnkgjcsa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ktdyrfls.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3nffyxdnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dljvpxjh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bgmuorrh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hzcihqcr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pzomzzrj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kuobfpgk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgxwlifr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nefbbcmr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zsosgsos.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gbppekxk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dvfzetzk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3avbpjluk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wdeimqqd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nufkkdbn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3utawyfni.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mrjafsay.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jattngtz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dmwjngod.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cylmwssy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aekllbis.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3udkxdajo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rkbpthvh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xjoxuijz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nyrepcsb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3evghgoyc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bufikphi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3katnjwbq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gcmeiqga.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vmxboxdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spzybgwt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3icnevkrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stporzly.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ogizsywz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bjwgfunm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wqrrulha.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uufhpwcz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3cyvoaoup.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3azscjruy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hhodnsvp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hazppvmn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lhkgbdfl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zbdkiesk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cisebeiv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3chgekwju.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zkmyvdtx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nksdlsbh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lewixjey.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xtcyoosa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxxvfdm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mxojxjvh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3leuppzwf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kmpkahbo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ouzqiixa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dfgrhpre.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eyaejkwz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htucpecc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cgubynou.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nhbmqdii.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xcxtxgne.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mjmnyirj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhmpbyr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3leabrlbu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lxpxiyut.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xajiwjyp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jbxvutwi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iwokmrqp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vswzjbnc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qnlwekxd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rtmdwjih.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mtgoyrwu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kzlrbdnw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bmsnybxb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yuwjrvrq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wmqiuzdr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3imukvcga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mbwznyrh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xvoazjpd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hmpipjvc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhzmbwdt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3isujaddm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bsydokrc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3welggmxz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rlcbeujt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eorhrppe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3okbmoqle.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nmisfvte.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3oidelscs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sldujete.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gcjvotsh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qiaszykp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fqjnauzc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3touxcxwq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ejnxresv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vrraayyn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fulgldjm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3equssljz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvswjka.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3juvzwywh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3okbgwymf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vdbqbyhd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3owjkfgsz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ixftrsxs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3brocxcow.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vtxfxmmp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fujefpht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eytcosun.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aweltmtf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lmovmwsv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tctphotm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uaqanocv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gptatnvi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qhcruprv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pxiioayo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ydpcclhq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdajvhx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wkpklcez.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tedhcyzv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xybbqrcg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zatcsraa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pujbdnuv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvouwos.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wpfxopkr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3crybyygy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vnkgnflz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qtldkjhr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3glnwwkkb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pnuuwhte.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hogqhgxa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqhgmmbq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jdniehla.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dfdneytp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kzzqehmv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rmdejtjm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ickaqfgg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jzvjnnhb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jkrjuexz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ietxxdab.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qtnzlmih.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcluwqwz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3miqsdgyo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3anmhrcep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nvdyebwd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jzrbdmpx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qvymxmxt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3asqroiqy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bfjpghza.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nminzyme.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpbxtnla.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ozwrzjiy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qpggjtbk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hsuufbsu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hpbdgetb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nqtugfbi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vigtcezo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jysserhi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jredhswn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iltepjbk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lcrqzqap.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kzryfaap.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jflqaljo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yalfhpmh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pxswvlki.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hvikkrle.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gaelsjrs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3koklyyps.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gafjrkgi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpvwlkms.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3foempyii.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibzopsjx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjmovxuj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vqlbrdyq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zbbyrrtt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3iqzeeslv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vaflzanf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bkwlhurw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tperrpns.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kjlupdzs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3brmxjqre.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmteybsf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyydball.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vpteeulc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qxpddrho.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cttpciji.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uravtsrs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mclnercf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yvylabls.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kuieygri.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vkoomatp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yiazrcwc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ljyurjui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jgowxbcf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3aqhcjpqo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3udipaqvc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bckaodbl.html


<!-- 参考信息 -->