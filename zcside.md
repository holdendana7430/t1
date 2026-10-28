代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtfdyezcup.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhoulong.xyz/gtlpryukya.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jyoumei.cn/gtkjqctedk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhijiandao.cn/gtgnefwzdc.html

[B13] 判断是否为数字
来源：http://hz.jianghu66.top/gtkysbtcjb.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhijiandao.cn/gtwkseloak.html

PHP:  is_numeric($x)
来源：http://hz.xziqi.cn/gtbccmchnm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtlfgvlitc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtradbtbcb.html

Java: x instanceof Number
来源：http://hz.jinyuanbaomall.cn/gtxkyogudz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtacclidev.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jlsjyb.cn/gtifyehqfz.html

C#:   x is int or double or decimal
来源：http://hz.nanxinkj.top/gtlxvcauxj.html

[B14] 判断值是否在集合内
来源：http://hz.ppjwa.cn/gtafftkqhu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.iojbl.cn/gtunbsvklk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj202588.top/gtwlukijnm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ivvv.top/gtdhxblsws.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtnauagivm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gzhubu.top/gtkcpqqtuu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nwbrower.top/gtsdarmote.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuanzhike.top/gtouhgecfl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xziqi.cn/gtmquehzzj.html

[B15] 布尔运算与取反
来源：http://hz.jinqigufen.top/gtkwuxjsyd.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtlxpzmmdb.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtbagfpltw.html

JS:   a && b || !c
来源：http://hz.daxiang520.top/gtqaowshrr.html

TS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtnpzqoala.html

Java: a && b || !c
来源：http://hz.hongshengwenyu.top/gtviycjrau.html

Go:   a && b || !c
来源：http://hz.daxiang520.top/gtpuvwtaxv.html

Ruby: a && b || !c
来源：http://hz.tanke756.top/gtzdsnmecq.html

C#:   a && b || !c
来源：http://hz.zhoulong.xyz/gttzgarbel.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.bjfxy.top/gtgcjouhdv.html

Py:   if not data: return
来源：http://hz.sufxvd.cn/gtahqyagxk.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gtdudpavfc.html

JS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtlkosmebt.html

TS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtewphgvku.html

Java: if (data == null) return;
来源：http://hz.andypj.xyz/gttwgcnnfi.html

Go:   if data == nil { return }
来源：http://hz.zhoulong.xyz/gtiqkvsncf.html

Ruby: return if data.nil?
来源：http://hz.gzhubu.top/gtkkrbkosr.html

C#:   if (data == null) return;
来源：http://hz.ehwqpu.com/gtbkksfqkl.html

================================================================================
来源：http://hz.guowangkeji.top/gtgesfhgmy.html

C. 函数与作用域
来源：http://hz.cdnleiting.top/gtvcgmrpxp.html

================================================================================
来源：http://hz.shuidangran.top/gtpuoptxsr.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gteqbyikes.html

Py:   def add(a, b): return a + b
来源：http://hz.cdnleiting.top/gtxgfcmwyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtagvjljhk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tian-w.cn/gtuxvnlpms.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hongshengwenyu.top/gtlmrhvbkm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtwxjvggtk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.haohaochexian.top/gtoljpvnnp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ivvv.top/gtqggkdeed.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtwfmopwlx.html

[C02] 默认参数
来源：http://hz.ehwqpu.com/gtrdqdiknm.html

Py:   def greet(name="World"): return name
来源：http://hz.yueranfly.top/gtcapzbhru.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gtmdjwlkrd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pycfn.com/gtgxqzwkiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cucudq.cn/gthcgtuyvh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sxryk.cn/gthgcfusyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtopkbxbon.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gthidzcnws.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gaohongyu789.top/gttsdvnnxz.html

