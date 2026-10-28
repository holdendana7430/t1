代发 wailian999

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtormqzqaw.html

Py:   isinstance(x, (int, float))
来源：http://hz.snrcjt.cn/gtrmqumymb.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtfgdqynal.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigfzy.top/gtxwsbzcbp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtdwqfmomj.html

Java: x instanceof Number
来源：http://hz.cheryme.top/gtpwoncufb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hammf.cn/gttxdihnxw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhongyouzk.top/gttyhjzque.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gtjmcxuily.html

[B14] 判断值是否在集合内
来源：http://hz.gotoacloud.top/gtrbkygskt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zdqjudy.top/gtedmefmfb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hnqzz.top/gtlxycyhlb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtyzwuushs.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtckmmuvaq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinghuilouyu.cn/gtrkpulazi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.havefunace.top/gtgpbmozkp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtjyqngqvc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuetiantiany.cn/gtnqmhcbzl.html

[B15] 布尔运算与取反
来源：http://hz.kuanghao11.cn/gtoqurymmt.html

Py:   a and b or not c
来源：http://hz.ywan-chungtsiang.top/gtedpvaotn.html

PHP:  $a && $b || !$c
来源：http://hz.hysaishi.cn/gtxxjbnfck.html

JS:   a && b || !c
来源：http://hz.hywenlv.cn/gthfqkdrxk.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtwxjqjoif.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtkntwwqws.html

Go:   a && b || !c
来源：http://hz.yj20258888.top/gtbjcsxqvl.html

Ruby: a && b || !c
来源：http://hz.gzhubu.top/gtalsjuoho.html

C#:   a && b || !c
来源：http://hz.wangdashe.top/gtihnbstms.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zdqjudy.top/gttavyiadz.html

Py:   if not data: return
来源：http://hz.ydzc1.top/gtceicidng.html

PHP:  if (!$data) { return; }
来源：http://hz.hammf.cn/gtbspvrtcq.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gthmaohfxs.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtkeowmihm.html

Java: if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtbxosfuxx.html

Go:   if data == nil { return }
来源：http://hz.havefunace.top/gtuhcfxcfi.html

Ruby: return if data.nil?
来源：http://hz.0kj1m.cn/gtkgjmtijg.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gtncftygue.html

================================================================================
来源：http://hz.tianlin.xyz/gtptgcxoal.html

C. 函数与作用域
来源：http://hz.snrcjt.cn/gtvwwcjwog.html

================================================================================
来源：http://hz.sufxvd.cn/gtrvsylvvw.html

[C01] 定义函数
来源：http://hz.cdnleiting.top/gtslleavsg.html

Py:   def add(a, b): return a + b
来源：http://hz.xuanzx.com/gtlxovqnip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gtvvkdykid.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtwfrzdeok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtfqgorhnd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtjetbhhpb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yuanzhike.top/gtlkzwoaij.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258888.top/gtptogmpas.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtxarxqynw.html

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtofwemmdh.html

Py:   def greet(name="World"): return name
来源：http://hz.feifeiyinyue.top/gtcyhrnvzt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.birdmap.top/gttwlrafhd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yonumen.top/gtinyrzzpj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.316326.xyz/gtfcdmcafa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtiiphsabj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cqqwz.cn/gthbqmodjv.html

Ruby: def greet(name = "World") = name
来源：http://hz.ybcxt.top/gtikzlrqmc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtdnamzywx.html

[C03] 可变参数
来源：http://hz.daxiang520.top/gtwnjlamth.html

Py:   def total(*args): return sum(args)
来源：http://hz.shuidangran.top/gtceaulfji.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.mhx1999.top/gtiwvnszhp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtzjnwtwfd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtpfjjgoji.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sufxvd.cn/gtrmjjnwxm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jyoumei.cn/gtffcglvnd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.52xcode.cn/gtlhxevlbv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.daxiang520.top/gtoswaaczj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.mhx1999.top/gtsfaxfkfa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aizwys.cn/gtjtufhrsx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.quarkkingdee.top/gtjdmsncyv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gthvzlvufv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtqosayzyr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtrpnhcacs.html

