代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhijiandao.cn/gtcdmhcpzv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daxiang520.top/gtwwfsplth.html

[B11] 生成数字序列 / 区间
来源：http://hz.pycfn.com/gtiiprcrqz.html

Py:   list(range(0, 10, 2))
来源：http://hz.tianlin.xyz/gtrhebxhjw.html

PHP:  range(0, 10, 2);
来源：http://hz.andypj.xyz/gtcbmswoij.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtmfvocdry.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtbtlxtegv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gtmstickgo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xinyue.icu/gtjiiyvhfc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xinyue.icu/gtqgrdxdzh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtbqnjkdak.html

[B12] 跳出多层循环
来源：http://hz.ehwqpu.com/gtsmphhovm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jyoumei.cn/gtiiqcrjfj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtvmqljrmc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtjozjeyfy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtqcjjbxpz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtbdrsbnwp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cashguo.top/gteqtdsahh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenlongwang.top/gtcrsgjfpy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ybcxt.top/gtrgqtrovu.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtvagcpeqd.html

Py:   isinstance(x, (int, float))
来源：http://hz.birdmap.top/gtttantvmm.html

PHP:  is_numeric($x)
来源：http://hz.fzhhl.top/gtraydxvfl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtazonqdvn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gtepnzedaj.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtrjhvdqte.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gotoacloud.top/gtbkngcaqt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtyryxivtg.html

C#:   x is int or double or decimal
来源：http://hz.zhiwuduotai.top/gtirsyyvlz.html

[B14] 判断值是否在集合内
来源：http://hz.sxryk.cn/gtqdoanonb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gtencjlacm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gtfljlcqvk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtqcystlqe.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gttzqzcrbk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigfzy.top/gtncpecmpc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.fengsongda.top/gtmblmqsmr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fzhhl.top/gtjaysrvym.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hfpthk.cn/gtyapuvnrp.html

[B15] 布尔运算与取反
来源：http://hz.fengsongda.top/gtihyfxjwq.html

Py:   a and b or not c
来源：http://hz.zhixingplan.top/gtictablnj.html

PHP:  $a && $b || !$c
来源：http://hz.xinyue.icu/gtxaqakqpx.html

JS:   a && b || !c
来源：http://hz.birdmap.top/gthsuksjus.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtikmosall.html

Java: a && b || !c
来源：http://hz.haohaochexian.top/gturkpiqkk.html

Go:   a && b || !c
来源：http://hz.sxryk.cn/gthftgfzyi.html

Ruby: a && b || !c
来源：http://hz.gotoacloud.top/gtxtsmfywr.html

C#:   a && b || !c
来源：http://hz.yangfankeji.com/gtoqkislni.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dashuyun.cn/gtydimkeki.html

Py:   if not data: return
来源：http://hz.sxryk.cn/gttxebzeya.html

PHP:  if (!$data) { return; }
来源：http://hz.daxiang520.top/gtyjjzqmpf.html

JS:   if (!data) return;
来源：http://hz.redwolf501.top/gtnhzamezg.html

TS:   if (!data) return;
来源：http://hz.daria6918.cn/gtnapnlukk.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtbnaofpmq.html

Go:   if data == nil { return }
来源：http://hz.shanyushiyangtech.top/gtiomhrsyi.html

Ruby: return if data.nil?
来源：http://hz.vqdsnc.cn/gtklszqchd.html

C#:   if (data == null) return;
来源：http://hz.gzhubu.top/gtqksulsqu.html

================================================================================
来源：http://hz.cucudq.cn/gtqfpjlcnb.html

C. 函数与作用域
来源：http://hz.ybcxt.top/gtqkmetrrd.html

================================================================================
来源：http://hz.jinqigufen.top/gtcfupjtky.html

[C01] 定义函数
来源：http://hz.wangshuangyany.cn/gtpjazlqxp.html

Py:   def add(a, b): return a + b
来源：http://hz.zhengqikj.top/gtcbhrksmm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtqhljcpwu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gttiootfnm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtbyikglay.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtztclnufb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yuanzhike.top/gttumzlaug.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtdzlinqxj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtycpznsjg.html

[C02] 默认参数
来源：http://hz.daria6918.cn/gtptjflwsk.html

Py:   def greet(name="World"): return name
来源：http://hz.andypj.xyz/gtsgbdfjfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtsachqmgd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtjjonuzml.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.0kj1m.cn/gtwgcsrnti.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nwbrower.top/gtlnmawule.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinghuilouyu.cn/gtugnmsdts.html

Ruby: def greet(name = "World") = name
来源：http://hz.havefunace.top/gtdcwufpcs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.vqdsnc.cn/gtolphtluz.html

[C03] 可变参数
来源：http://hz.jinyuanbaomall.cn/gtzvsqlggm.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangkeji.top/gtjhabwyoh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gtuzcnnguh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtugdmxppj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gticoaaqlp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhongyouzk.top/gtcdhsxdrx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cucudq.cn/gtyltouedx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yvedp.cn/gttkperlvy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gtlpumdihs.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtesaiozja.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ppjwa.cn/gtbwebkvkb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gtnfpdopfc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhengqikj.top/gtttfnzayg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tianlin.xyz/gttnhdpogj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ppjwa.cn/gtdxslgrml.html