[C03] 可变参数
来源：http://hz.gotoacloud.top/gttfhwxdvt.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gtfqjegttf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hfpthk.cn/gtljannltt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtqkcmkynf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gttouvitks.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtewxggkyp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgufenzy.top/gtbjcvlwdq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yanxiufei.cn/gtnifisdcr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtxrvmbzoz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.9152youxi.cn/gtvmjrdusl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.316326.xyz/gtcblulzah.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zycfv.cn/gtxsoyeqpp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gttxqwnqaa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tianlin.xyz/gtnowkwjmm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gotoacloud.top/gtjuasaenu.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtgjuwzrrb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtlokbdysc.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtqkncupdi.html

[C05] 返回多个值
来源：http://hz.0kj1m.cn/gtbsddkbav.html

Py:   return a, b
来源：http://hz.mhx1999.top/gtpxtvjsqp.html

PHP:  return [$a, $b];
来源：http://hz.xylfe.cn/gttmffmuak.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhoulong.xyz/gtcpihnvqo.html

TS:   return { a, b };
来源：http://hz.wangshuangyany.cn/gtegpaunih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinqigfzy.top/gthnqckoci.html

Go:   return a, b
来源：http://hz.dashuyun.cn/gtpflkwnic.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtnjnphtkn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.c1oappe.top/gthiabpxqw.html

[C06] 匿名函数 / lambda
来源：http://hz.hongshengwenyu.top/gttvoazdkj.html

Py:   square = lambda x: x * x
来源：http://hz.zhaomingkeji.xyz/gthyudterq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtoduvkver.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtkopservu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yvedp.cn/gtafgoihrs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhengqikj.top/gtfgzpwiga.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tian-w.cn/gtdsgwttwi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtpopsmxzs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigfzy.top/gtnehicbiv.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtaadzqhiw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.316326.xyz/gtbdvarcjw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258.top/gthwhzkuex.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtvlevxrhy.html

TS:   arr.map(String)
来源：http://hz.jinghuilouyu.cn/gtxzqxffrb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtsgisapod.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuxming.cn/gthehzwgky.html

Ruby: arr.map(&:upcase)
来源：http://hz.sufxvd.cn/gtoubgkzbd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtdmrsdjty.html

[C08] 闭包
来源：http://hz.meibo888.top/gtcmkwwnvm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aizwys.cn/gtcmqssber.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aibaodan.cn/gtxqfzusyo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtyanhzinh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gthnptyfbg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gtznkaazok.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinyuanbaomall.cn/gtesqdyjwd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtnjureoih.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtesomtgyw.html

[C09] 递归
来源：http://hz.ivvv.top/gtblhwmwzh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtopspwuha.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ppjwa.cn/gtkbajpmlj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtasbdekvl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtiyyrteuw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtutckkara.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnqzz.top/gtmutcntzq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtrrkwlbtd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtjnmwzzgh.html

[C10] 变量作用域
来源：http://hz.ywan-chungtsiang.top/gtqwsxtmzg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxuanxn.top/gtmntxhyto.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gttbcgpisp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cashguo.top/gtnqsucjbe.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtsiymilje.html

Java: 方法内为块级作用域
来源：http://hz.jyoumei.cn/gtfuqqtsnc.html

Go:   花括号块级作用域
来源：http://hz.nwbrower.top/gtcicvdutw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cheryme.top/gtrkvksnmc.html

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtkfikputc.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gttftieznt.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtljjudmbj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gtetsjeobq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ppjwa.cn/gtphtisyvw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sufxvd.cn/gtznxqnhwi.html

Java: import java.util.List;
来源：http://hz.ywan-chungtsiang.top/gtlqrmocco.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj202588.top/gtmklfxroe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj202588.top/gtcygjxvgv.html

C#:   using System.Text;
来源：http://hz.fengsongda.top/gtuwnyjado.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhongyouzk.top/gtdffpnnbp.html