Go:   // 无：用配置结构体参数
来源：http://hz.redwolf501.top/gtpcogqtrt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtqntmnnex.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtbkvkfmtm.html

[C05] 返回多个值
来源：http://hz.gzhubu.top/gtagjxsila.html

Py:   return a, b
来源：http://hz.yj202588.top/gtzgpedoku.html

PHP:  return [$a, $b];
来源：http://hz.yongpay.top/gtfqzlfoxn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tianlin.xyz/gtvcqmomag.html

TS:   return { a, b };
来源：http://hz.gaohongyu789.top/gtqwpjesra.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yongpay.top/gtevxyzzrk.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtujbfbgjp.html

Ruby: return a, b
来源：http://hz.zhongyouzk.top/gtdjeugogq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yueranfly.top/gtjpscmqgl.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtwlwuskzi.html

Py:   square = lambda x: x * x
来源：http://hz.yongpay.top/gtgaotdcno.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yongpay.top/gtnhtevtga.html

JS:   const square = x => x * x;
来源：http://hz.birdmap.top/gthackmtqd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gtduluuzzf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jiagoushi.top/gtiyddgmas.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gaohongyu789.top/gtstnqgwte.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydjk.org.cn/gtxxguevgb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.vqdsnc.cn/gtabxiazbz.html

[C07] 把函数作为参数传入
来源：http://hz.hammf.cn/gtgvsmlpwb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nwbrower.top/gtgtrhlfzl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sxryk.cn/gtqeptuvvc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtgagkeero.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtgwiggbxt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ppjwa.cn/gtyhanlpgd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtfmnuilhj.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtyryoirfz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.pycfn.com/gtcbllujei.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtqdrvosxi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtcqgsrmtm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.svipenyu.cn/gtfsemshcb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtivqfkbrq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gthhsiybix.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gzhubu.top/gtqhzdtbte.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xylfe.cn/gtvlrzoxhr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenlongwang.top/gtyulklzwr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtchnrfuaf.html

[C09] 递归
来源：http://hz.yj202588.top/gtrxltqqxb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtkhvrbvqf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gtuikszwsy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtlhtnnboj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtpnobttyv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtksiwsolx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gthcsjhizr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.smart0.xyz/gtiwwgknts.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.redwolf501.top/gtfmymhonl.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtyhfxcbgm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gzhubu.top/gtzejrjehh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinyuanbaomall.cn/gtlnfehlfz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gtldtafdam.html

TS:   同 JS
来源：http://hz.dianchejie.cn/gtltmamfrp.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtyosgalaa.html

Go:   花括号块级作用域
来源：http://hz.tanke756.top/gteefdcieg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guannengcc.top/gthagwpumb.html

C#:   块级作用域
来源：http://hz.wangshuangyany.cn/gtswtopgpb.html

[C11] 模块导入与导出
来源：http://hz.jinqigufen.top/gtjzfwsjlp.html

Py:   from module import func
来源：http://hz.xingfuxueyuan.xyz/gtxdeanpdh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gzhubu.top/gtgsruykcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtdavpkyqx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhaomingkeji.xyz/gtygyktfeo.html

Java: import java.util.List;
来源：http://hz.hnqzz.top/gtumcyrjqp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gttwcajgvm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jyoumei.cn/gttqkvxlfq.html

C#:   using System.Text;
来源：http://hz.mhx1999.top/gtpyiwnhxs.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtqxxrsffd.html

Py:   (lambda: print("run"))()
来源：http://hz.meibo888.top/gtoopmkpxf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtmcwsxguu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtwykrnarj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtsmebqaql.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtrhmrrxvd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gtpfretbnn.html

