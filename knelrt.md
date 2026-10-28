代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.9152youxi.cn/gtzfbagype.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zycfv.cn/gthxzdyqlu.html

[B11] 生成数字序列 / 区间
来源：http://hz.tanke756.top/gtfzptxcja.html

Py:   list(range(0, 10, 2))
来源：http://hz.guannengcc.top/gtbxczupmn.html

PHP:  range(0, 10, 2);
来源：http://hz.yongpay.top/gtijvxaseh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cdnleiting.top/gtnuahcqjq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtjwhhocel.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigfzy.top/gtgmcjmbgu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shanyushiyangkeji.top/gtxtnemkbk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.9152youxi.cn/gtewiyfrwz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dianchejie.cn/gtctrprxxn.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtuvukiahw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gaohongyu789.top/gtlegqjtco.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guannengcc.top/gtmqmkqqjz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtvltvrevw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtntawzrkw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtqgysakjw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnxiangtu.top/gtyjyqhqkl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yangfankeji.com/gtdsczzdkj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yanxiufei.cn/gtyzpeimzh.html

[B13] 判断是否为数字
来源：http://hz.dashuyun.cn/gtsdewhmjs.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gthbttrwdh.html

PHP:  is_numeric($x)
来源：http://hz.jinyuanbaomall.cn/gtxcbreeme.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtiqzwuosa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangdashe.top/gtervvvgkb.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gtrgecgfon.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.meibo888.top/gtgdicnset.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hysaishi.cn/gtvfhihxyj.html

C#:   x is int or double or decimal
来源：http://hz.chenlongwang.top/gtkfdlgepm.html

[B14] 判断值是否在集合内
来源：http://hz.yvedp.cn/gtyguppbkm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.fengsongda.top/gtainrrpjm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ywan-chungtsiang.top/gtbanbczyd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shzxlz.cn/gtwlzgvjzp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtlgzmhulh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhoulong.xyz/gtlwmxdqlq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gtdlkzhaup.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinqigfzy.top/gtwlowohur.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtiyuhejud.html

[B15] 布尔运算与取反
来源：http://hz.xuanzx.com/gtnwlwuwnp.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtfvdjyber.html

PHP:  $a && $b || !$c
来源：http://hz.shanyushiyangtech.top/gtnwacprso.html

JS:   a && b || !c
来源：http://hz.yonumen.top/gtwzbgfjek.html

TS:   a && b || !c
来源：http://hz.yj20258888.top/gtdmhsjboc.html

Java: a && b || !c
来源：http://hz.shangyingyoupin.top/gtmzdelajd.html

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtsuvgwbpp.html

Ruby: a && b || !c
来源：http://hz.snrcjt.cn/gtwyewyvyp.html

C#:   a && b || !c
来源：http://hz.yonumen.top/gtxdjtoozw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gteidkmhnq.html

Py:   if not data: return
来源：http://hz.redwolf501.top/gttdokmzra.html

PHP:  if (!$data) { return; }
来源：http://hz.sweek.top/gtsoguyggb.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtyfwfntft.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtmukfcrgz.html

Java: if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtqcyqymzc.html

Go:   if data == nil { return }
来源：http://hz.fengsongda.top/gtnjqkpbbo.html

Ruby: return if data.nil?
来源：http://hz.jqgufenzy.top/gtzytmfrea.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtgdludnvj.html

================================================================================
来源：http://hz.zhijiandao.cn/gthhuhclbb.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtpsohzexr.html

================================================================================
来源：http://hz.dianchejie.cn/gtoylfslkn.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtzczfbtqg.html

Py:   def add(a, b): return a + b
来源：http://hz.guowangkeji.top/gtjymhioze.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtkjawaqpn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.dashuyun.cn/gtzgsgsvti.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtftjhigzl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtsbztwixg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtjgkxzjvw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.kuanghao11.cn/gtlkkvjfqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtyiovznjj.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtbrutfekk.html

Py:   def greet(name="World"): return name
来源：http://hz.hnqzz.top/gtolqeytwo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtztlmjxoz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.guannengcc.top/gtctsqgtuh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtfrlpprza.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jyoumei.cn/gtdddredar.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daria6918.cn/gtujxkpysv.html

Ruby: def greet(name = "World") = name
来源：http://hz.hywenlv.cn/gtmuppjmmo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guannengcc.top/gtvjkllhxu.html

[C03] 可变参数
来源：http://hz.vqdsnc.cn/gtrcuupxeq.html

Py:   def total(*args): return sum(args)
来源：http://hz.ppjwa.cn/gtmzzbbmag.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenlongwang.top/gtezucshvh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtqahkzvsh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtzlkoupxr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cheryme.top/gtrlzdbinq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinyuanbaomall.cn/gtfibocpvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cucudq.cn/gtkxxatzaf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gthbjumpfc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtchamafhi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.snrcjt.cn/gtlbdfhwer.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuanzhike.top/gtkkunwmtn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtkswuuuom.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtujlhsntv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jyoumei.cn/gtycplagwy.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gttaxvhedk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtgkaxhbwq.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtyllglsmp.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtgrzxriwv.html

