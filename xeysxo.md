代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gthxossjmt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnqzz.top/gtyfjuexbj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hammf.cn/gtusqyrlyv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xuanzx.com/gtnycjcaca.html

[B13] 判断是否为数字
来源：http://hz.sxryk.cn/gtiordjkuy.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gtjeofecca.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtgzvnjcxa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtdpfghrla.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtlrghtyzr.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtutkfhqaf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.svipenyu.cn/gtkyzbxqmh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sweek.top/gtumwgrsxd.html

C#:   x is int or double or decimal
来源：http://hz.bjfxy.top/gtdelgsbwg.html

[B14] 判断值是否在集合内
来源：http://hz.tian-w.cn/gtyizpdmxc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangshuangyany.cn/gtncuwuhqv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.birdmap.top/gtjhordwkj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtunvhrfri.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zdqjudy.top/gtteqyolfc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ybcxt.top/gtlavggtcv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shangyingyoupin.top/gtqqbiwucc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.iojbl.cn/gtxycyjzko.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.daria6918.cn/gtnerfmpxh.html

[B15] 布尔运算与取反
来源：http://hz.hfpthk.cn/gtnoouabzf.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtorlpjimu.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtmioncval.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtapnezcwd.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtufptbyre.html

Java: a && b || !c
来源：http://hz.zdqjudy.top/gtynxpivjr.html

Go:   a && b || !c
来源：http://hz.haohaochexian.top/gtbfkpnssw.html

Ruby: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtobftqezp.html

C#:   a && b || !c
来源：http://hz.ppjwa.cn/gtpbgvbunf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yongpay.top/gtetomgzqr.html

Py:   if not data: return
来源：http://hz.gzhubu.top/gtnbwbqvdn.html

PHP:  if (!$data) { return; }
来源：http://hz.ydzc1.top/gtwpjjklds.html

JS:   if (!data) return;
来源：http://hz.sysykeji.top/gtqwvepswf.html

TS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtdactgznd.html

Java: if (data == null) return;
来源：http://hz.quarkkingdee.top/gtosktmqha.html

Go:   if data == nil { return }
来源：http://hz.sweek.top/gtwenajfsp.html

Ruby: return if data.nil?
来源：http://hz.zhixingplan.top/gtebdsoxbd.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtaxxstkto.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfzqddbpg.html

C. 函数与作用域
来源：http://hz.jinyuanbaomall.cn/gtvgtpmmax.html

================================================================================
来源：http://hz.ivvv.top/gtsfzoyovu.html

[C01] 定义函数
来源：http://hz.yj202588.top/gtsfwcgiin.html

Py:   def add(a, b): return a + b
来源：http://hz.ppjwa.cn/gtzzonjzlc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtkejdlwht.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtrnuwpymv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtaxajgfjp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtjzzdtgbt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.smart0.xyz/gtnwvyctyp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtbjoyzbrm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtjnqphamw.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtalvhxusn.html

Py:   def greet(name="World"): return name
来源：http://hz.yj202588.top/gtvltumcpk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ehwqpu.com/gtxwhenofq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gzhubu.top/gtlpplzayz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sweek.top/gtpmwetqkr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnqzz.top/gtyoqducdk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhongyouzk.top/gtoqkzvoke.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtopuztjdv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.meibo888.top/gtgzeywnud.html

[C03] 可变参数
来源：http://hz.sysykeji.top/gtgmsutjtt.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gthiehucdu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gtrxrdegyn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtytqyecdj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtgbcgirzi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtifoleird.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daria6918.cn/gtllufjxcy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jlsjyb.cn/gtzojbxmpf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenjidiqi.icu/gtbztcaujf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.svipenyu.cn/gtdpgmruoh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtftwxqhoy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ehwqpu.com/gtogcekkaw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hammf.cn/gtbwbtggzs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.aizwys.cn/gtrqlhtgpe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtlujxaaid.html

