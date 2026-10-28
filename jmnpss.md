代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtetogbbgy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.kuanghao11.cn/gtllvwrdgl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jyoumei.cn/gteutphbkb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangshuangyany.cn/gtwzhkbwoq.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gtcbblmghv.html

Py:   isinstance(x, (int, float))
来源：http://hz.0kj1m.cn/gtbphjfeem.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gtsdvllvva.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhijiandao.cn/gtdrjzfads.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtfoxbegqb.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gtjnglpheo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangshuangyany.cn/gtgfzpfsny.html

Ruby: x.is_a?(Numeric)
来源：http://hz.snrcjt.cn/gtvuitkoyt.html

C#:   x is int or double or decimal
来源：http://hz.yueranfly.top/gthwhvjysy.html

[B14] 判断值是否在集合内
来源：http://hz.havefunace.top/gtaopsaqpp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.daxiang520.top/gtofkckyhd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hongshengwenyu.top/gtdcmaifsg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtkyhdzwmf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtyepwkueb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangshuangyany.cn/gtjgmmtina.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.feifeiyinyue.top/gtmhpqprsr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tianlin.xyz/gtaphdxweb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jianghu66.top/gtvafoyqub.html

[B15] 布尔运算与取反
来源：http://hz.zhixingplan.top/gtdnxonnka.html

Py:   a and b or not c
来源：http://hz.jyoumei.cn/gtppcgsbnm.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtqnmhbaie.html

JS:   a && b || !c
来源：http://hz.zhixingplan.top/gtuagmpwah.html

TS:   a && b || !c
来源：http://hz.yj20258.top/gtrqdmxuio.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtqveuzwbn.html

Go:   a && b || !c
来源：http://hz.0kj1m.cn/gtehugcdpn.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtwhocnngb.html

C#:   a && b || !c
来源：http://hz.chenlongwang.top/gttzcyvubw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xylfe.cn/gtwphnqqqk.html

Py:   if not data: return
来源：http://hz.feifeiyinyue.top/gticghrvpk.html

PHP:  if (!$data) { return; }
来源：http://hz.aizwys.cn/gtjnfttith.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtalcnlkff.html

TS:   if (!data) return;
来源：http://hz.sxryk.cn/gttcxncxsm.html

Java: if (data == null) return;
来源：http://hz.meibo888.top/gtvakdhtma.html

Go:   if data == nil { return }
来源：http://hz.yonumen.top/gtficrdaon.html

Ruby: return if data.nil?
来源：http://hz.dashuyun.cn/gtogkqdcir.html

C#:   if (data == null) return;
来源：http://hz.daria6918.cn/gtrvvuzzbx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtyospaqno.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtcewecqde.html

================================================================================
来源：http://hz.aibaodan.cn/gthdqkrpqg.html

[C01] 定义函数
来源：http://hz.shangyingyoupin.top/gtfepkxiht.html

Py:   def add(a, b): return a + b
来源：http://hz.shuidangran.top/gtquzmjyfq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtlivagnmh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtxtrwgelo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtrdggasnq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtxovqsesd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtxzslzumh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxinkj.top/gtxvgysnba.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtnnvhfxxi.html

[C02] 默认参数
来源：http://hz.jyoumei.cn/gtkirnsmki.html

Py:   def greet(name="World"): return name
来源：http://hz.xingfuxueyuan.xyz/gtglthsrgk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guannengcc.top/gtenwwhxfn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtgqtshtcn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtsmvnpnhf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jyoumei.cn/gtccpcltgh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gogol.net.cn/gtnubegjbv.html

Ruby: def greet(name = "World") = name
来源：http://hz.cdnleiting.top/gtjvbthqsu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtjuiuxfle.html

[C03] 可变参数
来源：http://hz.cucudq.cn/gtgzpxuuob.html

Py:   def total(*args): return sum(args)
来源：http://hz.smart0.xyz/gtrvfetciy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtgtrgwicv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhaomingkeji.xyz/gtcprsfcdn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtxxvzzinf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtrdpbhbhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gtnrirqtbg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aizwys.cn/gtlxpexpvf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuetiantiany.cn/gtkmamzsdt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.snrcjt.cn/gtxgkqldhw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ehwqpu.com/gtqilhdtqc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zycfv.cn/gtztytdara.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtnglkwdtm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtsiiwbtjq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhixingplan.top/gtqsfskwfk.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtvnilyowy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtprwwsuum.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtzwhossjl.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtpmbiacqv.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtccffmbcr.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtbhfmzypz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gotoacloud.top/gtxhhhjzyt.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gttdgibrtb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtpwpukpir.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtxmivuvos.html

Ruby: return a, b
来源：http://hz.jinghuilouyu.cn/gtjhsjdiuw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xingfuxueyuan.xyz/gtfqjrnfcw.html

[C06] 匿名函数 / lambda
来源：http://hz.guowangkeji.top/gtrkwdgugb.html

