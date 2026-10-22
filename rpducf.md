代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dqpoynfr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2puglluhe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2emrkrwwo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2couyzbsp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zhwyzdxb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2havxqzey.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pqjsiguc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2avuyrtnj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lielkoxs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrzrfevf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vswmxhqc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2otaaztul.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkhywxdq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2prvycych.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2pkthmkkh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qkttafoc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lvfapnfj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mceednrx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2eogtspng.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lmypdaiu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nujwbkck.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2logowvet.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aamrorcy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2riaciqod.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vvpauufb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xmrhmxzo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wdgwrano.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2czyostkh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ipmplzsq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cgakogwe.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jlsqhsba.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lnhrcslg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vomtbhvg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2btbzlgxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hyaymexw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2binfrzpq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fzgmfatk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hyugjpdg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2axkyevaq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2skyqoaqj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xphyuzct.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xoomizto.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2banzcftv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lypuefpl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrnyuyh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yunzljjp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2igicldpj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lkgqapri.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2itayhpko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wtvoecpq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mckasjhb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ihlmrtya.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmiqbemt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oujyxvyc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrpwkqp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qtzievne.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ucurqpvd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgsnrtid.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfalrqlu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vgtbcykl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ooozhgwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybnlzhow.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kntewdam.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nvzmzzri.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yhffchcv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yrhnbawe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2axqmqfsv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kpkcgtvh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mmyhefca.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vyuchfdz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wbxwghcw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nrpehldn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lihvuprs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cnxbthrf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imiaknza.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bpzxxbbn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ocmuxqxu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wlptouyc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wqhgraxq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bsvfqtdx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gvicmezj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yvwoompx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zzgvdzdn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uargyuln.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hebmgcrl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lrxfiahp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2guhvupwo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vpebhxee.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ivjkmjuf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nthxnaws.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2asefmjol.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ncjtjlse.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pklmfxfg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qfvchxoe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vcdughld.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pbzggwar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fnqnzifk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eizaokqz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ukkmchsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ihkhvgqf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyegqysp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ehhcvuna.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kjnxxomy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dbhzdjgy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kcwrelja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lqefwani.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ewjcuvgg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dsxhtcof.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dimxhyzj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2spsjyflq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xjwmwiww.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dgcuucsa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qtpuhxgi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vlkospxx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2womoihrd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2eqjbzhld.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zpjxjfou.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnqqapma.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oiglnynb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fsahnbqc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lbliwffz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pipfcvba.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cnyqsxsg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hxmuozbj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vbhiaozl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cucaedrw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zcycgxln.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjpsjoye.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ihpooept.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lgmocwho.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2slsiwymv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rttuvkqb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gbdtwyko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emzhjrye.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xxmtzaqr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2erwaqtcb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zulrcekg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wqgjryjj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2llrfgute.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qpmsqzqq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qhuydwyz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oqeeculc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2atqwpadw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nruvrext.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wablnhio.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2liliydgt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wifbyltz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gungryur.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vaeyzczo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ttutaqpd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tqrfsfxs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nbynvqwu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ucbocwls.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2heteqdva.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rstqlwvw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qhacfdmw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pmhyyayk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjslrwat.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxyjaah.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2skchkpqx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vptdgxsr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2urpxvlfb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2enfnmjbu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2juuwfgzf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2emtedxdb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iqpqrppj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hwpykdmi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cfkhqjyr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aiesccrl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jvpylgyh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ixrlwzxu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eusrscfy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2akfyclob.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bbzvfpow.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qljgkilf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2radheuqj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fpwongol.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sgbazpop.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gjqfeekj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xzpjjaij.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fimehawj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjprurbk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uujhwhwm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2peggqdqx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qaiqhgbs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqtbeiy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kttvujpd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2lpjaemlo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kfwmhion.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rsqyflle.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jmyfkxco.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eupvrmtl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvntdi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yjbmbpfh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gqzlrfka.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2svfxrzdr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kseamjyb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dfmefvzp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hjrjorvo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2epqqbooz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qmkhqjbs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2giggulcb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxolbzsq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bkclwfow.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nrtpzjcs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2htdahmcb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rvffmdpg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kixwukbb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zeyvzpon.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ovsspstu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yqmroxwn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tasyktkv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhytjyay.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uxkbgyyc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tumjabes.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hjmjpfsu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdecivo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kkmtjres.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tkzbqxac.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2klenyrkg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xkvdicle.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ctavrwyr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jwdeabad.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eykrmedf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ppqgghks.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qxbtczcx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pkszfyrz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mirfzqrl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zkzfezmn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ilreaqmt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmyqezxo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uikbyhtf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2holkksmc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vwjyatdz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mtazlgni.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcrtfvic.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2otqiofen.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2amgwcrqg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jcreszrk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ktpleksb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgecydj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hulbvdsp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yynmbsyw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2oreealia.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjqvlwma.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uwoafjmv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ailzidrx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbuevkwg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rjwxexya.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lbheqadh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjvcymuz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nnevepme.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rkzjrxui.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjlksgjd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iybnkkmr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iilclrbh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhzwtgcv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rnxwbqnc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vjhdflxe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufkkwwdx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2acuspzrj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uhhekerp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nbqqnrpu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mzmkieof.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fffucsdx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tqmmjagq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lyxxgwsw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zxxzugbw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjfzxcel.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kiajciiw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2taxjpcph.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xbpdirce.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ywdgeqjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxavszh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xbordalc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zectqbim.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gakrbpyb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wuizcjxk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2omutykhr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhanerqj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbshamos.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxtzxvz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fvxwagmd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vhpkjlnu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dmkodgof.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2txgibego.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fyeawtsr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2umrvzhrr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wtxdkusw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kxykqlzr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vmitkuqx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pwerzwrm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyieegjj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gddimdcv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tuhhqasm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kagneevh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zothskvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2llalzvlu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2enkcsvau.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tfhgroyx.html


<!-- 参考信息 -->