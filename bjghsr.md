代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuanzx.com/gtlzkjroaa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cdnleiting.top/gtvfgdetmm.html

[B15] 布尔运算与取反
来源：http://hz.zycfv.cn/gtihxgnhlh.html

Py:   a and b or not c
来源：http://hz.nwbrower.top/gtignqpuyu.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtbovvqqoo.html

JS:   a && b || !c
来源：http://hz.redwolf501.top/gtfpekxiow.html

TS:   a && b || !c
来源：http://hz.mhx1999.top/gtwozekiud.html

Java: a && b || !c
来源：http://hz.aizwys.cn/gttugyrvoj.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtyepenzwg.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtsjcjchkf.html

C#:   a && b || !c
来源：http://hz.zdqjudy.top/gtwkmmdnzn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangkeji.top/gtoylmkuxq.html

Py:   if not data: return
来源：http://hz.shangyingyoupin.top/gthnjzezak.html

PHP:  if (!$data) { return; }
来源：http://hz.yongpay.top/gtscjskkpd.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gteopqsvkc.html

TS:   if (!data) return;
来源：http://hz.zhoulong.xyz/gthgllplph.html

Java: if (data == null) return;
来源：http://hz.birdmap.top/gtapdxqzmd.html

Go:   if data == nil { return }
来源：http://hz.fzhhl.top/gtcesxewnt.html

Ruby: return if data.nil?
来源：http://hz.cucudq.cn/gthhrxbeti.html

C#:   if (data == null) return;
来源：http://hz.sxryk.cn/gtqlnxyrid.html

================================================================================
来源：http://hz.yj202588.top/gthttrbvdg.html

C. 函数与作用域
来源：http://hz.dashuyun.cn/gtihwexjzp.html

================================================================================
来源：http://hz.yuxming.cn/gtlopwzpho.html

[C01] 定义函数
来源：http://hz.svipenyu.cn/gteuqbsnae.html

Py:   def add(a, b): return a + b
来源：http://hz.yj202588.top/gtekzikllr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gteooqymsr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtozlypiqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtknhigfmv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gttcfvhatp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zdqjudy.top/gtupvsmjcx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgufenzy.top/gttaucmgbs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtqbzkhqzi.html

[C02] 默认参数
来源：http://hz.c1oappe.top/gtprfuyjbg.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtfcfadkvd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xinyue.icu/gtdsfwgzkz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.iojbl.cn/gthsndajxm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shzxlz.cn/gttqseejoo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhongyouzk.top/gtrhfyendr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinyuanbaomall.cn/gtzcpfasrp.html

Ruby: def greet(name = "World") = name
来源：http://hz.zycfv.cn/gtxsaumxgt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxinkj.top/gttpdwzeci.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gtmxjkrycr.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258888.top/gtuhiwqdmu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangdashe.top/gtqdgvrris.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhixingplan.top/gtzvmhynqx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtniqgyxyp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtlyhcnugz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jiagoushi.top/gtwaqikfvd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtwsppligo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sysykeji.top/gtgmmcjuuw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.mhx1999.top/gtfrgvxckt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.52xcode.cn/gtqlygtwlj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtilatwhpr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtmckinjwl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zdqjudy.top/gtepyrldss.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ehwqpu.com/gtjazbnewl.html

Go:   // 无：用配置结构体参数
来源：http://hz.ywan-chungtsiang.top/gtvhrhapiv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtsokmnglp.html

C#:   f(a: 1, b: 2)
来源：http://hz.xylfe.cn/gtmxtlpkmr.html

[C05] 返回多个值
来源：http://hz.ppjwa.cn/gtnmtmbvhm.html

Py:   return a, b
来源：http://hz.fengsongda.top/gthvcewxyv.html

PHP:  return [$a, $b];
来源：http://hz.wangdashe.top/gtsislgumm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yongpay.top/gtkvghzrcl.html

TS:   return { a, b };
来源：http://hz.hnqzz.top/gtbrkqrxqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhaomingkeji.xyz/gtxplenxmu.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtxmhrjizo.html

Ruby: return a, b
来源：http://hz.yj20258.top/gtdwvjzmqk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ppjwa.cn/gtqdfnabvt.html

[C06] 匿名函数 / lambda
来源：http://hz.hongshengwenyu.top/gtsgdnfshq.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtqyzccwbx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shuidangran.top/gtpxwksfwl.html

JS:   const square = x => x * x;
来源：http://hz.hammf.cn/gtfgvioijp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtagshzefz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gtfxlupnem.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.havefunace.top/gtnawokvvp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gogol.net.cn/gthfpngjir.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtdgbaegww.html

[C07] 把函数作为参数传入
来源：http://hz.cqqwz.cn/gtnbjbhveh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtvnpmnjbf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gthldmaggv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guowangkeji.top/gtsbhsphfh.html

