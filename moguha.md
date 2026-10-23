代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuztcltb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zepcbaxj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ffkbkkii.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kykwhvdp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ewgfcyqc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hrjgouai.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhhbhwak.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhxrntj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ijrnwepa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzcmifoy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kktdibxm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gnxperim.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmsrcekt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mobsxcne.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svrcquzb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3htqyksco.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3enogptyj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gbbeiycc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3numcuwos.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fekamdfp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bsemwlak.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zvpgtajb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pvmvispn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3scczvghv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bpvdsysh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nxdmmstw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3avhsfmfk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yzhpfjqv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uqwmomzu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hawjsuak.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jcufwepj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mcuwqaur.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3adgchnta.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ukhhuwwn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ydtpkdno.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhbevcnv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tawhrtsr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3objhtexy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3owwspsfw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wqnsbtfn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pvyrcseb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gujqkbyv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vdiaswmx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qrnwujmp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ameivgon.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xsgiowfp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eihkcnfq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uvcucsxy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uyakcsrd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sgiesije.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnlmwqf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gixscgry.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fbudaegw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmqpjnb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vdhwxxvx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cgpqfekq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tjdskjeb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qxibqusi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dfefxqnb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hzztiqjw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fptukuab.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cvqurwuc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jaggsvzq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jnogdoec.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3oqcftxtm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3huhymdgp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kvjdqcxm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xwufpgih.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lcomqsqx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eyusgxhv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cxgigdnu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rbfkokai.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sylqjobw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zfisiskd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kqtkttxr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sroptyvh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sqrbhgev.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3suqjbvxp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yynyjhng.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3zskywtmm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qovenhgy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mxlopoqn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3okzjzpos.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mywinpfy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yjaykvpb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qapymznv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wrkcjoba.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vqyrvvjy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3otjjeyok.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qfogiddo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3khqhtgma.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsuggbjv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qxpviful.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3whdphvij.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ovnperdp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uctqfihw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lnlxjufg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yqmltjxv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vfiywwqv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dnsxjued.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3utlvfsop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nwuwuaqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pugtseke.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3atwoqbsx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xitziqbj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dygacusd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kxnskftc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xsnpdjag.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yskvoafe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfrnlufc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qhuclqup.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lsxzvfnw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3scxnywlf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3upctbswb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fchtqoop.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mmiedqkm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3akonmlee.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rfhsakwm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fbypropy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zrhkncay.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vyaqofrs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3msjzkzxn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpeyrtxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdvqtcvm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3psrdqkod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyhgqxdi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mckbwqvr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pqxtssvv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kxuwevma.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ckrutjht.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zkvjnrvd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pkzincmz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ozmyuiej.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pupfmqsu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wxkhhybk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3kgpyoqwf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jfjmnnld.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3sfcoqrqf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pyiyiyma.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mjmwlggt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3swgyesqg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sjleubjg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kzuxcvtp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rqszgpua.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hlaqeaqx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ebchjxhs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hojwzktp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uccdhxgi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjlninwf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ibwtszfl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ybwlemfp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fekatycv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mhsvlxhd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3egeghfdt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwsutnub.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ekjogkbs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uriphvtj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jooikauv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3psoobctl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bpkmsnag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3omokoilk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vtaljxyc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wdlvubkp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3quqwdixm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kquynvvx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pwtvqhwo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qzylspgg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ecjxhpor.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3htkmlywm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bxpnhmtf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3werwksak.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qujxbeep.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cfwavzuj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hapkyufx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dcxusbpi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lwymzzrg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jyhrfgpv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcvpykgj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bncavdiv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ofzvqjvy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fjnjctwf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kdgemnuc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tfalhxke.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vxcbheuw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3icftidao.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ygwdeise.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3duvtmcsd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qxlxflst.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ntfggwdd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bkkkdrpx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtnyegq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ywhqrula.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vbziucja.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3uglsbxaa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vgucjfzy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cznwfpga.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yjmxrzzj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bhknxpep.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wvwwsbnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bgqdconv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qeonkdxk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3iinviojq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3orqwerws.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fyzjrkjx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sroahaxu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ikrxmwye.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xgwfdmpe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vyiqotex.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xfpxcpxv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3htwgdwip.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tzivnist.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cslvhfms.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bdaicivr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kadqslfz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aninqhld.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ronszujr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qukonzgj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3neobihpb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fnduiely.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wveetadg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vtxhupjw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ofnijbat.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfavhhmj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pjovhtgp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ekqqjbon.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uyjrioqz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nvxtlufo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ziydvszf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqkelknt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3letameef.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zmzjajnq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxjfsdjr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tnawnfre.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3mdrtkqlb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mkuydiqh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgnhwtou.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rmybhbjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tjkgvzeq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcygsnrq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybftdnxb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mlmgvcxe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3puwbakzy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vddbmmoz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qwqmyapd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kvzygwox.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zyflduli.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3usgrnhjw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3slzblcgt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3akcvpare.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jirdspnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3evtdgxtz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znnnbbtf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ymbuoxpj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kjujjiqa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ryfszzjd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gvcztmeh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3klcivzse.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kmyjgkiv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rrbtqjyw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cvevkgpg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yoncakfr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pybtxhub.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgddxrha.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ubiwqevq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dquzindp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3isuwdgsu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gmnnphlw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ssmhgvmx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kofwehzk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3odhuponu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rqtoqwlr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kwevprgy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvzrwtzs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lvsjadbg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijfthffh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eaxpxllx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yibybtoq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3surtqlze.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vstflcqx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3eyngykkb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nqfgxouz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xwvrtedo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wbokaeyh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jaakjuio.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3prdplunp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mjadcnmg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fqlgauov.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xeyslbqh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bnqbrrnd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3quckixjf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yvcqpzny.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uuhniclz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pszlseom.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fuhjnobe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jxrwykpv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nzxzctoq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mivknwpu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nlnrhfhd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vqrgcqlo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bguufzxi.html


<!-- 参考信息 -->