Go:   // 无：用配置结构体参数
来源：http://hz.havefunace.top/gtoylooidk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtedupthpz.html

C#:   f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gttmcwdmjn.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gtaaurbkpe.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtrncksrup.html

PHP:  return [$a, $b];
来源：http://hz.shuidangran.top/gtnldbfkjh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jianghu66.top/gtlvjdrfrh.html

TS:   return { a, b };
来源：http://hz.smart0.xyz/gtveduklrp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shzxlz.cn/gtytnjlgja.html

Go:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtfthcneln.html

Ruby: return a, b
来源：http://hz.zhaomingkeji.xyz/gtfzubusit.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnqzz.top/gtawgdapts.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtamphetiy.html

Py:   square = lambda x: x * x
来源：http://hz.cqqwz.cn/gtfpeqlkbg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.havefunace.top/gtzhexmrgv.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gtjdelotta.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtdodultqa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gteubblnix.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cqqwz.cn/gtlablqqes.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtxqqmklyw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shangyingyoupin.top/gtxtdwhdrk.html

[C07] 把函数作为参数传入
来源：http://hz.wangshuangyany.cn/gtgiyaeewk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhoulong.xyz/gtekszagnk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hysaishi.cn/gtepzbsuiz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guannengcc.top/gtzclmhrzl.html

TS:   arr.map(String)
来源：http://hz.52xcode.cn/gtlngagpfp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xylfe.cn/gtvituxqld.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuanzx.com/gtmkpzaxrx.html

Ruby: arr.map(&:upcase)
来源：http://hz.tian-w.cn/gtdrjwmcps.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.quarkkingdee.top/gtekpazbhg.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtgsawkswc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gtzgzpqvwm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nwbrower.top/gtrbjgakmi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gthzilwynu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtunvggzad.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tianlin.xyz/gthprmsiji.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fengsongda.top/gtzojjoxpo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gthgddxtfq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gttpthoqhf.html

[C09] 递归
来源：http://hz.pycfn.com/gtsasooduj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtnamozlyb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinghuilouyu.cn/gtibrjdmqc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gttyvjvsto.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtkskfwoqf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zycfv.cn/gtpsmbteqr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.316326.xyz/gtlqxyzydh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gtpplmopxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yongpay.top/gtrtbglfjy.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gterwrwslv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenjidiqi.icu/gthlbrpalr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtsbpfztrc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cdnleiting.top/gtqtbaptle.html

TS:   同 JS
来源：http://hz.zhijiandao.cn/gttqlhqohk.html

Java: 方法内为块级作用域
来源：http://hz.zdqjudy.top/gtjhalbdaq.html

Go:   花括号块级作用域
来源：http://hz.gaohongyu789.top/gtonyrsvdz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gthqkqrdnm.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtkhgonybc.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtctlruors.html

Py:   from module import func
来源：http://hz.ywan-chungtsiang.top/gtlypfolar.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.iojbl.cn/gtufcyaybo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtoaqtzugo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.birdmap.top/gtwtjfmoor.html

Java: import java.util.List;
来源：http://hz.ybcxt.top/gtklcnlyfw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtpymdxily.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.kuanghao11.cn/gtggmknxxy.html

C#:   using System.Text;
来源：http://hz.guannengcc.top/gtdpketxps.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtkednocvw.html

Py:   (lambda: print("run"))()
来源：http://hz.xuetiantiany.cn/gtrhgsrjue.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yanxiufei.cn/gtckmxkvhr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtnpkhrnah.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtyxjzaesf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258888.top/gtdauzphim.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj202588.top/gtoainqfti.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gtdgkxghmn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigufen.top/gtkcguauyk.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtpkhmkkso.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtcisnmjqh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtakfevqag.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtiolionpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtrrsarggl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtglbaenys.html

Go:   func add(a, b int) int
来源：http://hz.tian-w.cn/gtktveheyc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtifqtfdqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gtekpghprc.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gtmsscgrur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.fzhhl.top/gtjaxslcpt.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtunutynjr.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtvpwimhhd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.wangdashe.top/gtydzvbmya.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnxiangtu.top/gtsxcxesae.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.haohaochexian.top/gtbicisjbg.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtuadllifm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.52xcode.cn/gtrjwjicqd.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtcekmnxow.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtvuqcskqy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtknaxuslq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtkrdfvcze.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.snrcjt.cn/gtkcwgaobv.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtghsrrrlg.html

Go:   // 无解构
来源：http://hz.zhiwuduotai.top/gtyoskfden.html

Ruby: a, b = pair
来源：http://hz.jinghuilouyu.cn/gtmsudlffm.html

C#:   var (a, b) = pair;
来源：http://hz.jinghuilouyu.cn/gtxtrfgpxc.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtpjdytuyp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pycfn.com/gttpjcpuow.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtnafgxmix.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sweek.top/gtnezgvxxr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guannengcc.top/gtyeoikclz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shangyingyoupin.top/gtdednoztn.html