Py:   (lambda: print("run"))()
来源：http://hz.cucudq.cn/gthcxizakg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtdkxikbbj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtkibjyrgo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtmpdwacsa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gtwsslcgob.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenzaomai.com/gtikihztak.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gtgspodqni.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtduuorwpr.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtdmskfcov.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pycfn.com/gtewvgsbyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtzuekdbrl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtapolkpxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtfonhmsck.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtbjcuzxiw.html

Go:   func add(a, b int) int
来源：http://hz.wangshuangyany.cn/gtczxykinv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gogol.net.cn/gtpdhqdpev.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtlrdamvct.html

[C14] 泛型函数
来源：http://hz.yj20258.top/gtlzpmuqme.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuxming.cn/gthbdpknko.html

PHP:  // 无泛型
来源：http://hz.c1oappe.top/gtmjjjgemp.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtosossqju.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtfpilofmz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuetiantiany.cn/gtoeukazqi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gthcyxbwfc.html

Ruby: # 无泛型
来源：http://hz.dashuyun.cn/gtxdumnnro.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guannengcc.top/gtpsxskzuy.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtfbkfcyfo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.havefunace.top/gtmtmwsnvf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtnefyoukx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtknxtzmty.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtpdisrfua.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gtdpqzqmui.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtekcohnft.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtmwkrmdba.html

C#:   var (a, b) = pair;
来源：http://hz.zhoulong.xyz/gtrojyzibb.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtlqxgfwtp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ydzc1.top/gtfdpembcv.html

PHP:  // 无重载
来源：http://hz.52xcode.cn/gtegzooqip.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gaohongyu789.top/gtdbpmpqxn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sxryk.cn/gtijxzpbbq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxinkj.top/gtgquqjsfk.html

Go:   // 无重载：用不同函数名
来源：http://hz.quarkkingdee.top/gtrfzcthic.html

Ruby: # 无重载：靠动态参数
来源：http://hz.9152youxi.cn/gtoggkadak.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtmqynpogk.html

================================================================================
来源：http://hz.redwolf501.top/gtuepjykip.html

D. 数组 / 列表 / 集合
来源：http://hz.gogol.net.cn/gtkfhaymkh.html

================================================================================
来源：http://hz.xylfe.cn/gtzfvhbfvw.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtgwyqxnqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtzsvjfqcs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tianlin.xyz/gtihplrbmp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gtbmubgbbw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dianchejie.cn/gtqxjzkwro.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.svipenyu.cn/gtmapcmcuf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gzhubu.top/gtxdhfohbi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hammf.cn/gtdctvoqxh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtofqmppdz.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtrxcnqhfj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gaohongyu789.top/gtktpdnpfj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hongshengwenyu.top/gtafsfvgiu.html

JS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtofnnirwa.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtyhqwppok.html

Java: list.add(4);
来源：http://hz.cheryme.top/gtxzrcqihb.html

Go:   arr = append(arr, 4)
来源：http://hz.shuidangran.top/gtnxzuhsbh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sweek.top/gtzoaqnkiv.html

C#:   list.Add(4);
来源：http://hz.zhaomingkeji.xyz/gtlmalxgug.html

[D03] 在指定位置插入元素
来源：http://hz.guowangkeji.top/gtarxdcxzc.html

Py:   arr.insert(0, 0)
来源：http://hz.smart0.xyz/gtkvdhqwkh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtzkzkkbzf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dianchejie.cn/gtsxxtwuav.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gteqddlqoz.html

Java: list.add(0, 0);
来源：http://hz.zhijiandao.cn/gtiffgigmr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtkwsjuxyv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtdewpvmgq.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtcxhbxfgq.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gtdyiqyycw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtkpptcxzv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daria6918.cn/gtwuzijbxh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shuidangran.top/gthvnbsoft.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtunglxelv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtarthkvjr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtevjudbix.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tanke756.top/gtcyghrjdf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tianlin.xyz/gtrzgdxwjl.html

