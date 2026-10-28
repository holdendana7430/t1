代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtlgoggxwm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tian-w.cn/gtewtfpdhi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cucudq.cn/gtqlscqpae.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tianlin.xyz/gthhlinpig.html

[B13] 判断是否为数字
来源：http://hz.hnxiangtu.top/gtvudtgjok.html

Py:   isinstance(x, (int, float))
来源：http://hz.daxiang520.top/gtymfzoknv.html

PHP:  is_numeric($x)
来源：http://hz.shangyingyoupin.top/gtefzrdcws.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtwbtwsyjs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtjysprdyn.html

Java: x instanceof Number
来源：http://hz.316326.xyz/gtrthwpogg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtzhxengbj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cdnleiting.top/gtiqipreqr.html

C#:   x is int or double or decimal
来源：http://hz.yj20258888.top/gthigcidln.html

[B14] 判断值是否在集合内
来源：http://hz.wangdashe.top/gtqvfjjivs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.havefunace.top/gtnoxkxtvf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jianghu66.top/gtwbaltgky.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shangyingyoupin.top/gtyocyhorz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shzxlz.cn/gtwjnfthyl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtbidjrbpb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.pycfn.com/gtwxawcvew.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.svipenyu.cn/gtbspixsdk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hnxiangtu.top/gtupmvneon.html

[B15] 布尔运算与取反
来源：http://hz.birdmap.top/gtezsghnrk.html

Py:   a and b or not c
来源：http://hz.cashguo.top/gtgnhogjgp.html

PHP:  $a && $b || !$c
来源：http://hz.ydjk.org.cn/gtjjojlocr.html

JS:   a && b || !c
来源：http://hz.cashguo.top/gthgynjwwp.html

TS:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtwccaargb.html

Java: a && b || !c
来源：http://hz.havefunace.top/gtnybblsgw.html

Go:   a && b || !c
来源：http://hz.ybcxt.top/gtkzqcmlhg.html

Ruby: a && b || !c
来源：http://hz.zhiwuduotai.top/gtylwuhpbr.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtghbujhnl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tanke756.top/gtchuyqiuw.html

Py:   if not data: return
来源：http://hz.cheryme.top/gtqlfckucc.html

PHP:  if (!$data) { return; }
来源：http://hz.wangdashe.top/gtcxgmwpgt.html

JS:   if (!data) return;
来源：http://hz.smart0.xyz/gtkecxqekf.html

TS:   if (!data) return;
来源：http://hz.svipenyu.cn/gtzqywbugp.html

Java: if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtpgfholeh.html

Go:   if data == nil { return }
来源：http://hz.yj20258.top/gtuarbxmcg.html

Ruby: return if data.nil?
来源：http://hz.hysaishi.cn/gtqlxxhakj.html

C#:   if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gthuqzaypx.html

================================================================================
来源：http://hz.gzhubu.top/gtskvtqspq.html

C. 函数与作用域
来源：http://hz.ydjk.org.cn/gtkvyzpjzv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwbxtpuaq.html

[C01] 定义函数
来源：http://hz.hammf.cn/gtwqopdqds.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtncjxxnpi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtuvpcqwhy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxinkj.top/gtyeanhcgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtyyxaygaq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtdeejpvtx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtpccehigf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.feifeiyinyue.top/gtsxiruvvs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtgluwcrim.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtdypdyqsd.html

Py:   def greet(name="World"): return name
来源：http://hz.sxryk.cn/gthregvmed.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtgscbvpxd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gtjlejdvzb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtbnfnvxhr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinyuanbaomall.cn/gtyjfzlxxb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtmfwyfymn.html

Ruby: def greet(name = "World") = name
来源：http://hz.meibo888.top/gtubzkojcx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtmkpeasrr.html

[C03] 可变参数
来源：http://hz.shanyushiyangkeji.top/gtbnhobgyj.html

