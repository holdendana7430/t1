代发 wailian999

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gwvrumwyf.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gauuntjdp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gpnjvtgad.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gbvzjqico.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gngmovhjx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/ghvsziftu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gjglgvksd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/grqldeemg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gnjkruzln.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gvyvmmmsa.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gdlguddlj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gxojndhcf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gvhgczsbc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gnuecgnkv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/ghjvqirad.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gsbfuxufn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxlnvzafl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gzmsgkvqe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gpoaqvqhy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gtpdugibx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gmkcghkeg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gemlylphq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxregxpyh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gqerivqug.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gbmaeqqax.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtdkbjgzq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gcetftmtl.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gnkogoypk.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gyapqwzjc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gxlwfejha.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/giqauhgkq.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gvmmtllko.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/ggkdwgtfg.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gbvawpxmz.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gwzzkrhwz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gywmhqvyo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/grjfuusty.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gueqkphjo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gmphiqpvh.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gvlserezx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gnlailiql.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/geoecntix.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gopkcburo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gmayketvm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/girxrzfyi.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/glefnfaiw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gnzzcicia.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ghdfpuyil.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gxiojwfqi.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gijxrkuse.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gskndcohn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gpknotenp.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gldjfunja.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/grdvoxmdl.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gzkfglahr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gkmpeleip.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gmxxwnnay.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gdxsineln.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqriswsyz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gjfltczqt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfiutpcq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/grulxgsuh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gzbiskcvt.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gmveuykrw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gicdjkhuq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvlpnqppo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gtbxvhzuo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gsnyebadh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gtknjjeui.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/ghzketcow.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gtvlcbqsj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gwxgmkuvq.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gdkfzswjd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gdqgcisxe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/goulqwwqt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/geserpzgt.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gwsunkzlp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbhppkdrp.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gllwsgrwh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gqggeovyi.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/givcbwpoh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/goizugxok.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gqqysvyxh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gygbblxut.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gnjssgwsp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/ghbnmvzag.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gecasrgph.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gyqwgctuk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gkzwiatyn.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gapsfxyal.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gnuhegaqf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gvaydvxit.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gpedtnzev.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gbfzpiefd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gfsckvkai.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/guhvlqccr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gngkfgbwt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gghttdpqf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggpkbkmag.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gejykrday.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gzcvzyjbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gsvjeuuji.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/ggtrbmwls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gsfeubolw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvdjsbbgt.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gebxmfvlv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gcwemnzcy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gjfxsnonn.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gnaltujkr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gifntectt.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gduzcrfao.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/giabuzlfh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/glrmrwcxh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gzhynyjkl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gqorrmoqo.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/givtctyxd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gciedhrmk.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/ggknfaeub.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gjdhndxib.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gxwpripui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/grabbvgxp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/ghcnrqbug.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/goycoegey.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gbjfspunp.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/ghytudwfk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/ghemnojmj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gbqksnmbw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gosdpxpbm.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gdxgtbyod.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/garxarbfb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gbpjsjiui.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gglylybki.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gtvflrazq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gajomsadm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gwrkszlqa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcxkvapit.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gxcnakuyo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcdwygiql.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdhjniroa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gliyukvvv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gftwjallj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gqqdtwzeo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gjwuizrfp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gybxogxek.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gqwubmzgh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gifvhvnlp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gxyxyqmvr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gojtfvdem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gwxhsivos.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gaqlkqpea.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gciqgexru.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gqhqnpivx.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsxdshmfm.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gdflfjmtm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gxgukkuio.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/guekpfrht.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gfuqezxgu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gyfixpqrw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gidqxcbat.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/guxkiukms.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gcqowunrp.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gtblwzgzo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gidjfmytn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gcbzerbzg.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gfmnjgfzt.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gjrafeapt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/ggwuwsrhi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfqvqnvjz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gktsjqbld.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gwtqpxnxd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/graqdxapj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gmsslqwoi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gvgnlatlk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsezlrvuy.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gekhtddhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwpzrdz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gljhllimd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grqqdakab.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gqkzjlklv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gqfhtekga.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnlrrqjty.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gecncwdkm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gxcceuczd.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gouuvcdhz.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grbcspkit.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvytrqvxd.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjykxeeby.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gbtqqlzfe.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/ghevumann.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjyvrge.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gcmgmsbqv.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gqrovaidf.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gjycofbvh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gluxlsqww.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gcdceiqcf.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gsbibzonk.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjlchaamt.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gvjasmgwf.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gvpunsaeu.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gxxsvrzwr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghjleanmm.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gomcjetbk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gnzshrcnh.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gkaajbsaf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/goetzhxjt.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/ggutonhuv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpvnewhud.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gcjmdpgzb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/grddfkadr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gaupqntuy.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gbiczcflz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/glcpklexr.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gjynvncxj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/giryfokzl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gqslaqohh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gynesqazf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/glytktmue.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gacqhrtgd.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gmqzihjew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gmxsdlrbp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gtfbovfnt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gbqklvjkl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gshrdwtgd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gmqjfuksv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gxtaqdphi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gkyqkifjk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gjaprulwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gdktgmint.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gxyhbtuby.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gtigebswf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gjhsgwhun.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/geqyxcrje.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gxzyqlrpu.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gxbgtqsiw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gqnpczuln.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gphohiovp.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gvljybbju.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gsifgziuc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gnyqluiyj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/giamhoxlq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/ggyogiwpu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gczuabwdi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gkgceuxdc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcjlfvnie.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gupyjodaq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gsmywsynx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/glfgrooyb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gxbducill.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaixyahuw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmmuoxdga.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ggxolctks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gbedwqqje.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gdbocsesj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/grufrwupi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gflxpyhjk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/giiksezrk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gwpbsvilh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpdbzktmr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gtjwzbszv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkmhwepdg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gnnpxexrv.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ghfrtphum.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gdazvdkko.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gddysvzbu.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gufunpmew.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gzfsvlutc.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gedyentyt.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gjqqwxqar.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gcvgqhtnt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/glwypixje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gzxadbcva.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gipwaavtw.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gkziaaszn.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gliadcksi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gyqnybfgl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gkwseijgo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gehuuzwlf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gkppgxqls.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gghrpcanm.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gciqdvwud.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gfbzhqies.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/guhrbolwa.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gwvlsmozn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gzzwsckun.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gbegdfraj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gdhfmwesy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gbczaotzi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/ggvihlcyd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guoxmelap.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gsttphbbz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/girpxwljw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gyapjnqeq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/glmqhwukw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/ggwbukmgv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gifiwsqmq.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gcqhfwaeo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/glybhwtln.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfwyxto.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/glgcauluk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gxeszrqgj.sHtML


<!-- 参考信息 -->