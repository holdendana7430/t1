代发 wailian999

[B13] 判断是否为数字
来源：http://hz.hongshengwenyu.top/gtjkjrlamv.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenzaomai.com/gtbezawwbx.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtvwhmixng.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtasyqimmu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtmeijirhc.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtntfgpicy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtbkxusxau.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangdashe.top/gtwcyexuav.html

C#:   x is int or double or decimal
来源：http://hz.wangdashe.top/gtheemnleh.html

[B14] 判断值是否在集合内
来源：http://hz.ydzc1.top/gtklgqlozn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigufen.top/gtcohohdmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hongshengwenyu.top/gtmfnwttiv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gttahcyaad.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtakwsgymy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnqzz.top/gtkxvgcvrz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shangyingyoupin.top/gtzvzodzan.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jianghu66.top/gtneplrjam.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhoulong.xyz/gtwffxzesm.html

[B15] 布尔运算与取反
来源：http://hz.52xcode.cn/gtpvrtykpy.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gtwuhyspgd.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigfzy.top/gtlmtquzrw.html

JS:   a && b || !c
来源：http://hz.haohaochexian.top/gtsvdtslbm.html

TS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtarbvymmh.html

Java: a && b || !c
来源：http://hz.jqgufenzy.top/gthsytrkar.html

Go:   a && b || !c
来源：http://hz.yangfankeji.com/gtbwgdakyg.html

Ruby: a && b || !c
来源：http://hz.zhijiandao.cn/gtcazxrpny.html

C#:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtcctjgsgl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinghuilouyu.cn/gtnxequfhh.html

Py:   if not data: return
来源：http://hz.wangshuangyany.cn/gtyyfaxque.html

PHP:  if (!$data) { return; }
来源：http://hz.fengsongda.top/gtsfqfcguv.html

JS:   if (!data) return;
来源：http://hz.tanke756.top/gtdgroeihq.html

TS:   if (!data) return;
来源：http://hz.yongpay.top/gtwypbzwuf.html

Java: if (data == null) return;
来源：http://hz.yuanzhike.top/gtfszpbvuj.html

Go:   if data == nil { return }
来源：http://hz.andypj.xyz/gtiwmruosf.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtmnlqmoxa.html

C#:   if (data == null) return;
来源：http://hz.yonumen.top/gtcvanibls.html

================================================================================
来源：http://hz.havefunace.top/gtbtzweavb.html

C. 函数与作用域
来源：http://hz.xinyue.icu/gtdvlziahx.html

================================================================================
来源：http://hz.chenlongwang.top/gtgdeajjmm.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gtaqegebyo.html

Py:   def add(a, b): return a + b
来源：http://hz.shzxlz.cn/gtkvwlzkle.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gthgmoccui.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtgmsjuzwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtjdpjbsan.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtfvupynev.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigufen.top/gtvdfzwzsw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tanke756.top/gtneygvqwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtajalagdw.html

[C02] 默认参数
来源：http://hz.daria6918.cn/gtpjfyftjs.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgufenzy.top/gtvyycjyyf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtjosubohz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtpghkmdxm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.52xcode.cn/gtjspofyxh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtojdcptum.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhongyouzk.top/gtsgxeoalh.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gtamhrjjyb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yanxiufei.cn/gtkueregfd.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtwgwkepxw.html

Py:   def total(*args): return sum(args)
来源：http://hz.cheryme.top/gtohaqvopm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sweek.top/gtttxbidxf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtyvfwagtq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtdditthpn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.bjfxy.top/gthsxidfrt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ydzc1.top/gtxhykvumb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinyuanbaomall.cn/gtrlwbeaad.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shzxlz.cn/gtpgiukgcv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.haohaochexian.top/gtogqheism.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhoulong.xyz/gtrlegcfji.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.snrcjt.cn/gthnyellhf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xylfe.cn/gthhtsksch.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtdlcruzwr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.iojbl.cn/gtnjaurgiu.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gteugstjne.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtrkryyslq.html