TS:   arr.map(String)
来源：http://hz.xuetiantiany.cn/gtacocrrvy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gtthvnfqru.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shzxlz.cn/gtzegndihi.html

Ruby: arr.map(&:upcase)
来源：http://hz.jiagoushi.top/gtgspcvfoi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gthuwwfavx.html

[C08] 闭包
来源：http://hz.yongpay.top/gtsquxepmg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gotoacloud.top/gtolmnbiyw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenjidiqi.icu/gtvrnedmvz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtromgczpp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtcnvmzqhg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zycfv.cn/gtzztzeyes.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zdqjudy.top/gtvbcgvisv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtqqphcqgt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtohyfwywd.html

[C09] 递归
来源：http://hz.cashguo.top/gtezroxghc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yonumen.top/gtnnnhrqky.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gtjgokyoam.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aibaodan.cn/gtavjobjul.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtwsblqjuu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tianlin.xyz/gtqdjbmpps.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gotoacloud.top/gtfxnkfdoz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtvxrijhwx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtcputzwpc.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gtkadbkstg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gteemgmksp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtmpmmijep.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ppjwa.cn/gtjnkuebff.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtqvwmgkoq.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtscvhtlcb.html

Go:   花括号块级作用域
来源：http://hz.feifeiyinyue.top/gtvitxarkx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtccfchkxp.html

C#:   块级作用域
来源：http://hz.jianghu66.top/gttittddrw.html

[C11] 模块导入与导出
来源：http://hz.yanxiufei.cn/gtbcnwmiwn.html

Py:   from module import func
来源：http://hz.jlsjyb.cn/gtqklansvi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258.top/gtvqdrjroq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtwdpetnjb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhongyouzk.top/gttnuvkzro.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtjxtiyeqd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.meibo888.top/gtbjcaylwz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gtzcxfhscj.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gtvcbiwoun.html

[C12] 立即执行函数 IIFE
来源：http://hz.iojbl.cn/gtqcuurlfn.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtabrzhxmt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gtwznatkbc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gtutgvgfaf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gthtdghuri.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gaohongyu789.top/gtfhiuiymt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gtwrwjegiy.html

Ruby: -> { puts "run" }.call
来源：http://hz.tanke756.top/gtqatbwmou.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yanxiufei.cn/gtzwlnjloc.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgufenzy.top/gtttxlusbi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.meibo888.top/gtjckwvhbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtksuabjyl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtwhgpmdon.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtwhkogcbf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtljrjskvi.html

Go:   func add(a, b int) int
来源：http://hz.9152youxi.cn/gtogtvyxcm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.meibo888.top/gtgkgjjxll.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.mhx1999.top/gtssxgtlgq.html

[C14] 泛型函数
来源：http://hz.cheryme.top/gtnghvsajr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.haohaochexian.top/gtszynhdoc.html

PHP:  // 无泛型
来源：http://hz.cqqwz.cn/gthtpwezlb.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtznimfubz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtmfwbityn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhiwuduotai.top/gtmormcuuu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gtepmyimha.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtipuombwg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtkhyvxuwj.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtcupaibsy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.316326.xyz/gtxomuxpcc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xinyue.icu/gtvtouomdl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tanke756.top/gtkjbdndxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtxllxorje.html

Java: // 无解构
来源：http://hz.gzhubu.top/gtjblluumd.html

Go:   // 无解构
来源：http://hz.zhongyouzk.top/gtnvamqqxo.html

Ruby: a, b = pair
来源：http://hz.gotoacloud.top/gtarwckliq.html

C#:   var (a, b) = pair;
来源：http://hz.yuxming.cn/gtawzujauk.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtknwkymtg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.svipenyu.cn/gtwbylbkws.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gtjbhnufqo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtyfrpqkkc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtkirthgqe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.redwolf501.top/gtmbcbbqzx.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtfjdevnpf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhoulong.xyz/gtpdabvrgb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gtgoueiqya.html

================================================================================
来源：http://hz.zhixingplan.top/gtvqhypxvf.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gtcchemadi.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrykduxwx.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtakxqygqa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtqitunere.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtfajzaznb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtswteycwh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtmrsxbpug.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.svipenyu.cn/gtkmztrfwu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gtfvrtxlcj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cucudq.cn/gtngnemuvc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtpdnxoeha.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gttxxdebrc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gthjrfkmmf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhoulong.xyz/gtuswgteoq.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtrcgozyxr.html

TS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtqziecsil.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtnjzhjzzc.html

Go:   arr = append(arr, 4)
来源：http://hz.fengsongda.top/gttmwrysla.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangkeji.top/gtpoexdyib.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gthfsiqidl.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtivzgggle.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtaoaduumq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtxhvbvxzr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tianlin.xyz/gtjjdlurzo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtsfgkoibe.html

