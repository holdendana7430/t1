代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtvlgcsgic.html

Java: x instanceof Number
来源：http://hz.yanxiufei.cn/gtarskouva.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ydzc1.top/gtosrwlisz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dianchejie.cn/gtbflbcixm.html

C#:   x is int or double or decimal
来源：http://hz.nanxuanxn.top/gtvodzcpva.html

[B14] 判断值是否在集合内
来源：http://hz.9152youxi.cn/gtpedctfne.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dashuyun.cn/gtucmyzlpo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xziqi.cn/gtcmesfshh.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gzhubu.top/gtuejoisun.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtmhxauuel.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cqqwz.cn/gttbussqvn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.feifeiyinyue.top/gtvoxpxoyn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuanzx.com/gtfvhhuzjz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.havefunace.top/gtpxdhzzyu.html

[B15] 布尔运算与取反
来源：http://hz.shuidangran.top/gtkrjvctka.html

Py:   a and b or not c
来源：http://hz.bjfxy.top/gtqbrvqizi.html

PHP:  $a && $b || !$c
来源：http://hz.yanxiufei.cn/gtnyfzqmtd.html

JS:   a && b || !c
来源：http://hz.zhongyouzk.top/gtczkrunqm.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gthxucogeb.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gtmbgjcjcs.html

Go:   a && b || !c
来源：http://hz.zhijiandao.cn/gtduurhlgd.html

Ruby: a && b || !c
来源：http://hz.ivvv.top/gtwveshltx.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtfjniprbw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tanke756.top/gtegajtzwp.html

Py:   if not data: return
来源：http://hz.xingfuxueyuan.xyz/gtmbvnetng.html

PHP:  if (!$data) { return; }
来源：http://hz.dianchejie.cn/gtgmzlvbae.html

JS:   if (!data) return;
来源：http://hz.cucudq.cn/gtoxhztske.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gtfcavpypd.html

Java: if (data == null) return;
来源：http://hz.guowangkeji.top/gtxnibobzi.html

Go:   if data == nil { return }
来源：http://hz.zhongyouzk.top/gtkdusapfu.html

Ruby: return if data.nil?
来源：http://hz.jlsjyb.cn/gtbugkssiv.html

C#:   if (data == null) return;
来源：http://hz.tanke756.top/gtbqgonruf.html

================================================================================
来源：http://hz.daxiang520.top/gtmrcvhcne.html

C. 函数与作用域
来源：http://hz.nanxuanxn.top/gtvmvkwtlp.html

================================================================================
来源：http://hz.sxryk.cn/gtsfxgsqnd.html

[C01] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtigqkkoij.html

Py:   def add(a, b): return a + b
来源：http://hz.sysykeji.top/gtphmsaups.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtelgabzmo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhixingplan.top/gtflaauhkf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtidptvqeg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtqpgstjvz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtroxdfapx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhiwuduotai.top/gtwewqupbz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtnghqaquv.html

[C02] 默认参数
来源：http://hz.mhx1999.top/gtffiuevco.html

Py:   def greet(name="World"): return name
来源：http://hz.smart0.xyz/gtfyriizgk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xuetiantiany.cn/gtojsmvfvb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258.top/gtffethsdk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gtlzhyxsda.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtvbwzqlgp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gthlmuobcz.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtqdiuxmxy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.daria6918.cn/gtksrlfgaq.html

[C03] 可变参数
来源：http://hz.hfpthk.cn/gtppsmcmex.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtajfwmptz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.meibo888.top/gtpmqfbiic.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtzlykggln.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtwgbnlwdt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yvedp.cn/gtylgjacxf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtzckxymft.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guowangkeji.top/gtfivgdayj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtomqdzqhu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.chenjidiqi.icu/gtxqaykrmr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.mhx1999.top/gtzyagjblk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xziqi.cn/gtqogarftc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gtioxbgxbi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.snrcjt.cn/gtocqnvlhx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinghuilouyu.cn/gtxzssevbv.html