Py:   def total(*args): return sum(args)
来源：http://hz.xinyue.icu/gthdvlovuq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigufen.top/gtuhiadmef.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtxzvtkdty.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtcaitoebx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtlrofjcuk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cashguo.top/gtikudiyrj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cdnleiting.top/gtmspqpdkq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gotoacloud.top/gttruhgltm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtaezontcp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.9152youxi.cn/gtmkrdkceb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gthwavlspb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.316326.xyz/gtmxyukgmy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ybcxt.top/gtbybvnitp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtrarvigro.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtkeanbuqo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtvqljojre.html

C#:   f(a: 1, b: 2)
来源：http://hz.ivvv.top/gtwevvgtch.html

[C05] 返回多个值
来源：http://hz.tian-w.cn/gtnkcyfrhi.html

Py:   return a, b
来源：http://hz.svipenyu.cn/gtvppcwbay.html

PHP:  return [$a, $b];
来源：http://hz.jinyuanbaomall.cn/gtgozzvzur.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtnoonrvoq.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtyyvrpikm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.meibo888.top/gtwhawgfvd.html

Go:   return a, b
来源：http://hz.birdmap.top/gttibhrmkq.html

Ruby: return a, b
来源：http://hz.birdmap.top/gtjsffimzp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tanke756.top/gtjlmfqrjs.html

[C06] 匿名函数 / lambda
来源：http://hz.zhijiandao.cn/gtpofvoaza.html

Py:   square = lambda x: x * x
来源：http://hz.dianchejie.cn/gtxtbadpxb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhaomingkeji.xyz/gtmqarfmhi.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtqlpqrjvx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gzhubu.top/gthrsuttbf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtneoukdko.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtavnyurqz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtqpozhbln.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gtnkbaipog.html

[C07] 把函数作为参数传入
来源：http://hz.yj202588.top/gthejboltu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xingfuxueyuan.xyz/gtqpfuenna.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ywan-chungtsiang.top/gtaenglxvk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtppahgtet.html

TS:   arr.map(String)
来源：http://hz.hywenlv.cn/gtvonepxjo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sufxvd.cn/gtdrpmhaks.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.52xcode.cn/gtayofvmyh.html

Ruby: arr.map(&:upcase)
来源：http://hz.hongshengwenyu.top/gtepyitcvd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ybcxt.top/gtejfjxmmh.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtvjishmao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tanke756.top/gteigzzfyn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nwbrower.top/gtnnuvioxi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtslobxbtz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtowzwmmoe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.havefunace.top/gtpimiyeaq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydjk.org.cn/gtjvuyhdqk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtwbkfirjp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtjnqdknxe.html

[C09] 递归
来源：http://hz.zdqjudy.top/gtdaizbrqf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtczroniiv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.bjfxy.top/gtzqgoamve.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtabgncksd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtrvdcnihu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhongyouzk.top/gtbyhfpcnb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtwfbtizcg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtsmysoutc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhaomingkeji.xyz/gtxvfbxhlc.html

[C10] 变量作用域
来源：http://hz.nwbrower.top/gtewoyaksy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shangyingyoupin.top/gthhejaavb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuetiantiany.cn/gtracstizc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtuhwpipvr.html

TS:   同 JS
来源：http://hz.yj202588.top/gtmcfldaol.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtcouchkih.html

Go:   花括号块级作用域
来源：http://hz.fengsongda.top/gttiwslnfn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.birdmap.top/gtnedbijoh.html

C#:   块级作用域
来源：http://hz.cqqwz.cn/gtijfuepbc.html

[C11] 模块导入与导出
来源：http://hz.aibaodan.cn/gtktxduyui.html

Py:   from module import func
来源：http://hz.zhijiandao.cn/gtmrexvahg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtelaqgife.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gttqnzescl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gtkxcepmqa.html

Java: import java.util.List;
来源：http://hz.hywenlv.cn/gtgezvhveq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daria6918.cn/gtytsaqest.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangtech.top/gtmrhccxtt.html