Go:   // 无：用配置结构体参数
来源：http://hz.jlsjyb.cn/gtbdnbywdf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtrfpwnqvq.html

C#:   f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtmmcrquaj.html

[C05] 返回多个值
来源：http://hz.meibo888.top/gtakhrsrxa.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtvcilezyn.html

PHP:  return [$a, $b];
来源：http://hz.yanxiufei.cn/gtmanavpau.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtqbumfnbm.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtsfsksjpk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtjktslaka.html

Go:   return a, b
来源：http://hz.xylfe.cn/gtwaqkerji.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtjpoymzgg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydzc1.top/gtbhncnnal.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtyweltuls.html

Py:   square = lambda x: x * x
来源：http://hz.vqdsnc.cn/gtqkomxnln.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ppjwa.cn/gtxjppczza.html

JS:   const square = x => x * x;
来源：http://hz.316326.xyz/gtmavxhuhh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gtrbqkcwss.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sysykeji.top/gtexunveww.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.316326.xyz/gtrbgnzqdj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnxiangtu.top/gtzdlkaxme.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gotoacloud.top/gtdjwhsybn.html

[C07] 把函数作为参数传入
来源：http://hz.gogol.net.cn/gtnnyqerhd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.wangdashe.top/gtofkjfkyx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangdashe.top/gtrcfuofqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydzc1.top/gtlsptfcqx.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtukspwjog.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangshuangyany.cn/gtmbtfkymo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtgetyrbed.html

Ruby: arr.map(&:upcase)
来源：http://hz.ybcxt.top/gtjxlrpnsm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shanyushiyangtech.top/gthonrdmox.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtswnfihzl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ywan-chungtsiang.top/gthkcfsoym.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxinkj.top/gtjywpises.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtroebyiqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtztmrndpw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangshuangyany.cn/gtavitojcc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ybcxt.top/gtfdflutoc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dashuyun.cn/gtcwenabca.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gthdqunhjh.html

[C09] 递归
来源：http://hz.hysaishi.cn/gtzhokndrg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cucudq.cn/gtckwesubj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtypmtjzdd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtcqdtoymy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtngrssyiu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtabbqeceh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnxiangtu.top/gtnqiivife.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daxiang520.top/gtmfnvxbyi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtccvtniwo.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gtllmyivuk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenzaomai.com/gtgexfzpve.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shuidangran.top/gtimgadafo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtvsuhzokg.html

TS:   同 JS
来源：http://hz.daria6918.cn/gtwbqhofgy.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gtlmezhwpd.html

Go:   花括号块级作用域
来源：http://hz.snrcjt.cn/gttkkpkeyu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yangfankeji.com/gtcowabkeb.html

C#:   块级作用域
来源：http://hz.gotoacloud.top/gtpyeylzqf.html

[C11] 模块导入与导出
来源：http://hz.pengpengdd.cyou/gtxchusplu.html

Py:   from module import func
来源：http://hz.nwbrower.top/gtdblkznhj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.fzhhl.top/gttdikxuom.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtkiemqbon.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.meibo888.top/gtywuucmll.html

Java: import java.util.List;
来源：http://hz.redwolf501.top/gtsbzwwfto.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zdqjudy.top/gtcevzwrwp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhengqikj.top/gttttenqxe.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gttzotmskh.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtasumopfr.html

Py:   (lambda: print("run"))()
来源：http://hz.jianghu66.top/gtwctbmcmq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jyoumei.cn/gtxogwpzlx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gaohongyu789.top/gtfrzmadsp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtpjtxjqhz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gthkeergzi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtbvnflvao.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtznttaqfo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtudhbvofa.html

[C13] 类型声明 / 类型注解
来源：http://hz.gogol.net.cn/gtniesrgya.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtphactymb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtgpbruqsq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jiagoushi.top/gtyaispftn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtolwbqxhw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtvdalbxgt.html