Py:   square = lambda x: x * x
来源：http://hz.yonumen.top/gtjiymxpcw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtneejvqhx.html

JS:   const square = x => x * x;
来源：http://hz.ybcxt.top/gtivylozuo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ivvv.top/gtsbncomyv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hongshengwenyu.top/gtcnkoyxwh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.smart0.xyz/gtqvesykan.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtqeczpmpw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gzhubu.top/gtjuteusfl.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtrkipebbp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgufenzy.top/gtriuxxxvc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ppjwa.cn/gtfsbdools.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ivvv.top/gtpsilmuhi.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtkrxftdli.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtyygbuplb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gthcpuwgnt.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtauhgdwjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhixingplan.top/gttlogsabw.html

[C08] 闭包
来源：http://hz.yj202588.top/gtanopofjk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aibaodan.cn/gtoxqdttdj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gtcfdtxwlh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtdujlrcoc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtoriwlpzj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gtndemuibp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtqmglfccz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hywenlv.cn/gtphlzjlcm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shangyingyoupin.top/gtdwhlwdti.html

[C09] 递归
来源：http://hz.chenlongwang.top/gtpdyeseru.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.redwolf501.top/gtxhifhwux.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jiagoushi.top/gtwnoufbgn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtkmuxkcuj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtenzokqwa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtngtmtnre.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigufen.top/gtabthhwsv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtrnzrztmg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtygqmtekp.html

[C10] 变量作用域
来源：http://hz.52xcode.cn/gtzqrzidgu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtrpbcnwid.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhongyouzk.top/gthfajsenw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuanzhike.top/gtpkqneyha.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtsvdmfsom.html

Java: 方法内为块级作用域
来源：http://hz.xinyue.icu/gtugozmuwk.html

Go:   花括号块级作用域
来源：http://hz.chenlongwang.top/gtniwbkxui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgufenzy.top/gtszkwtrpa.html

C#:   块级作用域
来源：http://hz.redwolf501.top/gtssqwkuye.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtznbjfpvn.html

Py:   from module import func
来源：http://hz.aibaodan.cn/gtlvbcvydx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtqdngtewz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ivvv.top/gtqbjulskr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jianghu66.top/gtgvtwajfj.html

Java: import java.util.List;
来源：http://hz.hysaishi.cn/gtkfqiuife.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenjidiqi.icu/gtyagzdmua.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangshuangyany.cn/gtwgintvaf.html

C#:   using System.Text;
来源：http://hz.sysykeji.top/gtzatxsgow.html

[C12] 立即执行函数 IIFE
来源：http://hz.shzxlz.cn/gtamormpry.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtqwewfmdw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hongshengwenyu.top/gtjmafloyu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtjffeshvm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtqwfjzhxv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtxmthddif.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tianlin.xyz/gtvmfbeeqh.html

Ruby: -> { puts "run" }.call
来源：http://hz.jlsjyb.cn/gtexhcfeny.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhijiandao.cn/gtaeygrutj.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinghuilouyu.cn/gtmstdkpmz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jiagoushi.top/gtvtwwapfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtutnlwfse.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtegedwmvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hongshengwenyu.top/gtyognzxki.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtlbadzavk.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gtjoyewkmo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gthafazsfd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.bjfxy.top/gtaarpqmpp.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gtgntkiuwd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgufenzy.top/gtaimqytsd.html

PHP:  // 无泛型
来源：http://hz.ppjwa.cn/gtgyoiblpi.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtxqkzvfwy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.svipenyu.cn/gtvqsecyac.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.c1oappe.top/gtrimawxsl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gttzhzgodg.html

Ruby: # 无泛型
来源：http://hz.zhaomingkeji.xyz/gtlqoowcom.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shanyushiyangtech.top/gtlmctyukn.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtxosaevmb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtsnazkcef.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtvcmklonu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtebomwsic.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtzwpbyqfu.html

Java: // 无解构
来源：http://hz.shzxlz.cn/gtgpideqkg.html

Go:   // 无解构
来源：http://hz.ppjwa.cn/gtnbecdurr.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtifylemva.html

C#:   var (a, b) = pair;
来源：http://hz.ywan-chungtsiang.top/gtocbduvom.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtbkeydmjo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtolqifitg.html

PHP:  // 无重载
来源：http://hz.tian-w.cn/gtiypgrdle.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtdmtcshhg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhixingplan.top/gtmfhmhugs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daria6918.cn/gtwltmwtac.html

Go:   // 无重载：用不同函数名
来源：http://hz.xylfe.cn/gtirpefoun.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zdqjudy.top/gtitshrznl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtypivcjqz.html

================================================================================
来源：http://hz.shuidangran.top/gtzimreqvx.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtfzmkprtj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpurjiuxz.html