C#:   f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtdgoqdblk.html

[C05] 返回多个值
来源：http://hz.hysaishi.cn/gtownkxpav.html

Py:   return a, b
来源：http://hz.gotoacloud.top/gtgdkjlrie.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtskkqykhw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fengsongda.top/gtrrufpuxq.html

TS:   return { a, b };
来源：http://hz.hfpthk.cn/gtlocvibre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhongyouzk.top/gtwevsgbcf.html

Go:   return a, b
来源：http://hz.birdmap.top/gthdbmrsvu.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtwbfdhswl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.andypj.xyz/gtxiqeiimj.html

[C06] 匿名函数 / lambda
来源：http://hz.316326.xyz/gtlntcqdkk.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtawrdohxk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yanxiufei.cn/gtxctzfeui.html

JS:   const square = x => x * x;
来源：http://hz.ydjk.org.cn/gtatjgcsjf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtbsjreebs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gzhubu.top/gtmzqbqaam.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuanzx.com/gtbmpgkddj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gtgwfkkaox.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.0kj1m.cn/gtmcfdecyt.html

[C07] 把函数作为参数传入
来源：http://hz.hnqzz.top/gtubjbtzwi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yonumen.top/gtjwcybrno.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtbjxtcwqd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.pycfn.com/gtdaivcrxo.html

TS:   arr.map(String)
来源：http://hz.sweek.top/gtuiswbwgb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hammf.cn/gtqcvkomgw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtftngdial.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtbzeiatid.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtjhrztcor.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtlpcfiisf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtfakngqep.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtncpdoyjb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtnybbhssg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtbyzcqbzt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydzc1.top/gtoaasmtpu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jlsjyb.cn/gtldpbelce.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtwidkjbkf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtprqpoqxa.html

[C09] 递归
来源：http://hz.yangfankeji.com/gtpjjuywfu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gthtolcgof.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jyoumei.cn/gtvahrraaa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gthjjogeud.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtoebcvegm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhongyouzk.top/gtlgjpnawo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtwpnwvqwv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtnzpooyiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtjmoxczhv.html

[C10] 变量作用域
来源：http://hz.cdnleiting.top/gtwanbmgoe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtrljjmrcp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gogol.net.cn/gtguaufkmy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuetiantiany.cn/gtjqauuibk.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtpysjkuyp.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gthjvbmswj.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtgfhauuyf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhengqikj.top/gtfnkeevsu.html

C#:   块级作用域
来源：http://hz.zhixingplan.top/gtywnftvkk.html

[C11] 模块导入与导出
来源：http://hz.nanxinkj.top/gtnzbawedl.html

Py:   from module import func
来源：http://hz.ehwqpu.com/gtidqqujnf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.c1oappe.top/gtiwjczlqa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtbkkuartx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gtfqxqzbvq.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtdfbwszhq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gtauvxmrfz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xinyue.icu/gtdkbqkpkv.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gtccoqsjdm.html

[C12] 立即执行函数 IIFE
来源：http://hz.gotoacloud.top/gtcsiqudhr.html

Py:   (lambda: print("run"))()
来源：http://hz.ydjk.org.cn/gtdvykavyv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinghuilouyu.cn/gtlpamjjny.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtxthqdysu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtxawpryzi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtxexfcdpt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtvrxbpsae.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxinkj.top/gtnxzfgwww.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhoulong.xyz/gtdtcxbeko.html

[C13] 类型声明 / 类型注解
来源：http://hz.pengpengdd.cyou/gttypkcbcj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zdqjudy.top/gturnsqgjx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtcmxtnibb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hysaishi.cn/gtuuqofcrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtcscpofsl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtbwdyqklx.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtqjgneucd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhiwuduotai.top/gtiaurvxpm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtvydqheus.html

[C14] 泛型函数
来源：http://hz.shangyingyoupin.top/gtguqlypep.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangshuangyany.cn/gtejuslivs.html

PHP:  // 无泛型
来源：http://hz.tian-w.cn/gtxmwrwhqc.html