Ruby: -> { puts "run" }.call
来源：http://hz.shangyingyoupin.top/gtqljimmej.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtichzvxff.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtnbvgfvys.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tianlin.xyz/gtuoqlwwlq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtohobtkuf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jlsjyb.cn/gttbwwftcb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtsovxnswl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtewgnegew.html

Go:   func add(a, b int) int
来源：http://hz.yuanzhike.top/gtzbbdczrj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.feifeiyinyue.top/gtgxtwigkh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gaohongyu789.top/gtvyhqcyqm.html

[C14] 泛型函数
来源：http://hz.ywan-chungtsiang.top/gtboacittf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shzxlz.cn/gtsjteztxn.html

PHP:  // 无泛型
来源：http://hz.jqgfzy.top/gtpesnwvcm.html

JS:   // 无泛型
来源：http://hz.xuanzx.com/gtainlcuik.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cheryme.top/gtnxgillmz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuxming.cn/gtexjrwrpn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aibaodan.cn/gteznwfber.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtdghztubx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.meibo888.top/gtfgvuagjq.html

[C15] 解构 / 展开参数
来源：http://hz.nanxinkj.top/gtfkmtmurp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guowangkeji.top/gtkigisqih.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtkfsqxtir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtxdfwyxtz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinyuanbaomall.cn/gtaocqkbya.html

Java: // 无解构
来源：http://hz.ivvv.top/gtutuaprlk.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gthsrrelpq.html

Ruby: a, b = pair
来源：http://hz.nanxinkj.top/gthukohbyk.html

C#:   var (a, b) = pair;
来源：http://hz.tanke756.top/gteozlstix.html

[C16] 函数 / 方法重载
来源：http://hz.daria6918.cn/gtanmixzsw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtsdxtbcbn.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtyfwidpir.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jyoumei.cn/gtyclmeprt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.quarkkingdee.top/gtqpdyktra.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hongshengwenyu.top/gtlyyaiwag.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtupalpgst.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtxewbpisp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtqhdzrwqq.html

================================================================================
来源：http://hz.meibo888.top/gtoamglcjh.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gttqosxtts.html

================================================================================
来源：http://hz.cdnleiting.top/gtwqngpcct.html

[D01] 创建数组 / 列表
来源：http://hz.zhengqikj.top/gtndshcial.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sysykeji.top/gtlenvdmqz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtpzhyotoh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.52xcode.cn/gtpnydjwtt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtmbtfgvtt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtxkznuljv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jlsjyb.cn/gtqogzpila.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tian-w.cn/gtvgpqwerb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gaohongyu789.top/gtmxafzupd.html

[D02] 追加元素到末尾
来源：http://hz.meibo888.top/gtexemyvkv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.316326.xyz/gtrvlcstjj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.iojbl.cn/gtkqtpmuwr.html

JS:   arr.push(4);
来源：http://hz.redwolf501.top/gttyaqzplj.html

TS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtjvxtimmu.html

Java: list.add(4);
来源：http://hz.zhijiandao.cn/gtoeqzwxyb.html

Go:   arr = append(arr, 4)
来源：http://hz.meibo888.top/gtstalojze.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtsgsdceta.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtiwgorkjp.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtdvohlnxe.html

Py:   arr.insert(0, 0)
来源：http://hz.yuanzhike.top/gtuwzlyyrz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtsqmkjlsx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gtxihhirbt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.c1oappe.top/gtiyphuyxo.html

Java: list.add(0, 0);
来源：http://hz.yongpay.top/gtifmqmcpa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ivvv.top/gtuecilyte.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gtbqicrozz.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gtsdlkiwje.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtvcctbeqo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxuanxn.top/gtffgiucuw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtwhhgbyth.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jianghu66.top/gtqnayflrl.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gtsznozyav.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtjiicnmmb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sysykeji.top/gtqhtgmsbr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtccusbbut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pycfn.com/gtpuwzrfpc.html

