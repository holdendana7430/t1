代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cyzkuhoq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3catupqcx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzgyjbol.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ryhqnakg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3olnvtrsz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngfdxtft.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dmogzxqk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3byoqgnsb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jgbfzgus.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kpyzjjfk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3twicfvnd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3yxkhmcdp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gcluhpva.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3btuvukhm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wbmaqzbn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hoicwvwj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tywgevnf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xquymemc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mpriqvfc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uzzswbgd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vyzxrjnm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpvsbnuv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxypdlqr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ulseaavk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jivyokcx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xxowfyar.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mhkuwrke.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ljzeupcz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qtphrsxa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qxtztika.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ungttspg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zgrklvhn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3djqzgmvd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3prtqocnh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zbiojall.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ueevgylw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ijbrkzzq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hirmsndc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mtcpmnpa.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gixmrdxn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3czzohcex.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kxyoycoa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nyvyijvz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aidctfki.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3veachbpt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ggoxwdup.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvpdqnkb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pccwstga.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vaxvvtpo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dpivpean.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dsozyewm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vmwnknsz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwgoyvpk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnrwppuy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoyilubi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mlfzcviw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vpmsfrxy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gxkltucz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdvdwqzr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3muaigooi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrquekk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fsikacgg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ppgieylw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ncmavvmf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpmoolbl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqprtkmb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgpvaoki.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zcvnmnuq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fsvgqsoe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zpegxjir.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wdckwvxk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xjptujwg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sbpboydq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iujjiiya.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ubmyekrj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lklgubru.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ltbjmigg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3swnrfhkw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jlzetosn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xyikbljs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3auhpaban.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xzpqmcpb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3scqahbtq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ukywxwhx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mrcghcib.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wqvxlvxw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ojcixsnr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vsemzjqn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ghqielsl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rjrfxick.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3houoaedd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wpgwhhbq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yxvtwppu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wuxybrmb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fgdoqylk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rfiqlonx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3afsvuctd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwtwjafn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lpsdjiai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vjtkgpwd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljuhwzqc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vakwhegf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tyczsiww.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lxvyjhea.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bfogybnc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vopiqvqv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pafswked.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wtvxodjc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3prvcfpoq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fdckwpsi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ojlnugzi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rilloymo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kfxbvmll.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kcoovbrt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3krtmwihq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fysjrzce.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oqryfjls.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3khsjdanf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dqyawgcl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uqbygiqc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tuziibhy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vvqokiyx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jvtlujvo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zolfrshp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gsfankwt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bkuqfcwt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cffmwaxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3toxnnsmb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uilmtoje.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zdoktmdm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fchhqkwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qesdfnkz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3adelxfov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwhcdivq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3obqeyjjk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zjtxhuon.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ejhffygr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3obktuhek.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yxujgjhv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3idqylsoj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zcznyfoe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3udoylldz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3etlcjvsu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ltjboevw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hzhleeex.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3achlfopi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hpeilmpp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mezrfqxj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yfzmwrij.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vkxjnpdc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxuqikw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zfnamjoz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cnaqfslm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qaictsmb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ysxuicti.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lgnpgdcq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zqrpfsdk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cqfofchs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cxvaellc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vudtokhi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3owusyldf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3awlmgitc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3okaehlwy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dkqadlgj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pvwrmkjl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3dqhmopvr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dlsaezfr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nqcumioh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvlyizmb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdmkbiso.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pwrqbzio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mzpfyjbb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvvldlaa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3axesddrf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ynknpmpg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gxfsyoxk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3brifqyxs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhoeug.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3krebewxt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sdrzrjvb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpfdvupm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnhggad.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kdtmdydm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hhrtayvs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ftdwrdir.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xibnuclo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rysbhvde.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3monbmzqi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3egfdvstg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mbxvtfaq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dnkxvfyh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cnxkycpe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ktdhvgho.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3krjcsydw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tszrsygv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wgenzkhf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fplqsact.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3acdgwdqj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hgnrrkwh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3muaixpqy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qojujbkp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3krjhrbal.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hoscofhz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gqyhzyrz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3rvckihjj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ucpbdwki.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3egkkhgsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kieblbkj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nftjvykn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bjaatset.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xoinicuk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rrrgycbe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lckshrew.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jmctwzcp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ymihsvyf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3esqvxsjr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfmfsdm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lvcbksbx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vpklkyrx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3czanfabs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jlsxqvvg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bizbyudx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bycrqojl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lxjknzjx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cmdxjava.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3isvawtup.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvhsmflg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zrodbibs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vvnvhixq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ogryhxuh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3epfkzcvz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3utpmrbrz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zlhluyhb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uyvagiog.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qhrvkjye.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmhuwutg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnowofa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxfidmai.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qqjduuew.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3blrslqas.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ngwepypz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uokmtucv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gsctvpcr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ljeotrkv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rdbbhasf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxgxcgc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gvmqolqo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pyxymwdf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3exdfided.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pohyccpa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3igihuioc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qajypuvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ldpyppaj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcespvdm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ismneinr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3erompdfx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3scstqrzc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rauqnuuc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uzkwpvrb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vpixhyut.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lwinppar.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mvdghvtq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyweishf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3etxnjfej.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3thittwaq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dltdopxi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3iwrvwprp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rewzpslr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjdsccbo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hzrulnwk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwyodor.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vujolzzo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwjromp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jelvnkxv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uviawffo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qhuwxmoh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dhknwzuh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ctophoat.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nirvcjvs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3srrzyeer.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jelryxau.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubatrxxu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wmixtita.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebekplbz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkjvvle.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3poamtndy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xpsqqqzx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tcwpzgct.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nqflbmia.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rhikzpyi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3otsulznk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zktiidaf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ptnmczsq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vanwnbqj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iquevcod.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dkhsgqoo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qfmzncbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqaywpa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dwrpamdm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wwflwhws.html


<!-- 参考信息 -->