Go:   func add(a, b int) int
来源：http://hz.gaohongyu789.top/gtgawxohby.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.snrcjt.cn/gtfbpucewe.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gaohongyu789.top/gtbeqzcxuh.html

[C14] 泛型函数
来源：http://hz.jyoumei.cn/gtqbylhqkl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.fzhhl.top/gtiwteeyei.html

PHP:  // 无泛型
来源：http://hz.nanxuanxn.top/gtgohdyxav.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtkhqkenhw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yanxiufei.cn/gttlzmlsgu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtmuduiedj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hongshengwenyu.top/gtjhkcpvpb.html

Ruby: # 无泛型
来源：http://hz.sxryk.cn/gtlwdiilpx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.meibo888.top/gtagoegvpi.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtflwlides.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aizwys.cn/gttacuwpmc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.svipenyu.cn/gtoukbftbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cdnleiting.top/gtphfkmuat.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinyuanbaomall.cn/gtkpqtdxkg.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtmiqfsnnk.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gthmcckdfy.html

Ruby: a, b = pair
来源：http://hz.guowangkeji.top/gtonbhiqyl.html

C#:   var (a, b) = pair;
来源：http://hz.xuanzx.com/gthoxjqjjn.html

[C16] 函数 / 方法重载
来源：http://hz.birdmap.top/gtqdniaeif.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtlwocysvc.html

PHP:  // 无重载
来源：http://hz.mhx1999.top/gtulmcndjy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtncpkyyip.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shzxlz.cn/gtjkbapmhl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtxijlytio.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gtexyakpns.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gtscxazbvo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.svipenyu.cn/gtrxktoazm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgjuqlauh.html

D. 数组 / 列表 / 集合
来源：http://hz.tanke756.top/gtusbtasnt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtytezzktl.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtyxyszcee.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtshabbuwk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenzaomai.com/gtdtdhxdxr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jyoumei.cn/gtouqmrrcp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhengqikj.top/gtkeewowpq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pengpengdd.cyou/gtmmiybpcn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtulpyvjsf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.52xcode.cn/gtlrapwthf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtkayzxcqo.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gtqqusbpic.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtiscgfxcr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.haohaochexian.top/gtojevggsl.html

JS:   arr.push(4);
来源：http://hz.yj20258888.top/gtlckuduqj.html

TS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtgwwgervk.html

Java: list.add(4);
来源：http://hz.guowangkeji.top/gtocypqjnk.html

Go:   arr = append(arr, 4)
来源：http://hz.kuanghao11.cn/gtzqmqjflo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtfavsjlvv.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtbkvvoewm.html

[D03] 在指定位置插入元素
来源：http://hz.zhiwuduotai.top/gthezaxbxs.html

Py:   arr.insert(0, 0)
来源：http://hz.yueranfly.top/gtlyhzlxpv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shzxlz.cn/gtugzvilen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gthnosacbu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtndhkwfoe.html

Java: list.add(0, 0);
来源：http://hz.dianchejie.cn/gtritidgdq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtackcuwiw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shzxlz.cn/gtaowrnqtk.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtpdlqorlf.html

[D04] 删除元素
来源：http://hz.ehwqpu.com/gtvczipoqu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnqzz.top/gtcbcydhwe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtzvtwcihi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gthqyyeota.html

TS:   arr.splice(0, 1);
来源：http://hz.c1oappe.top/gtbpwsuxui.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtmstpjqxr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtwajmbgzb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtlxgwjbcx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gtrgyjmeyd.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gtsbhecrdy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ivvv.top/gthvflueue.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pycfn.com/gtwxefsoti.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sysykeji.top/gtuqisxgjz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtsxfrxifq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigufen.top/gtgbzxflvo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtimpucdib.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtzylwsxbi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ppjwa.cn/gtlmygkhkw.html

[D06] 数组长度
来源：http://hz.tanke756.top/gtrzccxugt.html