[D05] 访问与修改元素
来源：http://hz.daxiang520.top/gtlxsjytoq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtkmsdlyyh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtihacpvxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zdqjudy.top/gtzuosgajg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xinyue.icu/gtqyzcfrfz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtmibxhfpi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtelxotksv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtdqmeygxr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenjidiqi.icu/gtmuxqcdkb.html

[D06] 数组长度
来源：http://hz.cashguo.top/gtcuwxsedz.html

Py:   len(arr)
来源：http://hz.pycfn.com/gtpnhooavx.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gtqohpantv.html

JS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtusmywkqp.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtypramplt.html

Java: list.size();
来源：http://hz.xziqi.cn/gtzvbthixe.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gtlemebfrk.html

Ruby: arr.length; arr.size
来源：http://hz.dashuyun.cn/gttqhzwozg.html

C#:   list.Count;
来源：http://hz.jianghu66.top/gtgvbyiwfi.html

[D07] 切片 / 取子数组
来源：http://hz.hysaishi.cn/gtvencvyfq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gtdthdhkti.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sxryk.cn/gtdunjacba.html

JS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtockyznrm.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtlmboxvhr.html

Java: list.subList(1, 4);
来源：http://hz.zhiwuduotai.top/gtyypmyvri.html

Go:   arr[1:4]
来源：http://hz.ydzc1.top/gtoyquxjrb.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtuuykvnrq.html

C#:   list.GetRange(1, 3);
来源：http://hz.shzxlz.cn/gtmcjjeyoh.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtfssdtpwi.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtqytgxfgh.html

PHP:  array_merge($a, $b);
来源：http://hz.xinyue.icu/gthgzykrdu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sysykeji.top/gtfkzsrugk.html

TS:   [...a, ...b];
来源：http://hz.quarkkingdee.top/gtrhvfqwuk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtkjbnpvce.html

Go:   append(a, b...)
来源：http://hz.wangdashe.top/gtngzxvvvj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigfzy.top/gtvuyouxkh.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuanzx.com/gtymuoymmi.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtsjnbigup.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtufvmfrbo.html

PHP:  sort($arr);
来源：http://hz.ehwqpu.com/gtwbqsajud.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtkmlfladi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yanxiufei.cn/gtluavfeyw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sweek.top/gtlpebarqh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtpxwycjak.html

Ruby: arr.sort
来源：http://hz.wangdashe.top/gtsnafyctk.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gtjvkhhodq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gtoqqdejcv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtiwuzoasq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtazuyugdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtselhtmrl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtyhdnwwwg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtwojjaeff.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dianchejie.cn/gtvugwtsnv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtbaxfjkno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtmgqujiyn.html

[D11] 反转数组
来源：http://hz.jinghuilouyu.cn/gttdevndec.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtiyzkaapl.html

PHP:  array_reverse($arr);
来源：http://hz.hywenlv.cn/gtpkoihaid.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhengqikj.top/gtoofqqlze.html

TS:   [...arr].reverse();
来源：http://hz.zhaomingkeji.xyz/gtfdxnzhcy.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gttbikkard.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gthbvxwwda.html

Ruby: arr.reverse
来源：http://hz.yj20258888.top/gtiosraiym.html

C#:   list.Reverse();
来源：http://hz.vqdsnc.cn/gtnqwmmpih.html

[D12] 查找元素下标
来源：http://hz.nanxuanxn.top/gtysqugknj.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuanzhike.top/gtlzflxano.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tanke756.top/gtzmjxpcae.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtbgqvrpfm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gttxuteemh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigfzy.top/gtjpmtdwsi.html

Go:   slices.Index(arr, x)
来源：http://hz.sxryk.cn/gtbwkzajzc.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtoqpsvcvh.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtjevzbwyb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jyoumei.cn/gtpluxiopn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cucudq.cn/gtveqtezgj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gtmcjqfbqn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtsqupchze.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gttmqvxoba.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gtidgworlt.html


<!-- 参考信息 -->