[D01] 创建数组 / 列表
来源：http://hz.meibo888.top/gtdiydtbma.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtqhxdqcjg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.bjfxy.top/gtalfhtqmm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxinkj.top/gtybblexob.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtzplgowzc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydzc1.top/gttxjthlly.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtfwxuoutb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hysaishi.cn/gtkwkudrnt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nanxinkj.top/gtapgtmhul.html

[D02] 追加元素到末尾
来源：http://hz.yvedp.cn/gtmfjssfvp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.birdmap.top/gttytetbjk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhiwuduotai.top/gtfxnfeqko.html

JS:   arr.push(4);
来源：http://hz.sysykeji.top/gtejkbcvyd.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtdnbcring.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gttgdaxnqh.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtgbgtfpyo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.9152youxi.cn/gtcxbyzjdl.html

C#:   list.Add(4);
来源：http://hz.zhoulong.xyz/gtbcarfkwl.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gtmwnanztr.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtifgwahzq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xziqi.cn/gtzouxckih.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.9152youxi.cn/gtsfzelqug.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtteaugful.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtnnpjnpms.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sufxvd.cn/gtnkakzztv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gtctyihruw.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gttnrdsldz.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gttpjrnvfx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sufxvd.cn/gtqtgfvajv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gtlccqwoqt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangshuangyany.cn/gtqzfutkeb.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtfflvgwny.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zdqjudy.top/gtiouwljzt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtckbhpszk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gttfcyeibt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigfzy.top/gtunedoogb.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtcwpzznma.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtkxvvzpta.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtydfwixxy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fzhhl.top/gtqemzfpry.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtivxandyz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtesrgldry.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.9152youxi.cn/gttkfjnvdu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtvzmpcsgf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtlapncjvi.html

[D06] 数组长度
来源：http://hz.vqdsnc.cn/gtecvomxqx.html

Py:   len(arr)
来源：http://hz.vqdsnc.cn/gtmukqhzqc.html

PHP:  count($arr);
来源：http://hz.52xcode.cn/gtlmicjskr.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtlaxuaebr.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtgfuhrfth.html

Java: list.size();
来源：http://hz.sxryk.cn/gtfxbzspjz.html

Go:   len(arr)
来源：http://hz.aibaodan.cn/gtqzldbjey.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtnaaljzvf.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtafydlktk.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtwyeoazdh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigufen.top/gtbrtgyxsr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gtdgwlryxc.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtybdjjpxj.html

TS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtttsmelam.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gtmqvkzpnt.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gtipfnutlv.html

Ruby: arr[1, 3]
来源：http://hz.hammf.cn/gtyqxgebnd.html

C#:   list.GetRange(1, 3);
来源：http://hz.birdmap.top/gtubjegkkn.html

[D08] 合并两个数组
来源：http://hz.gzhubu.top/gtseyahilf.html

Py:   a + b;  a.extend(b)
来源：http://hz.ydzc1.top/gteuymfwey.html

PHP:  array_merge($a, $b);
来源：http://hz.c1oappe.top/gtlnhdcahz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gthjwvfilp.html

TS:   [...a, ...b];
来源：http://hz.haohaochexian.top/gtltndftnv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zycfv.cn/gthjuamhjz.html

Go:   append(a, b...)
来源：http://hz.cheryme.top/gtoxmqfexc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258.top/gtxscrngin.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtmyywccag.html

[D09] 排序（升序）
来源：http://hz.xuanzx.com/gtmetgjlyf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gthynvecko.html

PHP:  sort($arr);
来源：http://hz.smart0.xyz/gtuduxztqr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gotoacloud.top/gtskerwuvn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtdzvokzui.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtoqwtlixb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gttrpsanab.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtpleydxhp.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gthdsgeomo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.haohaochexian.top/gtewxjpmgo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtegpuovxa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtimstbfpc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtyrbearti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtzskshzue.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gtuvfdgpln.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ivvv.top/gtujokctyl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtsmroqupy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtsjinlmta.html

[D11] 反转数组
来源：http://hz.jianghu66.top/gtwinzbnmq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtfaynkrss.html

PHP:  array_reverse($arr);
来源：http://hz.chenzaomai.com/gtjhfjutve.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gturugoypi.html

TS:   [...arr].reverse();
来源：http://hz.cucudq.cn/gtqqqrcwdf.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtcwntglrz.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtjnbyqgrl.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtzugoiphm.html

C#:   list.Reverse();
来源：http://hz.yj202588.top/gtimeoznrx.html

[D12] 查找元素下标
来源：http://hz.jinqigufen.top/gtjwcgyrma.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gtxnpjqlyo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.316326.xyz/gtnjpunorc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtnlhvranc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtwouuvwxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtenqutuhh.html

Go:   slices.Index(arr, x)
来源：http://hz.yonumen.top/gtagowapiq.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtjkkdpemp.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigfzy.top/gtwbbdryer.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sufxvd.cn/gtqpuxjpeb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtmkuvgjwo.html


<!-- 参考信息 -->