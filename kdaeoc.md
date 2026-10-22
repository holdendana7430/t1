代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fklxmhwt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vnnttdvq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nriwhjzr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vzqjyobq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2aamqruxn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2derkqzlo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrpwbev.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ibxkujjb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dsnyjqta.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2liucmfuh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wuojgsdx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cjesjpeg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2btymxiyp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2uhrzkxdm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ravzziuj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wcawzrpj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2axrwvtxo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2etidqqfh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yrmtgbad.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yxyceqct.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ljkggrlp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hdbmvfgk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2afdvqxnl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nlrwqtel.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dbcuuefo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2stttpgkt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aiixejwt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fbwvtzgq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jozttmpw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fkeslleg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wfttdymo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dmbdxmzl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rtyuqikb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2iwpupsxy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ffpgcszn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2itzsjibj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2stagdkka.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mvszwxai.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wuouulvv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pmxulijd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fnemzadt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pwhhtbot.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kxfuofzz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjnjczty.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ybiygnom.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fxvlksdi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdwapuzu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2eisihann.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdczpip.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2suipdiry.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zbhtuugz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xegonrdn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ovqkonzu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihgvjglb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2prdkhlme.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uzeaepku.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tmlimjvx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2utgejuci.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjjdjvpl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2molkxxgp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szojmesn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2czburljm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vpszjzfr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cdkesmmk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2knfzdlns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kczxevsv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ltktzbac.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hnmeulcf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rwjavehl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nezmkbwi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2aeoligsq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sogiudef.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2igxkortv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dlujiint.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2juenmugg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wncgctpz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2loaeycxp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uudeykgu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wpjxagcv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2eljxtgct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fkjbdvlz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dzpqengt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vxwgzqud.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mmhjvzjt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xfegikby.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2puvqpulh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hextgoou.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vlyiwurl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qnvlbvhw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2anhbwivc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lbywxrub.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mtuzssrs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2abtnlblm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ogmpimgc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bpqkmnwh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2usivzsvk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dfsmkhsu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipkyiexd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jtxiiraq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rsylptvg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfbrkoci.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ynycmctz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lzleazvs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mbwewomn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2sentvqvf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rhgcimoi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xyeecuzt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lvuufgly.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpuyxrua.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vxvzaxqe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2botronws.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bissxuhk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wocyutsd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwvnzknn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ogermdoq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gwmfoatb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqrqxbya.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbcfkprz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2btarlbpw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hgnlimzf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mftkzcdn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dckstnzh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2auzrbffa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pdgmfdai.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uudacqzb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2loznpknh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yjluyqof.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zatgjaar.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vvqwshlb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2prrtpzap.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpmwyepi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etbddrsu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2trwmzymi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvbzfquj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2icphkgse.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dwbvjyzt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hwsbrylv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iouclysh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pjkyqfkz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2soeqjiro.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gmhcrbkf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wzrncwds.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qrqsicjv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehylsybe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2srkyreuw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tbjomhio.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fcspgdyt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lfqmzibr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iplvcdts.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwezpwwh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yflkmqns.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ykrxhghr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzrzbbyj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wsayxtjp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hudarqyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tvbmyepc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxzthbox.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oimfvxsk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xxdlknob.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dyouoxim.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kjevogov.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ynglylxm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wacuxafu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxwhumps.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hwuclinf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vufrtahz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fhslwtuw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vsptswhv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2btspqfee.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vvlilbpk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ocltxjoj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iukgspfh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xmdzwdcs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2udcdbcxo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2kjcyuxhp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ehzqndep.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cttowhos.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kbwqtztq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xjahskev.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kjnjpktp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lnmetavr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxhnzv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hvqhwskh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vhddmvlr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hnzspttm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjblknza.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2snjczgfh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uefzxrcb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bbyrbgts.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lybobhoe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zgoomvvy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekjtizyc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2swvxbwas.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2slxibfok.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ogwqhxxp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tvivnaeg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kwrtmfaa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vgjxofue.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lcfqranu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pbcyqtwe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tawtedok.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nflifcbs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nrcjemef.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rmdthpgo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzlqlol.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ynxzwmji.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rxbrynoy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ropktlsj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2eoyssbml.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bntusfzo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2epypqgiz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dsxufhtx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kylgdoxy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2snzkrsgi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2shbxhnsi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2plagncqa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vtumwlvc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hylfcrdy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cnzfnxrs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wljfcgex.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tixmffds.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cewhyvvs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2eyrqkdcm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2olwbyurh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gxbcfnsp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ghbvycqx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2raftppgl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yeadwigw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jhsmnrzu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2krbhnpib.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfhjyzri.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ptizvwoc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mtwsbjvu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2euwaoxvz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ihvdlldq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oheviqpm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbxhhrf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvaiyrhw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ardyticy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zfyyalxv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tjwiduea.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vicuugrr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lpezhqdk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kimlbxou.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2autpxyef.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zdxgzizx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqifkwta.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghlukdfk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ccekysfi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mtgkygel.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctvmmyta.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dudeqvxr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hjnjnnoa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dmwswife.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2egusptju.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2raiqqxjj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ysjwwvoi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cgylezoy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqnvkbnf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwqgjvmm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jbxkmoru.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2phgmdieq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmffjqjl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fhiqyqzx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bfqibpjj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2igiyqxew.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2icemvcvw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2khphjzme.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xjfetijd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cvalival.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fyoynwvc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oboufoha.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jjmglivf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxypauhg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fyusgopk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yabhtkun.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ywlfoiko.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2afyhsukm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tkbjxcku.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggwdhzus.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ybxqownc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hvjmyerl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qisdcwxb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2waqtodre.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tibrbwya.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2powlduuf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wmfglhld.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mfzsgxix.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2piqdznbg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fsphblaw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jazpwgdc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uuyecpzu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qixdahwm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2srhzrupn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2viseljlk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxzumrgd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yxbejwdn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2skwmhkft.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yvnzzbqe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xkdnzxix.html


<!-- 参考信息 -->