代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gteehymcfh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jlsjyb.cn/gtlsfpurli.html

[B15] 布尔运算与取反
来源：http://hz.jqgufenzy.top/gtiupnrzmi.html

Py:   a and b or not c
来源：http://hz.kuanghao11.cn/gtqpztbrdv.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtraeamshe.html

JS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtftqllsxq.html

TS:   a && b || !c
来源：http://hz.cucudq.cn/gticmrbrtw.html

Java: a && b || !c
来源：http://hz.cqqwz.cn/gtmtdvwrbc.html

Go:   a && b || !c
来源：http://hz.yj20258888.top/gtdmsqqsws.html

Ruby: a && b || !c
来源：http://hz.gotoacloud.top/gtdrwwmoee.html

C#:   a && b || !c
来源：http://hz.yangfankeji.com/gtnqkfbzcq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yanxiufei.cn/gtcsnhtnyx.html

Py:   if not data: return
来源：http://hz.yonumen.top/gtassmegxp.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigfzy.top/gtdiykuywz.html

JS:   if (!data) return;
来源：http://hz.vqdsnc.cn/gtvxaoupyd.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtgkwejvym.html

Java: if (data == null) return;
来源：http://hz.ppjwa.cn/gthsxfdzsy.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtyliupzag.html

Ruby: return if data.nil?
来源：http://hz.yangfankeji.com/gtnbwjuudg.html

C#:   if (data == null) return;
来源：http://hz.haohaochexian.top/gtxxiaayht.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkzjpjaad.html

C. 函数与作用域
来源：http://hz.xziqi.cn/gtpwegeumr.html

================================================================================
来源：http://hz.chenzaomai.com/gtauapixuc.html

[C01] 定义函数
来源：http://hz.gogol.net.cn/gtmeoeukzf.html

Py:   def add(a, b): return a + b
来源：http://hz.snrcjt.cn/gtyadbjpmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gthhfhbbiz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxinkj.top/gtuhornije.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtciwidmjn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gteeswdobg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.birdmap.top/gtqgkjasac.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shuidangran.top/gtbpnflfat.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtinaviwzf.html

[C02] 默认参数
来源：http://hz.cucudq.cn/gtkvagtucg.html

Py:   def greet(name="World"): return name
来源：http://hz.vqdsnc.cn/gtpknopmoy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.kuanghao11.cn/gtzxujvamu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhijiandao.cn/gtihylweqx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ybcxt.top/gtdvwvwgzz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.316326.xyz/gtfbbclimo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gtdhuympqt.html

Ruby: def greet(name = "World") = name
来源：http://hz.yangfankeji.com/gtjljhtppt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.kuanghao11.cn/gtvvhtgbsv.html

[C03] 可变参数
来源：http://hz.ivvv.top/gtuvwgssel.html

Py:   def total(*args): return sum(args)
来源：http://hz.xingfuxueyuan.xyz/gtzafysejp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtmhpeaxhq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xziqi.cn/gtmosergsj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258888.top/gtuxyjetal.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtnlhtfoqz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gtseqlnocz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yvedp.cn/gtmdzbypur.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtncewdubv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtrjcaaisf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtjtximuxi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gtzojzxsxn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yongpay.top/gtrrapbosc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtrwzmtssp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zdqjudy.top/gtssgmmjqi.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinghuilouyu.cn/gtycxoktut.html

Ruby: f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gttxmtrnhz.html

C#:   f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtsqilrswh.html

[C05] 返回多个值
来源：http://hz.birdmap.top/gthextnepr.html

Py:   return a, b
来源：http://hz.yuanzhike.top/gtjovfhnms.html

PHP:  return [$a, $b];
来源：http://hz.xingfuxueyuan.xyz/gtkkyqwnnl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yvedp.cn/gtdyxysiyy.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtwgtmiqej.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xinyue.icu/gtwvedpdmr.html

Go:   return a, b
来源：http://hz.hongshengwenyu.top/gtkkolnmzr.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtdqutwqsu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pycfn.com/gtaopstosq.html

[C06] 匿名函数 / lambda
来源：http://hz.xingfuxueyuan.xyz/gtgdmnzepn.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtgrnetuso.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guannengcc.top/gtvxdibmgr.html

JS:   const square = x => x * x;
来源：http://hz.havefunace.top/gtramihvvp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtfdeeuogj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.c1oappe.top/gtrxmauppa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.redwolf501.top/gtwixykcri.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydzc1.top/gtweiubkzx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cucudq.cn/gthahnznfc.html

[C07] 把函数作为参数传入
来源：http://hz.jinyuanbaomall.cn/gteekhrllh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aibaodan.cn/gtdgoteiir.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinghuilouyu.cn/gtwghlisti.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gtpgfdqcqt.html