JS:   // 无泛型
来源：http://hz.jiagoushi.top/gtonzmdlby.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxuanxn.top/gthicwdxcq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.316326.xyz/gtzepzvixl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtckbrklhs.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtllihvejb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.kuanghao11.cn/gtgcchlzyx.html

[C15] 解构 / 展开参数
来源：http://hz.tanke756.top/gtdxayvgft.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigfzy.top/gtwggejgfk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtntgjyres.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cdnleiting.top/gtkiaurksj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydzc1.top/gtyyezfdzt.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtobhpldwf.html

Go:   // 无解构
来源：http://hz.fengsongda.top/gtwsndavmh.html

Ruby: a, b = pair
来源：http://hz.zhixingplan.top/gtxzrlclaq.html

C#:   var (a, b) = pair;
来源：http://hz.ydjk.org.cn/gtjkjivncn.html

[C16] 函数 / 方法重载
来源：http://hz.aizwys.cn/gtjeykwxqk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.c1oappe.top/gtgzpukdsv.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtderogkev.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cucudq.cn/gtyffzzuxn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xinyue.icu/gtjlcdtvnf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jlsjyb.cn/gtnxuxaarv.html

Go:   // 无重载：用不同函数名
来源：http://hz.fengsongda.top/gtvvllzeph.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtrtiogytl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aibaodan.cn/gteybjkovn.html

================================================================================
来源：http://hz.guowangkeji.top/gtzusfciwp.html

D. 数组 / 列表 / 集合
来源：http://hz.fengsongda.top/gtynlujnpg.html

================================================================================
来源：http://hz.dashuyun.cn/gtxmniujkw.html

[D01] 创建数组 / 列表
来源：http://hz.zhixingplan.top/gtbthmxcrp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cashguo.top/gtniyicavk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yonumen.top/gtunnmgsfr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ppjwa.cn/gtiiwxxmsm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangdashe.top/gtibpiwahg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daria6918.cn/gtbgnpythm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.iojbl.cn/gthokzzswn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtnjtxxzoz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtbxwbbitn.html

[D02] 追加元素到末尾
来源：http://hz.jinqigufen.top/gtpxzqysvf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jyoumei.cn/gtzlfkiwcy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtxlrvdrwc.html

JS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtfcujwwdo.html

TS:   arr.push(4);
来源：http://hz.ybcxt.top/gtthgpfqbk.html

Java: list.add(4);
来源：http://hz.hfpthk.cn/gtjoukhmzf.html

Go:   arr = append(arr, 4)
来源：http://hz.guowangkeji.top/gtawpnqsbx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtsffyzbdl.html

C#:   list.Add(4);
来源：http://hz.aibaodan.cn/gtflkthcqx.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gtrxpqslsl.html

Py:   arr.insert(0, 0)
来源：http://hz.pycfn.com/gtcnfzykgh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuxming.cn/gtmoryojpd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtgarlropb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gtqwmqjhvc.html

Java: list.add(0, 0);
来源：http://hz.snrcjt.cn/gtwlpuxgde.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xziqi.cn/gtuvcjewta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinghuilouyu.cn/gttpbsnpxn.html

C#:   list.Insert(0, 0);
来源：http://hz.wangshuangyany.cn/gtjzkqmhil.html

[D04] 删除元素
来源：http://hz.sufxvd.cn/gtazipziya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hammf.cn/gtdvmxnuav.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258.top/gtpfxbcxje.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shuidangran.top/gtvqlfzsxj.html

TS:   arr.splice(0, 1);
来源：http://hz.hnxiangtu.top/gtbkbccecu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ehwqpu.com/gtgzcekhpf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtgxmxqquy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hysaishi.cn/gtjplwcdju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinyuanbaomall.cn/gtlhnziirl.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gtjpmecmwa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtzfyammwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtwwjquckz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtytdeqbbw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pycfn.com/gtkwmmeqlw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yonumen.top/gtfraxjlxj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtgkoscebb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtktvkjpap.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtxbzksoad.html