Java: list.add(0, 0);
来源：http://hz.xuetiantiany.cn/gtcbfilmwb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtftgvlzlf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gtvpjgdbdg.html

C#:   list.Insert(0, 0);
来源：http://hz.tanke756.top/gtmgjbrtpd.html

[D04] 删除元素
来源：http://hz.snrcjt.cn/gtzisbqfki.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.smart0.xyz/gteqxzbrsb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinghuilouyu.cn/gtxnwnxbfg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenlongwang.top/gtqfwlfuqa.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtmacoelcb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.dashuyun.cn/gtygpdajhy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtcjhiffdj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.bjfxy.top/gtjpqncrxf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gogol.net.cn/gtbgrokblj.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gttumianoe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtyebtevfw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gtyztvgikh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gtmlxsljaj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtwzkmcdjj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnqzz.top/gtfpkbbthf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.52xcode.cn/gtdckchdad.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtvcloyuvm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.52xcode.cn/gtpcjyptnh.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtxyufzgug.html

Py:   len(arr)
来源：http://hz.ivvv.top/gtkkdblzgg.html

PHP:  count($arr);
来源：http://hz.nanxuanxn.top/gtownkjjxe.html

JS:   arr.length
来源：http://hz.snrcjt.cn/gtvejbjybl.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtabvwhkhp.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtztybqhho.html

Go:   len(arr)
来源：http://hz.gaohongyu789.top/gttofvnidq.html

Ruby: arr.length; arr.size
来源：http://hz.hywenlv.cn/gtfajvpnuw.html

C#:   list.Count;
来源：http://hz.daria6918.cn/gtrrmaqkgz.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gthofqirvw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.iojbl.cn/gtdodopfes.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnxiangtu.top/gtyqycvmnr.html

JS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtrwizivaq.html

TS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtblextsto.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gtxvlamfce.html

Go:   arr[1:4]
来源：http://hz.zhongyouzk.top/gtzuewksne.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gtseuttilk.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gtclvtuvzx.html

[D08] 合并两个数组
来源：http://hz.aibaodan.cn/gtxciolclh.html

Py:   a + b;  a.extend(b)
来源：http://hz.ydzc1.top/gtftekoiow.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gtbvfukjhu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtwbhzkxuf.html

TS:   [...a, ...b];
来源：http://hz.cashguo.top/gtlmvzlhtn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yangfankeji.com/gtvrajauhu.html

Go:   append(a, b...)
来源：http://hz.quarkkingdee.top/gttatlrtur.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnxiangtu.top/gtnuathoax.html

C#:   a.Concat(b).ToList()
来源：http://hz.gotoacloud.top/gtonrldfem.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtupthtprk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtinoeotow.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtxzpblbpz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gtxasaceiq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gthrevpztm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.smart0.xyz/gtxpkqjrig.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yonumen.top/gtscokgoyk.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtchoipodb.html

C#:   list.Sort();
来源：http://hz.cqqwz.cn/gtasndphij.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhijiandao.cn/gtdppxwsui.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daxiang520.top/gtwwetijyq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtsgkhztjf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtctdnkdfz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtbuasyhyo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gteossykvm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtiedvibce.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.kuanghao11.cn/gthmnnyaqg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yueranfly.top/gtxmzjnclm.html

[D11] 反转数组
来源：http://hz.birdmap.top/gtskegrncy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxinkj.top/gtqinmxcyu.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtkfspijio.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nwbrower.top/gtbualjiup.html

TS:   [...arr].reverse();
来源：http://hz.gaohongyu789.top/gtkgchjune.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtlqzmbkwp.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtbmgprmri.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtlftmbugw.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gtodfvbnzy.html

[D12] 查找元素下标
来源：http://hz.yonumen.top/gtumpahhfw.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtfdeenjld.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtjrzbthmg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtlevsirhr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtwktpgnnc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhijiandao.cn/gtgkyewwkx.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtpljkgwtr.html

Ruby: arr.index(x)
来源：http://hz.nanxinkj.top/gtsmfttogd.html

C#:   list.IndexOf(x);
来源：http://hz.xinyue.icu/gtdjsaahwz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yueranfly.top/gtjajdlyqj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtdejzmqlp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.iojbl.cn/gttiofaxad.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtlipagrde.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtpydggmpz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cheryme.top/gtzfkecfmz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gteelwfzsl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtgbqirwje.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shuidangran.top/gtqpuljvrc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtltsprchp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtrfhdeegs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gtkhmwfebn.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtoyqvjgca.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gttzvtzamb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.kuanghao11.cn/gtqrcktkur.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtlnxhkqjm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtlfdrphdn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtlrvscnfd.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtcgyuwcxs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtqvnolcns.html

PHP:  array_unique($arr);
来源：http://hz.haohaochexian.top/gtiezpqaig.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtlbbrrrrs.html


<!-- 参考信息 -->