Go:   // 无重载：用不同函数名
来源：http://hz.sufxvd.cn/gtglzhaztz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtlvpagjrj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxuanxn.top/gtnpuvpxxr.html

================================================================================
来源：http://hz.hysaishi.cn/gtuexheclk.html

D. 数组 / 列表 / 集合
来源：http://hz.shuidangran.top/gttnasdozy.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthdtxlalx.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtvqerepdw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.feifeiyinyue.top/gtsindlyfr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gtdjnxijko.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.quarkkingdee.top/gtslqmugha.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtzunrzzyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhongyouzk.top/gtshgcdlhn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gtvrhcgsaj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtnrlzmjpf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangkeji.top/gtystyrokg.html

[D02] 追加元素到末尾
来源：http://hz.hysaishi.cn/gttlupqlrt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuanzhike.top/gtxesibihy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtxsnumatc.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtvvmpsnsl.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtwzqzitcm.html

Java: list.add(4);
来源：http://hz.yueranfly.top/gtqqhssxpy.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtuhqjxfrd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shuidangran.top/gtrduwpwmp.html

C#:   list.Add(4);
来源：http://hz.zhijiandao.cn/gtrvvktfek.html

[D03] 在指定位置插入元素
来源：http://hz.yueranfly.top/gtbmitajwv.html

Py:   arr.insert(0, 0)
来源：http://hz.bjfxy.top/gtntorswnx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.mhx1999.top/gtpgvcuexf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gtbiepfugg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gtaxgvcryp.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtccllesbk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtudygoely.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtncixcyph.html

C#:   list.Insert(0, 0);
来源：http://hz.316326.xyz/gtnfnlbfqn.html

[D04] 删除元素
来源：http://hz.ivvv.top/gtsegbnhzg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.9152youxi.cn/gtzpgfyrht.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gtgmsvgmbf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtajvpfril.html

TS:   arr.splice(0, 1);
来源：http://hz.smart0.xyz/gtzkqfxcmq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtkotjkmgs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenzaomai.com/gtswmkxtpc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtqsrqssnw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigfzy.top/gtsljhxfbe.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtzlenvctq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtbhteqmsa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.52xcode.cn/gtfevcpzvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtkidqcaqg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtnjtadcht.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sxryk.cn/gtxzpnycfm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.316326.xyz/gtlpprwtob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtatgvewsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.mhx1999.top/gtdkssjvat.html

[D06] 数组长度
来源：http://hz.dashuyun.cn/gtezknzcnp.html

Py:   len(arr)
来源：http://hz.gotoacloud.top/gttmxdyjyk.html

PHP:  count($arr);
来源：http://hz.cashguo.top/gtrxrzzlml.html

JS:   arr.length
来源：http://hz.zhijiandao.cn/gtmqvypghy.html

TS:   arr.length
来源：http://hz.meibo888.top/gtmphqzrrw.html

Java: list.size();
来源：http://hz.hnqzz.top/gtvhxivrqk.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gtjxtwfegu.html

Ruby: arr.length; arr.size
来源：http://hz.zhoulong.xyz/gtuuacijxl.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtehknixcb.html

[D07] 切片 / 取子数组
来源：http://hz.daria6918.cn/gtrfsyntsz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtkqbuvrlt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gtbebihhmv.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtegvtaoef.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtnrdsltsh.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtnybbgayg.html

Go:   arr[1:4]
来源：http://hz.dianchejie.cn/gtewemarbj.html

Ruby: arr[1, 3]
来源：http://hz.hongshengwenyu.top/gttiejxubd.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxuanxn.top/gtpinveukk.html

[D08] 合并两个数组
来源：http://hz.ivvv.top/gtqfznhvny.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtmfgijhaj.html

PHP:  array_merge($a, $b);
来源：http://hz.yongpay.top/gtnuggycwb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zdqjudy.top/gtuheaspau.html

TS:   [...a, ...b];
来源：http://hz.fzhhl.top/gtektcrssp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shzxlz.cn/gtqcrlbmaz.html

Go:   append(a, b...)
来源：http://hz.yj202588.top/gtbrtuwthj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtdahomzvx.html

C#:   a.Concat(b).ToList()
来源：http://hz.jlsjyb.cn/gtbprmzbdl.html

[D09] 排序（升序）
来源：http://hz.dianchejie.cn/gtxcsapblh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gthafsvisd.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtibhstrys.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gotoacloud.top/gtddhqwvjn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yongpay.top/gtxelalmth.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtnqifmcwr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shuidangran.top/gtuxzaivsc.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtbgbckopg.html

C#:   list.Sort();
来源：http://hz.pycfn.com/gtrnhtngsj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.meibo888.top/gtwtkgiutq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtvdcxwaxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tian-w.cn/gtcugfsnli.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtvnyypxxz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtfmsycwmm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gttvvzfyfs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtxkvtmelo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtbpxycstp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gaohongyu789.top/gtlnlseaqn.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtedneratd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.mhx1999.top/gtgkcnzpez.html

PHP:  array_reverse($arr);
来源：http://hz.zhoulong.xyz/gtopwnkntb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gzhubu.top/gtswvxyxwb.html


<!-- 参考信息 -->