Go:   // 无：用配置结构体参数
来源：http://hz.xylfe.cn/gtazyvtvki.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtvjnsihes.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtmkofajxe.html

[C05] 返回多个值
来源：http://hz.hnqzz.top/gttphvtjck.html

Py:   return a, b
来源：http://hz.zhengqikj.top/gtrvsclmco.html

PHP:  return [$a, $b];
来源：http://hz.nwbrower.top/gtixqslhxb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinghuilouyu.cn/gtskfsfhvp.html

TS:   return { a, b };
来源：http://hz.zycfv.cn/gtgkcmsreu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dianchejie.cn/gtwowdnnyw.html

Go:   return a, b
来源：http://hz.yuanzhike.top/gtwgoacgyj.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtqnavvmzd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zycfv.cn/gtvvnhzfzu.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangtech.top/gtehmastuy.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangtech.top/gtvkfriqwz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhongyouzk.top/gtejtbcfci.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtesndjuvt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.birdmap.top/gtjxtzcrvp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gticfxyrbh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gtucclxlns.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtotrzwizu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nwbrower.top/gtyyfonatp.html

[C07] 把函数作为参数传入
来源：http://hz.havefunace.top/gtschqikxh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtwjcpxiqc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtkjtjmgam.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shangyingyoupin.top/gtjtkspdxp.html

TS:   arr.map(String)
来源：http://hz.0kj1m.cn/gtatlueajr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ywan-chungtsiang.top/gtlnkdfpho.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtheltjizp.html

Ruby: arr.map(&:upcase)
来源：http://hz.9152youxi.cn/gthikrfuhl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gaohongyu789.top/gtsnxfoycv.html

[C08] 闭包
来源：http://hz.jinqigufen.top/gtlbhexxlb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sweek.top/gtntchjvcl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtgfdcoeey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtndhmixar.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtywnaxjmh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ehwqpu.com/gttjgoxhpa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.meibo888.top/gtrxewayta.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gthajsotvv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtvvoudzfv.html

[C09] 递归
来源：http://hz.zhongyouzk.top/gtxrmpsscs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.havefunace.top/gteirncrib.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sweek.top/gtmgvnnsuw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtonyqpatp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gttunezksi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.smart0.xyz/gtpiweasge.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtmwrnoyfw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aizwys.cn/gtjofqurrm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtwbwtxzkd.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtibkolaiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pengpengdd.cyou/gtzkbppsay.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtfoxwaozu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.redwolf501.top/gtzijgekzr.html

TS:   同 JS
来源：http://hz.chenzaomai.com/gttvvqifrz.html

Java: 方法内为块级作用域
来源：http://hz.xinyue.icu/gtqqlafcbl.html

Go:   花括号块级作用域
来源：http://hz.jiagoushi.top/gtidaoxzfr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tian-w.cn/gtbejoxvpr.html

C#:   块级作用域
来源：http://hz.dashuyun.cn/gtvgmwczsr.html

[C11] 模块导入与导出
来源：http://hz.jinqigufen.top/gtcftjhzkw.html

Py:   from module import func
来源：http://hz.aizwys.cn/gtkshwerhh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigufen.top/gtxbolgcsw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtdzczefot.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yonumen.top/gtjsxwhlus.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtqkpiqwzn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sufxvd.cn/gtgkaqqczm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sufxvd.cn/gtguvlcrdz.html

C#:   using System.Text;
来源：http://hz.xuetiantiany.cn/gtymjxtrjs.html

[C12] 立即执行函数 IIFE
来源：http://hz.svipenyu.cn/gtitbbrgkp.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtfyztrjbs.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtfzkahhhv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtclgsjpqc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtzvihvunl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gtkxerwniu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nwbrower.top/gtpcbqlidf.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhongyouzk.top/gtafsfzcxk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.wangshuangyany.cn/gtrhmkhgme.html