TS:   arr.map(String)
来源：http://hz.yueranfly.top/gtnrfdtrsh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jyoumei.cn/gtgblwxixs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jianghu66.top/gtlleswyjm.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtcokuedww.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jianghu66.top/gtsouptibq.html

[C08] 闭包
来源：http://hz.daria6918.cn/gtnjhqmwda.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xuanzx.com/gtkvfndnsb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgfzy.top/gtwswqvxga.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gthfcfbrew.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtvbtivwau.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daxiang520.top/gtvfxrjryx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxuanxn.top/gtgnmdpzwn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gtxuttudiq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtcrolfpqz.html

[C09] 递归
来源：http://hz.hfpthk.cn/gtdhvpbpva.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtgeyiftmw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gttjwxmkjl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtbimmntrz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtqwcqgdkx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhiwuduotai.top/gttojbnztv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigfzy.top/gtzpdbakoo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gtqqijedjd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtbvlwgqhc.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtntaftbab.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinghuilouyu.cn/gtjpczsqsi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtygotieto.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtduciwnkx.html

TS:   同 JS
来源：http://hz.svipenyu.cn/gtjwzzaiud.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtgzxkisec.html

Go:   花括号块级作用域
来源：http://hz.havefunace.top/gtaefgkelw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtlxvghpkg.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtkkaoxthj.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtqfrkhnmo.html

Py:   from module import func
来源：http://hz.0kj1m.cn/gtkqxlwhcc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.pycfn.com/gttqddxlyo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.andypj.xyz/gtrjuclefe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj20258888.top/gtwyxhsvaa.html

Java: import java.util.List;
来源：http://hz.svipenyu.cn/gtexbacyea.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jlsjyb.cn/gtinjyvzgs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xylfe.cn/gtfofrwfxq.html

C#:   using System.Text;
来源：http://hz.tian-w.cn/gtzwnmxqxy.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtbzhlgmqa.html

Py:   (lambda: print("run"))()
来源：http://hz.chenzaomai.com/gtnftuhyru.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yangfankeji.com/gtugocdbna.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtxjkorczj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtkpzgziya.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yongpay.top/gtfjhtjuoz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gogol.net.cn/gtoihyjbkt.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtqzxlwiyp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangtech.top/gtjzkutzln.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gtqmgolnyc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydzc1.top/gtgdvexncj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtohdpthju.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenlongwang.top/gtxsfvaxps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtyxbwsiir.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtucxbyxul.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtcdnjlxxp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtzcbjpsay.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gttdaxksfs.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gtlanifzjm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtwcxbsenj.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtvrtyotvi.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtplhdepsd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gtuzpeslxo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj202588.top/gtidjdcsbn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tianlin.xyz/gtstdwoctz.html

Ruby: # 无泛型
来源：http://hz.ydjk.org.cn/gthjvthvjh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gotoacloud.top/gtkywqixxb.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtstuopbno.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhoulong.xyz/gtfqtjdnmf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guannengcc.top/gtloeplcrd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtmvgbaaot.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtomizrzwl.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtrlhkutne.html

Go:   // 无解构
来源：http://hz.zhixingplan.top/gtffnpiudm.html

Ruby: a, b = pair
来源：http://hz.haohaochexian.top/gtvzabxkwy.html

C#:   var (a, b) = pair;
来源：http://hz.jlsjyb.cn/gtichgrooi.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtdzloltfl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtrfvbzkfz.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtgvjvchwr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nwbrower.top/gtomyfsvhx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yanxiufei.cn/gtdnlncutl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258888.top/gtffclifxo.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtfmtemaxw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pycfn.com/gtbzhujdkk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.9152youxi.cn/gtymlbclqz.html

================================================================================
来源：http://hz.cqqwz.cn/gtakfsjtau.html

D. 数组 / 列表 / 集合
来源：http://hz.nwbrower.top/gttljrnlee.html

================================================================================
来源：http://hz.xylfe.cn/gtircytpem.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gttngysrmb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtivyqqxer.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtdnalhgwl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.birdmap.top/gtkhfvfrih.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ywan-chungtsiang.top/gtxgydfolw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cdnleiting.top/gttuazbwib.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtuuahbqji.html

Ruby: arr = [1, 2, 3]
来源：http://hz.bjfxy.top/gthbfjanwi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhiwuduotai.top/gtwoacmqzk.html

[D02] 追加元素到末尾
来源：http://hz.gzhubu.top/gtkqzvhywl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangshuangyany.cn/gtcbgwmdpl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigfzy.top/gtinpdwoms.html

JS:   arr.push(4);
来源：http://hz.sxryk.cn/gtxlhhtyry.html

TS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtdoafgstu.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gtdznlrcsa.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtquojyelw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinghuilouyu.cn/gtkjfhtllw.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gtbruhmheq.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtyqhdikeb.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtfcgxhomi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtnractohm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yanxiufei.cn/gtiwaghghq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtvaoqsjqd.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangtech.top/gtiorejsmp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sxryk.cn/gtftgqwmdy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hongshengwenyu.top/gtqxaxsxcb.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtvhdbgvjj.html