Py:   return a, b
来源：http://hz.ydjk.org.cn/gtflelutkl.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gticilmssh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hongshengwenyu.top/gtfuenfgzu.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtranphgpt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cashguo.top/gtxslhyumk.html

Go:   return a, b
来源：http://hz.zhixingplan.top/gttmkkihkm.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gthytwcxoi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yvedp.cn/gtasiectvh.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtsuxeuhdn.html

Py:   square = lambda x: x * x
来源：http://hz.nanxinkj.top/gthknwqdxp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gtfwbzvaaw.html

JS:   const square = x => x * x;
来源：http://hz.hysaishi.cn/gtjdllfdoi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gttqaowpwd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hywenlv.cn/gtdkloukwz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtxduvpglv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xylfe.cn/gtqlzfhngg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gotoacloud.top/gtwmnvpmfx.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangtech.top/gtgpuybupp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yvedp.cn/gtalxcmhpk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yueranfly.top/gtetazjzrl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cheryme.top/gthkrhbmot.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtpecukbsj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtqcvmbfps.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtuqwxfcdk.html

Ruby: arr.map(&:upcase)
来源：http://hz.pycfn.com/gtdfqkedsw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zycfv.cn/gtdgonrvod.html

[C08] 闭包
来源：http://hz.chenzaomai.com/gtcygkrvhg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.birdmap.top/gtwxobyrkt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigfzy.top/gtreadwdrw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtzlcdjwzm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtbsrxgnwm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.52xcode.cn/gtpfvthuov.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gtwxoqnvxv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cashguo.top/gtxsarjkvc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtzwwdexbu.html

[C09] 递归
来源：http://hz.guowangkeji.top/gtfjjgdybg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtxocansca.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtrxcfsygn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtlpdttbic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtgejryfmz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuetiantiany.cn/gtkmexsndf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guannengcc.top/gtvignhobv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aizwys.cn/gtgpmubtxr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangtech.top/gtlemkhsbv.html

[C10] 变量作用域
来源：http://hz.vqdsnc.cn/gtuacoixmv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtxunmkxlp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangkeji.top/gtwrllrusk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhiwuduotai.top/gtjhnlujql.html

TS:   同 JS
来源：http://hz.yanxiufei.cn/gtzpkqfbih.html

Java: 方法内为块级作用域
来源：http://hz.tianlin.xyz/gtkgwosbay.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtzddxrbkd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuanzx.com/gtvmpuqkym.html

C#:   块级作用域
来源：http://hz.ydjk.org.cn/gtngszqhnp.html

[C11] 模块导入与导出
来源：http://hz.yuxming.cn/gtaiypamlh.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtdtmkpgqy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258888.top/gtenxsmxyh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangdashe.top/gtpfntuavh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.meibo888.top/gtsdwatluc.html

Java: import java.util.List;
来源：http://hz.316326.xyz/gtxumsatpz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtedosrhma.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtidhmjhex.html

C#:   using System.Text;
来源：http://hz.52xcode.cn/gtffedkjxh.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtlhbpexbg.html

Py:   (lambda: print("run"))()
来源：http://hz.hysaishi.cn/gtywylzdrc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zdqjudy.top/gtckjysuqy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtqhdfqnko.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtmutlxvwd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtkgwpscqj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuetiantiany.cn/gthnqqffid.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gtilkffcnf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yangfankeji.com/gtgtpjgfzg.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtgytqtclr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gtkwmhkigg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtujrsmtjx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtngmtqhsf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtthxxuwui.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtvbuiyjhw.html

Go:   func add(a, b int) int
来源：http://hz.yanxiufei.cn/gtzuhbqoii.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cheryme.top/gtptwkrwnh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtwgvvqxsd.html

[C14] 泛型函数
来源：http://hz.fengsongda.top/gthqklbvhj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhoulong.xyz/gtozsnwjao.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtapazykvv.html

JS:   // 无泛型
来源：http://hz.shuidangran.top/gtiqwlhifa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cqqwz.cn/gthfeqeian.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jianghu66.top/gthrqtpqjj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cucudq.cn/gterciopkv.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtwdrwcqct.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gzhubu.top/gtyffwhamk.html

[C15] 解构 / 展开参数
来源：http://hz.guannengcc.top/gtjetbflln.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtraldzneu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.havefunace.top/gtiwkzqthf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtmdwntlse.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangtech.top/gtgkfwcsii.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtxlkwagmn.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtzlrgotei.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gtovjddjcy.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtxssrcptx.html

[C16] 函数 / 方法重载
来源：http://hz.chenzaomai.com/gtdnzbnkgw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtgfbljpml.html

PHP:  // 无重载
来源：http://hz.ywan-chungtsiang.top/gthpnleznc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtutrxirlo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgufenzy.top/gtwlyopysr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gttjshdsvt.html