[D06] 数组长度
来源：http://hz.shanyushiyangkeji.top/gttowkhdfh.html

Py:   len(arr)
来源：http://hz.sufxvd.cn/gtdbiktsex.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtyetggifz.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtrqpulquj.html

TS:   arr.length
来源：http://hz.52xcode.cn/gtqwuxgifd.html

Java: list.size();
来源：http://hz.ywan-chungtsiang.top/gtzlsggjbg.html

Go:   len(arr)
来源：http://hz.yonumen.top/gtezacbtfc.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtryxvzymm.html

C#:   list.Count;
来源：http://hz.zhijiandao.cn/gtgavcmmmp.html

[D07] 切片 / 取子数组
来源：http://hz.xinyue.icu/gtufporyki.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtmigtwwdt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gtvhftksmv.html

JS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtgvrxcsfg.html

TS:   arr.slice(1, 4);
来源：http://hz.aizwys.cn/gtqvguawbm.html

Java: list.subList(1, 4);
来源：http://hz.tian-w.cn/gtgvrmayxr.html

Go:   arr[1:4]
来源：http://hz.chenzaomai.com/gthzlsvxtb.html

Ruby: arr[1, 3]
来源：http://hz.pycfn.com/gtsgqgitok.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuanzx.com/gtzwzvwbwb.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtcyrjowam.html

Py:   a + b;  a.extend(b)
来源：http://hz.52xcode.cn/gtpxingtco.html

PHP:  array_merge($a, $b);
来源：http://hz.wangshuangyany.cn/gtmifshfgp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtbkapwlnh.html

TS:   [...a, ...b];
来源：http://hz.guowangkeji.top/gtzsssrwig.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cdnleiting.top/gtzjinmdns.html

Go:   append(a, b...)
来源：http://hz.zhaomingkeji.xyz/gtnjbntrxa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gtzihtfwpw.html

C#:   a.Concat(b).ToList()
来源：http://hz.vqdsnc.cn/gtelogwdgw.html

[D09] 排序（升序）
来源：http://hz.zhongyouzk.top/gtdeagdmzb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtcdelxmzj.html

PHP:  sort($arr);
来源：http://hz.nanxuanxn.top/gtzvscsqij.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fengsongda.top/gtfbedgwnf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtuhxtyfix.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gogol.net.cn/gtrcyjgyis.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtcoiqsegk.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtokwfnoqg.html

C#:   list.Sort();
来源：http://hz.xinyue.icu/gtccxxaxoz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yvedp.cn/gtctzcyxgp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuanzx.com/gtyfgvkrju.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtemewhojd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtgixpakxe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gttxmilknq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ivvv.top/gtxnknplyr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinghuilouyu.cn/gtxxummmeu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtqjgehllf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gogol.net.cn/gtfswonjjr.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gtlgmdbgcc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yvedp.cn/gttnjcfyfk.html

PHP:  array_reverse($arr);
来源：http://hz.gzhubu.top/gtzpeeujog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gtbkvxklwf.html

TS:   [...arr].reverse();
来源：http://hz.sxryk.cn/gtcqpzkgzz.html

Java: Collections.reverse(list);
来源：http://hz.shangyingyoupin.top/gtokqzextm.html

Go:   slices.Reverse(arr)
来源：http://hz.havefunace.top/gticozayes.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gtqznziwfc.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtkuzmcwjh.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gtbcgdxtox.html

Py:   arr.index(x);  x in arr
来源：http://hz.snrcjt.cn/gtnkwgquut.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pycfn.com/gtminnbpzs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.316326.xyz/gtbntldxom.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gthozmjxfd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtfzyngeai.html

Go:   slices.Index(arr, x)
来源：http://hz.9152youxi.cn/gthwfnjqod.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtocmsliwn.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtmwiqymcb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtshtcqeiu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.iojbl.cn/gtlwznecbe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtylmvvtsd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtnqnotesj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtnfuclbdu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtovmwlexg.html


<!-- 参考信息 -->