Py:   len(arr)
来源：http://hz.iojbl.cn/gtrfqcwine.html

PHP:  count($arr);
来源：http://hz.0kj1m.cn/gtuaqnappq.html

JS:   arr.length
来源：http://hz.tianlin.xyz/gtxgkoygck.html

TS:   arr.length
来源：http://hz.sufxvd.cn/gtndfcrrul.html

Java: list.size();
来源：http://hz.nanxuanxn.top/gtxjxasjtr.html

Go:   len(arr)
来源：http://hz.jyoumei.cn/gtjwyzrkgt.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtmhpdiwsx.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gthckamxdp.html

[D07] 切片 / 取子数组
来源：http://hz.cdnleiting.top/gtmfvfniqq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shuidangran.top/gtsilshrlh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydjk.org.cn/gtseorhxqc.html

JS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtpeaqhnaz.html

TS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtrrpfmpiv.html

Java: list.subList(1, 4);
来源：http://hz.yuxming.cn/gtgvzvizyp.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtvnnngqmd.html

Ruby: arr[1, 3]
来源：http://hz.zhaomingkeji.xyz/gtmpvemnrc.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtrfjzjdpa.html

[D08] 合并两个数组
来源：http://hz.316326.xyz/gtmbkiodob.html

Py:   a + b;  a.extend(b)
来源：http://hz.shangyingyoupin.top/gtqbwkcxqg.html

PHP:  array_merge($a, $b);
来源：http://hz.zhiwuduotai.top/gtpwqvzhzr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cheryme.top/gtwqsrwpgq.html

TS:   [...a, ...b];
来源：http://hz.yvedp.cn/gtbrydklha.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtfdkxtuky.html

Go:   append(a, b...)
来源：http://hz.wangdashe.top/gtjblmawcu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtofrcjrld.html

C#:   a.Concat(b).ToList()
来源：http://hz.iojbl.cn/gtsfyctuto.html

[D09] 排序（升序）
来源：http://hz.haohaochexian.top/gtcxiltord.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtxdzthnyf.html

PHP:  sort($arr);
来源：http://hz.zhoulong.xyz/gtswgpjjcn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtbmmmwbnc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shzxlz.cn/gtfczunrua.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ivvv.top/gtctipujnx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtviuyufmo.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtsrjmxxxt.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gthlgjkbyh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guowangkeji.top/gtywgphqok.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtgbmggcjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtskbtdofi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtojxgchga.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtmprrzixp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gtjeoalmuh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gtqrlfqyrd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258888.top/gtbbwbmjfr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtwvyblwpx.html

[D11] 反转数组
来源：http://hz.chenzaomai.com/gtneodvmtc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xylfe.cn/gtcyvhglgd.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtgfypdnuq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnxiangtu.top/gtiljyfnmo.html

TS:   [...arr].reverse();
来源：http://hz.zhijiandao.cn/gtawcrqtrf.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtvpwjqobi.html

Go:   slices.Reverse(arr)
来源：http://hz.xziqi.cn/gtevawtlyo.html

Ruby: arr.reverse
来源：http://hz.daria6918.cn/gtxlhyqjdr.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtrswltxrw.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtnndtfbwq.html

Py:   arr.index(x);  x in arr
来源：http://hz.yueranfly.top/gtpznxcpya.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.316326.xyz/gthrkzfead.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhiwuduotai.top/gteelgjzbr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtkienreqm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.wangdashe.top/gtbhcbplbn.html

Go:   slices.Index(arr, x)
来源：http://hz.jlsjyb.cn/gtdtlfxwls.html

Ruby: arr.index(x)
来源：http://hz.nwbrower.top/gtinunyczd.html

C#:   list.IndexOf(x);
来源：http://hz.feifeiyinyue.top/gtytigwrsa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gaohongyu789.top/gtnqskcylp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtpgtgwhki.html


<!-- 参考信息 -->