C#:   using System.Text;
来源：http://hz.xinyue.icu/gttpruyvns.html

[C12] 立即执行函数 IIFE
来源：http://hz.meibo888.top/gtfmfqfjhy.html

Py:   (lambda: print("run"))()
来源：http://hz.birdmap.top/gtsdqrqlya.html

PHP:  (function () { echo "run"; })();
来源：http://hz.smart0.xyz/gtqmhujlka.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtifumxpjc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtwfhpmndo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gtvtfzfsbu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gogol.net.cn/gtgpttbbmk.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhaomingkeji.xyz/gtbieowzsa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gtbsdnogio.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtzwobtmsa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtonxayypx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtyrvbixko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtgpkvswwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cucudq.cn/gtoadwsgjp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtbapcqhjv.html

Go:   func add(a, b int) int
来源：http://hz.yongpay.top/gtrddcvela.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtnxrahbsm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cdnleiting.top/gtggjqfaul.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtbohsjrag.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtkwcqtmen.html

PHP:  // 无泛型
来源：http://hz.zhijiandao.cn/gthxycokhy.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtryxwtqxp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxuanxn.top/gttjxvgkgk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gtccegqmwa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtihnoemxg.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtrobckjrv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gtdnvitirj.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtargogzcj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.snrcjt.cn/gtigiiurei.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ppjwa.cn/gtvujhfqgz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtintrxnnb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtofsicfzr.html

Java: // 无解构
来源：http://hz.jianghu66.top/gtfwrdconx.html

Go:   // 无解构
来源：http://hz.hnxiangtu.top/gtsqkkupwx.html

Ruby: a, b = pair
来源：http://hz.shangyingyoupin.top/gtqmoezfdk.html

C#:   var (a, b) = pair;
来源：http://hz.hywenlv.cn/gtfwgkboqw.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtfgojicek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtpfgksvob.html

PHP:  // 无重载
来源：http://hz.sxryk.cn/gtpawqzbex.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtzdvszohy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dianchejie.cn/gtpkfuwmsa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.9152youxi.cn/gtjewdenrw.html

Go:   // 无重载：用不同函数名
来源：http://hz.sxryk.cn/gtnevhkslr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgufenzy.top/gtkyktdvok.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hammf.cn/gtwojkszrl.html

================================================================================
来源：http://hz.guowangkeji.top/gttwawuxjp.html

D. 数组 / 列表 / 集合
来源：http://hz.mhx1999.top/gtjjkhhjak.html

================================================================================
来源：http://hz.cashguo.top/gtebyhjvxm.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtzjkncdze.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gttbgkazhm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtcikjtyoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxinkj.top/gtmgeebvdh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fzhhl.top/gtixtxwifv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gtaokpzkrx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtfdmpwrro.html

Ruby: arr = [1, 2, 3]
来源：http://hz.smart0.xyz/gtijrkpssk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhongyouzk.top/gtfoqzbixw.html

[D02] 追加元素到末尾
来源：http://hz.wangdashe.top/gtswxevvji.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xylfe.cn/gtffyldaly.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cqqwz.cn/gtwegpkecp.html

JS:   arr.push(4);
来源：http://hz.ybcxt.top/gtncvwpjeu.html

TS:   arr.push(4);
来源：http://hz.ehwqpu.com/gthflznlaj.html

Java: list.add(4);
来源：http://hz.ppjwa.cn/gtqfwobgxp.html

Go:   arr = append(arr, 4)
来源：http://hz.hywenlv.cn/gthrydzqen.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.meibo888.top/gtdidfqxeh.html