[C13] 类型声明 / 类型注解
来源：http://hz.andypj.xyz/gtyyanbary.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtrnogkrlm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gttqgstrlc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.iojbl.cn/gtcvvkwnxf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtkkkvxxti.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtssiqiuux.html

Go:   func add(a, b int) int
来源：http://hz.tian-w.cn/gtlagffnst.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jianghu66.top/gtmcgytlaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtvytqranq.html

[C14] 泛型函数
来源：http://hz.wangshuangyany.cn/gtswyerzra.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xingfuxueyuan.xyz/gtlzhppirk.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtvmbxjang.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtspkziyxz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtxidehnjy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gtwcefefwe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.vqdsnc.cn/gthuaalxbk.html

Ruby: # 无泛型
来源：http://hz.jinghuilouyu.cn/gtkchpdldb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.0kj1m.cn/gtvltkjtqj.html

[C15] 解构 / 展开参数
来源：http://hz.nanxinkj.top/gtlyoyijpe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhoulong.xyz/gtxiznawnc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gtlhsywawi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtwxoabszo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gtqiacsvbi.html

Java: // 无解构
来源：http://hz.c1oappe.top/gtdoxuwmfo.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtbruezurs.html

Ruby: a, b = pair
来源：http://hz.jinghuilouyu.cn/gtjpdyuypo.html

C#:   var (a, b) = pair;
来源：http://hz.jianghu66.top/gtlqfeulxk.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtpauzrtbq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gtgpvcitvi.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gtlqswctoc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.c1oappe.top/gtslmgparn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtiskrhzul.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhengqikj.top/gtnoscmjgh.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtpautubyv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtooswdzdt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinyuanbaomall.cn/gtijgcjkgl.html

================================================================================
来源：http://hz.cashguo.top/gtpwrdvjbe.html

D. 数组 / 列表 / 集合
来源：http://hz.dianchejie.cn/gtlrbvcedd.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuubwykcu.html

[D01] 创建数组 / 列表
来源：http://hz.dashuyun.cn/gtvhrhmfuj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yvedp.cn/gtjvhphaie.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fzhhl.top/gtgrqpwloa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenzaomai.com/gtlzkgronh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhixingplan.top/gtsbabdyfs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtiutlvkkk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aizwys.cn/gttnwxcmmv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtjqantbfe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sxryk.cn/gtkvdqkneb.html

[D02] 追加元素到末尾
来源：http://hz.bjfxy.top/gtnjsogxno.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jiagoushi.top/gtccpxbwgz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cqqwz.cn/gtiznhbmjx.html

JS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtmoybnysu.html

TS:   arr.push(4);
来源：http://hz.sweek.top/gtmmfkjgls.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtcjojjkql.html

Go:   arr = append(arr, 4)
来源：http://hz.hnqzz.top/gtqjxwmegr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jlsjyb.cn/gtvgrrzmqf.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtwbfvxkvu.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtvbtlrmie.html

Py:   arr.insert(0, 0)
来源：http://hz.shzxlz.cn/gtugqtljse.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenlongwang.top/gteaqpjzvf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ybcxt.top/gtuxesumxl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtlajivjdk.html

Java: list.add(0, 0);
来源：http://hz.chenlongwang.top/gtcscpnyxs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ywan-chungtsiang.top/gtoxfxllrp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hongshengwenyu.top/gtanxwoadf.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gttccteefe.html

[D04] 删除元素
来源：http://hz.jinqigfzy.top/gtwzzhpxtp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.feifeiyinyue.top/gtihsvmlgd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtpdppdoap.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gtkjealozg.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtiqwsjxku.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.9152youxi.cn/gtepuzsioy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtzkcuanhf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gthcljdekk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhengqikj.top/gtmmhdwnvf.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtpiqmwowp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtqzpzqmzn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtirbucxpq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gtirfkncrv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtbkafzdjd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtclkbfcwp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zycfv.cn/gthvaaujvl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtfhzroepp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtzybmjkff.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtpdbfgicn.html

Py:   len(arr)
来源：http://hz.sxryk.cn/gtwtfhhlpf.html