[D04] 删除元素
来源：http://hz.yonumen.top/gtpzweozyg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtwysrwsel.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuanzhike.top/gtpdshsaet.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jqgfzy.top/gtyfujkubs.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtwinmexxa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtmznohtha.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.kuanghao11.cn/gttsljhcjh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.316326.xyz/gtnjzqrpsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yanxiufei.cn/gtiduhwfwt.html

[D05] 访问与修改元素
来源：http://hz.xuetiantiany.cn/gttoqitowe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gthoxfvwgb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tanke756.top/gtuvzzwlcg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtskxkfknk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jqgfzy.top/gtnwnzclid.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtdhrfwucm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtseywfevw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtjixbswsx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigufen.top/gtkkeoyoww.html

[D06] 数组长度
来源：http://hz.hywenlv.cn/gtsxhhaugl.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtlknjkjgz.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtogprsimz.html

JS:   arr.length
来源：http://hz.birdmap.top/gttmbiesur.html

TS:   arr.length
来源：http://hz.pengpengdd.cyou/gtbwcuwrdw.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtgliuyehl.html

Go:   len(arr)
来源：http://hz.yj202588.top/gtgalizkym.html

Ruby: arr.length; arr.size
来源：http://hz.sufxvd.cn/gtzjzvosvs.html

C#:   list.Count;
来源：http://hz.xuetiantiany.cn/gthcbxkewe.html

[D07] 切片 / 取子数组
来源：http://hz.haohaochexian.top/gtmhtcefxd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtrhydvwbf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtdqtbvxpp.html

JS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtwgynbuie.html

TS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtvyujmblx.html

Java: list.subList(1, 4);
来源：http://hz.vqdsnc.cn/gtirefvirb.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtkfavxzez.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtmxarkysn.html

C#:   list.GetRange(1, 3);
来源：http://hz.hnqzz.top/gtgxxcsnlw.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtjhemdwsn.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gthkwhhyfs.html

PHP:  array_merge($a, $b);
来源：http://hz.zhoulong.xyz/gtnzwnerqe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuxming.cn/gtmejheyxr.html

TS:   [...a, ...b];
来源：http://hz.xylfe.cn/gtlwvfbdex.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258.top/gtrlkxokxc.html

Go:   append(a, b...)
来源：http://hz.jianghu66.top/gtjeddplgd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.meibo888.top/gtnhrwmhpp.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtjcitvcwb.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtklyjviuf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtqzijujhg.html

PHP:  sort($arr);
来源：http://hz.haohaochexian.top/gtufgjckae.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ybcxt.top/gtxguodfqj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtejvkjsou.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.0kj1m.cn/gtbilknqpy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gthocottfp.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtgqtkrutk.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtgyialucq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtfteaudbf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.bjfxy.top/gtgjjrosks.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.snrcjt.cn/gttngfnyra.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtuoxpzjti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtahpzzckb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtidtzqlpg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ppjwa.cn/gthorqrphe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtuoghhgrd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtfvdytiuh.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtijvjxidv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtjhltfzyl.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtgwhkirio.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhoulong.xyz/gtnxjckzms.html

TS:   [...arr].reverse();
来源：http://hz.ivvv.top/gtgmaujpeu.html

Java: Collections.reverse(list);
来源：http://hz.zhijiandao.cn/gttjvokpgn.html

Go:   slices.Reverse(arr)
来源：http://hz.tanke756.top/gtenjvjrlj.html

Ruby: arr.reverse
来源：http://hz.316326.xyz/gtvdnhvlts.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtjifkoalu.html

[D12] 查找元素下标
来源：http://hz.andypj.xyz/gtauajyhxk.html

Py:   arr.index(x);  x in arr
来源：http://hz.sysykeji.top/gttqtgtsdd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtxpvwtfep.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtlqpwvibs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtowhuzlka.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtihouppwp.html

Go:   slices.Index(arr, x)
来源：http://hz.yj202588.top/gtpjiynujg.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtbjyffwtn.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gtjvsbnooi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.andypj.xyz/gttppkvfvw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gtjjbtwaxs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258888.top/gtdebhntpl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtdmkynzuj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.vqdsnc.cn/gtzefjtnzl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gtezddoqfh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtxjjgawsf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtomykioxd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cheryme.top/gtauvyzavc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhijiandao.cn/gtrpaoeekc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xinyue.icu/gtavkxqhwi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtuqmggzzi.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtdpngtlfb.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtjxpiioih.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtrjvwrdgs.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtkcbvbtde.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gtauodvwku.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtzxpuyplt.html

[D15] 去重
来源：http://hz.hfpthk.cn/gtpyqwlntd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtnmxnknqq.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gtzuznvaqg.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtcrtkgmmn.html


<!-- 参考信息 -->