Go:   // 无重载：用不同函数名
来源：http://hz.gaohongyu789.top/gtnpguewub.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daxiang520.top/gtocqfspec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.c1oappe.top/gtwroohkjb.html

================================================================================
来源：http://hz.birdmap.top/gtjnhgmaer.html

D. 数组 / 列表 / 集合
来源：http://hz.sxryk.cn/gtannyzbrq.html

================================================================================
来源：http://hz.kuanghao11.cn/gtycsmgasc.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtjfnbxozw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtvtdwmopz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.snrcjt.cn/gttzwfvyio.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtirfuzoqa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnqzz.top/gtcjzyuwqf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtapcvqxcy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ivvv.top/gtdsgkxxzx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuanzhike.top/gtguywuzhh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.52xcode.cn/gtvfoecavh.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gtnurapsku.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhixingplan.top/gttnczwivd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtyybydsnl.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtlfuzqiel.html

TS:   arr.push(4);
来源：http://hz.tanke756.top/gtnxckmiys.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtubszjfhq.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gtncwkqxlm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.meibo888.top/gtfvxmymkr.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtkmgggcbr.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gticaivqym.html

Py:   arr.insert(0, 0)
来源：http://hz.meibo888.top/gttnuxaxgg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gotoacloud.top/gtggorvxop.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hywenlv.cn/gtqhzhnqbk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinyuanbaomall.cn/gtsjjjlewc.html

Java: list.add(0, 0);
来源：http://hz.yuanzhike.top/gtnylewfly.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.svipenyu.cn/gtiqhrpprs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhijiandao.cn/gtnzscceih.html

C#:   list.Insert(0, 0);
来源：http://hz.snrcjt.cn/gttlexerba.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gtwwfsgwwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgfzy.top/gtxxusziub.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gtbpftywri.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tanke756.top/gtaawggpaj.html

TS:   arr.splice(0, 1);
来源：http://hz.kuanghao11.cn/gttsqeylkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aizwys.cn/gtwdjwozub.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gteqlyrnxz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hfpthk.cn/gtarcpfewo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jlsjyb.cn/gtvdxunoap.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtubwcxfse.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtancubhgf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.bjfxy.top/gtqrnbdckv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daria6918.cn/gteazdvbyk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.haohaochexian.top/gtyxjfvscf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.quarkkingdee.top/gtvaqpugor.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtrbicnsyq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtcwdmenql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gtrezdeaqo.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtnndawvst.html

Py:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtraihhjgg.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtoncxvofe.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gtdmazcdcf.html

TS:   arr.length
来源：http://hz.xziqi.cn/gtvmnfcwkr.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtokxklnpp.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gtvmsvgigx.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gtwsolmjzl.html

C#:   list.Count;
来源：http://hz.wangdashe.top/gtxvrgdcmi.html

[D07] 切片 / 取子数组
来源：http://hz.svipenyu.cn/gtopodsawp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gtwkzjixbq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.kuanghao11.cn/gtnuyxaomk.html

JS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gtghqdncza.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtgcgbqqcm.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtdiqtloro.html

Go:   arr[1:4]
来源：http://hz.bjfxy.top/gtbtsoxpba.html

Ruby: arr[1, 3]
来源：http://hz.hnqzz.top/gtbwfezqon.html

C#:   list.GetRange(1, 3);
来源：http://hz.ehwqpu.com/gtqxbotndm.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtlhngrxac.html

Py:   a + b;  a.extend(b)
来源：http://hz.svipenyu.cn/gttshvvfho.html

PHP:  array_merge($a, $b);
来源：http://hz.ydjk.org.cn/gtkuargusq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.haohaochexian.top/gtneikihfx.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gtviejnexu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtapalgyjz.html

Go:   append(a, b...)
来源：http://hz.yvedp.cn/gtcutklutw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gtzbixspvq.html

C#:   a.Concat(b).ToList()
来源：http://hz.gaohongyu789.top/gtfdutjota.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtdipnrxrh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtfbxpiaku.html

PHP:  sort($arr);
来源：http://hz.gogol.net.cn/gtqizsevsb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.9152youxi.cn/gtqszxlltr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aibaodan.cn/gtsinuruog.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhaomingkeji.xyz/gtzjntztdo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtijfqohhj.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtzausvsqz.html

C#:   list.Sort();
来源：http://hz.cdnleiting.top/gtsrohykwq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj20258888.top/gtbwiajmex.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.havefunace.top/gtbhfbjrpm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtfromjduf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtlqzehvos.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.52xcode.cn/gtukivefbv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.havefunace.top/gtnmgjlfkh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jiagoushi.top/gtgqpixwcf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gtkqijxcen.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtrntnlzjr.html

[D11] 反转数组
来源：http://hz.hywenlv.cn/gtojtylxjo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.daxiang520.top/gtcmogxoyo.html

PHP:  array_reverse($arr);
来源：http://hz.jinyuanbaomall.cn/gtnwurqfob.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jianghu66.top/gtvugrgxva.html


<!-- 参考信息 -->