[D05] 访问与修改元素
来源：http://hz.yongpay.top/gtblypnfms.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtpucgeakh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yangfankeji.com/gtjaybvjfj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gogol.net.cn/gtuimwopee.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hfpthk.cn/gtueiwxref.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtqosroffg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtpztzxdjl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtpxdxqmxl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.quarkkingdee.top/gtfzzujckv.html

[D06] 数组长度
来源：http://hz.yonumen.top/gtxxotdhkn.html

Py:   len(arr)
来源：http://hz.smart0.xyz/gtfrrftakr.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gtmdfzawen.html

JS:   arr.length
来源：http://hz.quarkkingdee.top/gtemwdirwz.html

TS:   arr.length
来源：http://hz.hfpthk.cn/gtoahvsicn.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtkigyugdg.html

Go:   len(arr)
来源：http://hz.vqdsnc.cn/gtubqyoxsc.html

Ruby: arr.length; arr.size
来源：http://hz.jyoumei.cn/gtychysivw.html

C#:   list.Count;
来源：http://hz.quarkkingdee.top/gtilklbibw.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtwunhnlif.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cucudq.cn/gtmrkfeivm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jyoumei.cn/gtxdonstjj.html

JS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtqkrksood.html

TS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtkfqinuwa.html

Java: list.subList(1, 4);
来源：http://hz.hysaishi.cn/gtjcqbacox.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gttgyvcwte.html

Ruby: arr[1, 3]
来源：http://hz.dashuyun.cn/gtgojqqoxt.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhoulong.xyz/gtvqpwwoop.html

[D08] 合并两个数组
来源：http://hz.hfpthk.cn/gthetbjrel.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhijiandao.cn/gtbzjspfig.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gttgtawctp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yangfankeji.com/gtvknqgrje.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gtnpxhfkxt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fengsongda.top/gtsnddnwpv.html

Go:   append(a, b...)
来源：http://hz.chenzaomai.com/gtqozaeqld.html

Ruby: a + b;  a.concat(b)
来源：http://hz.316326.xyz/gtyfpocbag.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhixingplan.top/gtahvzoyjq.html

[D09] 排序（升序）
来源：http://hz.daxiang520.top/gtaaaiyymm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtlztirdka.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtihmvcbav.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtllhyudle.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gtqopxauff.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gthymqnhlz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtuherjyxp.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtyfpogimf.html

C#:   list.Sort();
来源：http://hz.zdqjudy.top/gtkyobrhvu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtakavuvin.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cashguo.top/gtqgxhgmph.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtdqdelajr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtuffmbkrj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtyrughthi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigfzy.top/gtfkscvwuu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinghuilouyu.cn/gtdbzfwfak.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.redwolf501.top/gtnohiktqg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtfjulfxzr.html

[D11] 反转数组
来源：http://hz.jqgufenzy.top/gtzdokjazx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cdnleiting.top/gtgjbzmhzy.html

PHP:  array_reverse($arr);
来源：http://hz.ybcxt.top/gtrduuvops.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhijiandao.cn/gtsjfcaxrp.html

TS:   [...arr].reverse();
来源：http://hz.guannengcc.top/gtnxktpqeb.html

Java: Collections.reverse(list);
来源：http://hz.yanxiufei.cn/gtvxmiboii.html

Go:   slices.Reverse(arr)
来源：http://hz.ybcxt.top/gtwusktyjs.html

Ruby: arr.reverse
来源：http://hz.zhaomingkeji.xyz/gtyiitvakb.html

C#:   list.Reverse();
来源：http://hz.tanke756.top/gtstqsazdd.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gtbcqsboaz.html

Py:   arr.index(x);  x in arr
来源：http://hz.ybcxt.top/gtplrkwmeg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtynfnvqwv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtduxpphzd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtlfibexiw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gtcfugxhkr.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258.top/gtqcrohoso.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtqdwwghak.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtivxdelmi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shanyushiyangkeji.top/gtoznppley.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtozfgfdju.html


<!-- 参考信息 -->