PHP:  count($arr);
来源：http://hz.cashguo.top/gtxfpcarbh.html

JS:   arr.length
来源：http://hz.cashguo.top/gtvbcrkuag.html

TS:   arr.length
来源：http://hz.zhongyouzk.top/gtqafmwrfw.html

Java: list.size();
来源：http://hz.xingfuxueyuan.xyz/gthageoheh.html

Go:   len(arr)
来源：http://hz.jlsjyb.cn/gtokmyofbe.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gtemqriarw.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtsaxeycvk.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtavqwyuyn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tianlin.xyz/gtmpghzkhb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.feifeiyinyue.top/gtyifijbdr.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtqpsodzin.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtfwuvgdlx.html

Java: list.subList(1, 4);
来源：http://hz.aizwys.cn/gtoaojimvw.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gtkwkspehs.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtzfrwmyvq.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtvgbmbziq.html

[D08] 合并两个数组
来源：http://hz.quarkkingdee.top/gtdpaoocog.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtqcyglzrb.html

PHP:  array_merge($a, $b);
来源：http://hz.quarkkingdee.top/gtghxinhrf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuxming.cn/gtferkgqed.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtrxacesnx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sysykeji.top/gtnihzaztz.html

Go:   append(a, b...)
来源：http://hz.shuidangran.top/gtwagfkwco.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtfvqappxm.html

C#:   a.Concat(b).ToList()
来源：http://hz.gaohongyu789.top/gtjlwzmiqy.html

[D09] 排序（升序）
来源：http://hz.zhaomingkeji.xyz/gttajychxi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuxming.cn/gtzhzphjmw.html

PHP:  sort($arr);
来源：http://hz.aibaodan.cn/gtifxitoed.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinqigfzy.top/gtkthmgyqx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zycfv.cn/gthzwpquwd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tianlin.xyz/gtfgelaqon.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sysykeji.top/gtuydskppf.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtziokhkfx.html

C#:   list.Sort();
来源：http://hz.yueranfly.top/gtzvwnxbqh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fengsongda.top/gtjhnmcrsr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuetiantiany.cn/gtadkqzfqm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtqodeomva.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtfpzwljep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtlkqcfxsh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnxiangtu.top/gtsxpxdgik.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xziqi.cn/gtanavmwqp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.meibo888.top/gtglfhyquw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtzrynfamr.html

[D11] 反转数组
来源：http://hz.zhengqikj.top/gtrmmgdijj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jlsjyb.cn/gtnolgyljs.html

PHP:  array_reverse($arr);
来源：http://hz.iojbl.cn/gtttfqiepw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuetiantiany.cn/gtsamfjppz.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtcqfgxtxj.html

Java: Collections.reverse(list);
来源：http://hz.xuetiantiany.cn/gtamxaagzv.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gtqsjgwvlg.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtvutpygxk.html

C#:   list.Reverse();
来源：http://hz.ehwqpu.com/gthjbdkivv.html

[D12] 查找元素下标
来源：http://hz.tian-w.cn/gtzhcsbwet.html

Py:   arr.index(x);  x in arr
来源：http://hz.jianghu66.top/gtyghahnna.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.haohaochexian.top/gtklqtdebo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gthrooddtq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cheryme.top/gtcxnorkmo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guowangkeji.top/gtyzmamfqg.html

Go:   slices.Index(arr, x)
来源：http://hz.haohaochexian.top/gtfjqgyzkd.html

Ruby: arr.index(x)
来源：http://hz.havefunace.top/gtikefmrih.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtkruplsnm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.bjfxy.top/gtwkohomwp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258.top/gtkezhjtow.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cqqwz.cn/gtltdutmal.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtlymehsyx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtskerivag.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cqqwz.cn/gtnccpnoih.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.kuanghao11.cn/gtwlkymkia.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtvrwcpvln.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gtafvqduoy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hammf.cn/gtienszwyt.html


<!-- 参考信息 -->