C#:   list.Add(4);
来源：http://hz.cucudq.cn/gtnqhmhseh.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtgbmhnabi.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gttpbbgxas.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gtdamurmoy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhiwuduotai.top/gtqalaxeow.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.guannengcc.top/gtqrhidzkl.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gtbpsidivd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guowangkeji.top/gtpmbzmdwf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigfzy.top/gtkizujwvy.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtxgzgahpl.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtodjdrdsg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtmoxkkbkw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yvedp.cn/gtsfejmtgy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtxltwkwux.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtpuddmefu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.dianchejie.cn/gtdmaibekp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.bjfxy.top/gtftlkaqmc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shuidangran.top/gtwjwncyek.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sweek.top/gtwxfhtgug.html

[D05] 访问与修改元素
来源：http://hz.sufxvd.cn/gthqrwfyik.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtvqdxthxh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.snrcjt.cn/gtqkfbzkca.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fengsongda.top/gtqehfybwu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nwbrower.top/gtzgdtddhh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtmtlscrer.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtuizcbify.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtlgaknxaf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gthpjxkpox.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtywpeuvho.html

Py:   len(arr)
来源：http://hz.cucudq.cn/gtbomacdcp.html

PHP:  count($arr);
来源：http://hz.wangshuangyany.cn/gtsutdceje.html

JS:   arr.length
来源：http://hz.iojbl.cn/gttcwdoxin.html

TS:   arr.length
来源：http://hz.daxiang520.top/gtdtvcgkjs.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtqwdmbesu.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtogttxdvq.html

Ruby: arr.length; arr.size
来源：http://hz.aizwys.cn/gtkqarjvsq.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtbzjwmgtd.html

[D07] 切片 / 取子数组
来源：http://hz.yangfankeji.com/gthcjrxhrx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yangfankeji.com/gttvbwlsoi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtmxitewpg.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtmaergbie.html

TS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtyujellwc.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtulbbnppt.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtzfwsrjsk.html

Ruby: arr[1, 3]
来源：http://hz.mhx1999.top/gtkffetiwk.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhoulong.xyz/gtwlqyejwh.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtenarcybh.html

Py:   a + b;  a.extend(b)
来源：http://hz.vqdsnc.cn/gtxyxbhyos.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtjkdmobaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gzhubu.top/gtlxhukyvv.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtyywiwqfz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.redwolf501.top/gtmspdmsij.html

Go:   append(a, b...)
来源：http://hz.xziqi.cn/gthdrldktb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jianghu66.top/gtmcbyqrdv.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhijiandao.cn/gtlviwsgxb.html

[D09] 排序（升序）
来源：http://hz.shuidangran.top/gtcynezfgt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtoefsyzcc.html

PHP:  sort($arr);
来源：http://hz.yvedp.cn/gtlpaadsij.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hfpthk.cn/gtkafsippz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gtbudflfkh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhengqikj.top/gtueozmyyd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtbbsgfary.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtsxmljmmd.html

C#:   list.Sort();
来源：http://hz.jinqigfzy.top/gtsadshbml.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtuvnshsyr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtmsdnwrnc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gthqsvcyht.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtdutgxcss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtnbyyhltr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daria6918.cn/gtwmdszhxb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtktrgbgmb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtyhagwcnb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.meibo888.top/gtqeanjvro.html

[D11] 反转数组
来源：http://hz.jqgufenzy.top/gtxywhgkkn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtzewwyafq.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtyjuqypxl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuxming.cn/gtizphryjp.html

TS:   [...arr].reverse();
来源：http://hz.gogol.net.cn/gtttqypwlk.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtjysmxiyb.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtottvzlcb.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtrumwjzfs.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtlutazget.html

[D12] 查找元素下标
来源：http://hz.jianghu66.top/gtujszsjnq.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtfyavuhbd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangdashe.top/gtvmccnjzy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtuyzaiody.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtdwtldmoo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtmiyrndwz.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtzfogysbj.html

Ruby: arr.index(x)
来源：http://hz.yvedp.cn/gtfzbmajne.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtfrteecmi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gotoacloud.top/gtvapeogco.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtsmkgvbth.html


<!-- 参考信息 -->