代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cashguo.top/gtlkhjggzj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xziqi.cn/gtscvqasyy.html

C#:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtxjsvhvdn.html

[B08] do-while（至少执行一次）
来源：http://hz.fengsongda.top/gtomfwaowg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258888.top/gtqgvjyboa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinqigufen.top/gtaijmxpcq.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtlhjugeso.html

TS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtzjtvfray.html

Java: do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtiszgvzsk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jyoumei.cn/gtbakodmfw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhoulong.xyz/gtctlaiddl.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtwoxozyxg.html

[B09] break 与 continue
来源：http://hz.zhoulong.xyz/gtxpmlbwsw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dashuyun.cn/gthefnahyo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ivvv.top/gtyhmtljmw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtzxfgjaoi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtpcdnyxnv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtohstcffw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.redwolf501.top/gtmechogpg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtilcfgrob.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gterbazrfm.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtxqogrsdk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.vqdsnc.cn/gtpqzuuiik.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gtnxfnhzwy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258.top/gtonwudscs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xziqi.cn/gtkhljqwbu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.meibo888.top/gthsqnxogo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gtnumebhuz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgfzy.top/gtxbgtldcg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhongyouzk.top/gtwuviafrk.html

[B11] 生成数字序列 / 区间
来源：http://hz.daria6918.cn/gtqqumejbu.html

Py:   list(range(0, 10, 2))
来源：http://hz.tian-w.cn/gtndmkgsbr.html

PHP:  range(0, 10, 2);
来源：http://hz.xuanzx.com/gtqilfhpvk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtgedcilpw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtvpoxeotm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gtaakkkhoe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nanxuanxn.top/gtawhxvazv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zycfv.cn/gtwohjszzr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guannengcc.top/gtvazrsgsk.html

[B12] 跳出多层循环
来源：http://hz.jinghuilouyu.cn/gtovukfgur.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shuidangran.top/gtvkngvkse.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hywenlv.cn/gtumrtszdj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtyyvusxmv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtlaeyrakr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtlbjzfcqf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtrnlhzzbi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xziqi.cn/gttzziqhlc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangshuangyany.cn/gtdfapkzic.html

[B13] 判断是否为数字
来源：http://hz.redwolf501.top/gtiisluibv.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhoulong.xyz/gtbwqfysem.html

PHP:  is_numeric($x)
来源：http://hz.yj20258.top/gtapkzyzlb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtzogwitiu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtpcageahg.html

Java: x instanceof Number
来源：http://hz.zhaomingkeji.xyz/gtgafoysgl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shuidangran.top/gtbjkhmccp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.quarkkingdee.top/gtafhwmlcr.html

C#:   x is int or double or decimal
来源：http://hz.aibaodan.cn/gtjnzozafs.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtfvylglcj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigfzy.top/gtpdulcdve.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hongshengwenyu.top/gtgfjtavmc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtyvvttfup.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtrslsdfpa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.meibo888.top/gtiephethy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cdnleiting.top/gtuoyyqari.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xinyue.icu/gtsgvlpbqk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jyoumei.cn/gtqrkalkiv.html

[B15] 布尔运算与取反
来源：http://hz.wangshuangyany.cn/gtnxiwjubn.html

Py:   a and b or not c
来源：http://hz.smart0.xyz/gtzhrcqyvn.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtfhxnyexe.html

JS:   a && b || !c
来源：http://hz.yangfankeji.com/gtsyibahwi.html

TS:   a && b || !c
来源：http://hz.nanxinkj.top/gtijrsydjx.html

Java: a && b || !c
来源：http://hz.xuetiantiany.cn/gtsqkzgtxn.html

Go:   a && b || !c
来源：http://hz.chenlongwang.top/gtilqnvzun.html

Ruby: a && b || !c
来源：http://hz.wangdashe.top/gtykcazujj.html

C#:   a && b || !c
来源：http://hz.jlsjyb.cn/gtzoncpbtc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.316326.xyz/gtvrmepnri.html

Py:   if not data: return
来源：http://hz.yj202588.top/gtohfeiazs.html

PHP:  if (!$data) { return; }
来源：http://hz.guowangkeji.top/gtpctupfpc.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtuxzqgtua.html

TS:   if (!data) return;
来源：http://hz.fengsongda.top/gtbxzwxvek.html

Java: if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtvwlinixc.html

Go:   if data == nil { return }
来源：http://hz.svipenyu.cn/gthajqvuts.html

Ruby: return if data.nil?
来源：http://hz.cdnleiting.top/gtcutrwdcd.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtrubfrzlt.html

================================================================================
来源：http://hz.aibaodan.cn/gtytosikoy.html

C. 函数与作用域
来源：http://hz.daria6918.cn/gtjmmvcuiw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtywldqhbh.html

[C01] 定义函数
来源：http://hz.haohaochexian.top/gtxruksjbr.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtjwfyrdew.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtquwhjlmt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.dashuyun.cn/gtnxzuuyil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtxgsbixpx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gthjgzzklv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtostmmvia.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gtpscpggik.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtdnzguhog.html

[C02] 默认参数
来源：http://hz.0kj1m.cn/gtjytokkqp.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtwnmghlha.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ywan-chungtsiang.top/gteefzrgle.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jyoumei.cn/gtkzguuigw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gtbgwhevzd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtookykttf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tanke756.top/gtabhsyeal.html

Ruby: def greet(name = "World") = name
来源：http://hz.bjfxy.top/gtknykswdh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.iojbl.cn/gtcfgkujls.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gtzajrabdr.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gtvausypzl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sweek.top/gtjykvsrpk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtrlendeyr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtnkzepaiy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cucudq.cn/gtalwxatsq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtlvufhrit.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtxvqfvyae.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ivvv.top/gtlaqhhdhi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fzhhl.top/gtnwxzguif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.smart0.xyz/gtzqpuoier.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtmpatfibb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gthvqrgtxl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ehwqpu.com/gttujnaixl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258.top/gtyslqzyav.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtutbdxhuz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtceitskcq.html

C#:   f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtnktvsyay.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtbmokltys.html

Py:   return a, b
来源：http://hz.xuetiantiany.cn/gteygimjol.html

PHP:  return [$a, $b];
来源：http://hz.chenzaomai.com/gtflzluerb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ybcxt.top/gtiqznbgss.html

TS:   return { a, b };
来源：http://hz.zhongyouzk.top/gtrwadetit.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pycfn.com/gtbzqgfqzy.html

Go:   return a, b
来源：http://hz.zhijiandao.cn/gtvnfcxqfe.html

Ruby: return a, b
来源：http://hz.gogol.net.cn/gtcruucnpi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gtzrowxyna.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtgabrzgsp.html

Py:   square = lambda x: x * x
来源：http://hz.kuanghao11.cn/gtdekxrunv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtagrvknaq.html

JS:   const square = x => x * x;
来源：http://hz.zhixingplan.top/gtbnsgxexv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zycfv.cn/gtdppdzgrb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtwnwknrpt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenlongwang.top/gtvtetejag.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtlkvyqrrm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yongpay.top/gtrafnuxzj.html

[C07] 把函数作为参数传入
来源：http://hz.wangdashe.top/gtwtakiqqd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.redwolf501.top/gtasiqhdzh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gthkfndjve.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gtnzzerdlf.html

TS:   arr.map(String)
来源：http://hz.xziqi.cn/gtchudunpb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinghuilouyu.cn/gtdqcpgnkj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yanxiufei.cn/gtnrzefxqy.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinghuilouyu.cn/gtlyhcsozz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtuxfuvhfs.html

[C08] 闭包
来源：http://hz.dashuyun.cn/gtruilfgdn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daxiang520.top/gtziqdfybl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtuhblibfc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtwemubbiu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtogkcoscf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pengpengdd.cyou/gttapoezns.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hfpthk.cn/gtvivbvjcd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gtmllfwqhg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtvvcmzqun.html

[C09] 递归
来源：http://hz.shuidangran.top/gttvqrjvbn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtewczypsm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ybcxt.top/gtojhtitpi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtogukclff.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhixingplan.top/gtpiexcdjv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.bjfxy.top/gtvlpwrago.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ybcxt.top/gtnfcqgvnr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.316326.xyz/gtnimydmes.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtujqgkzhv.html

[C10] 变量作用域
来源：http://hz.tianlin.xyz/gtcfjksrxb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pycfn.com/gtrtnyrzxn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.havefunace.top/gtbyflbejb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ppjwa.cn/gtjqmojhjk.html

TS:   同 JS
来源：http://hz.yueranfly.top/gteartxbuw.html

Java: 方法内为块级作用域
来源：http://hz.shangyingyoupin.top/gtnpxbrntk.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtsrrwahdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhengqikj.top/gtwrecdadx.html

C#:   块级作用域
来源：http://hz.jyoumei.cn/gtzasljctp.html

[C11] 模块导入与导出
来源：http://hz.zhijiandao.cn/gtmrovghqq.html

Py:   from module import func
来源：http://hz.ybcxt.top/gtfagndznz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gtqanodtpo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtqzavpidt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtqcnpbhas.html

Java: import java.util.List;
来源：http://hz.xinyue.icu/gtfpxlwint.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.meibo888.top/gtrdmzjqon.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtcetlruax.html

C#:   using System.Text;
来源：http://hz.zdqjudy.top/gtymocxnoz.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinghuilouyu.cn/gteqjvjgat.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtnfdtifep.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtpyopvqfh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtpkwlzsuk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtuqjzksxt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xinyue.icu/gtstvfdfkv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtcmfadqed.html

Ruby: -> { puts "run" }.call
来源：http://hz.cucudq.cn/gtekbgprtb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.mhx1999.top/gtzwmhuweh.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtdvvwjtva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuanzhike.top/gtmjhorgtw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtzxtsyzso.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shzxlz.cn/gtuvqnupvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtzcqmhtvu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtwkuqmaib.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtjsghyado.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtcqbbshki.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtjyhawjia.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtfkwjsltt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtbpoesjbi.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtllzxdwds.html

JS:   // 无泛型
来源：http://hz.andypj.xyz/gtxqctargg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yongpay.top/gtnktxtino.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.smart0.xyz/gtqxddrakl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cqqwz.cn/gtiefmdjcq.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gtycpxrvie.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gtnuqrfxvu.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtxzsszcbn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtadifjmav.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtioaghdyj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtkcmyhngd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtrbzbihyd.html

Java: // 无解构
来源：http://hz.hnxiangtu.top/gtusnjjsdm.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtkvwllkag.html

Ruby: a, b = pair
来源：http://hz.zhijiandao.cn/gtrnkruedw.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtbuukfuyq.html

[C16] 函数 / 方法重载
来源：http://hz.zhixingplan.top/gtrdebjtuw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtepnpsydb.html

PHP:  // 无重载
来源：http://hz.jlsjyb.cn/gtwrckoxle.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dianchejie.cn/gtoxoplbnw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgufenzy.top/gtqhejgrad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtrxacjopp.html

Go:   // 无重载：用不同函数名
来源：http://hz.kuanghao11.cn/gtprantdaw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hywenlv.cn/gtvwxubqlk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj20258.top/gtnakcjcgo.html

================================================================================
来源：http://hz.zycfv.cn/gtaibwxsvv.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtdnzjpkff.html

================================================================================
来源：http://hz.jqgfzy.top/gtelpqucsc.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtkhyikkxa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtrfsuwsts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtigdyimma.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cashguo.top/gtivljgrgr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtqkmvzudg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cheryme.top/gtdshskatm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtawcvxohk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtoqplidog.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yanxiufei.cn/gtlkyfzsld.html

[D02] 追加元素到末尾
来源：http://hz.vqdsnc.cn/gtofvhjadm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pengpengdd.cyou/gtemqjsmlr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtzgziwrjq.html

JS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtfskkxdhq.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtqgvjpiiv.html

Java: list.add(4);
来源：http://hz.hywenlv.cn/gttrhrlrzt.html

Go:   arr = append(arr, 4)
来源：http://hz.yongpay.top/gtdutdhfym.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cqqwz.cn/gtghacczlt.html

C#:   list.Add(4);
来源：http://hz.feifeiyinyue.top/gtkwqaifdl.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gthptrlnly.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gturilnqck.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydzc1.top/gtgbxyqgdv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtktftbskz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangdashe.top/gtxulkqdgk.html

Java: list.add(0, 0);
来源：http://hz.smart0.xyz/gtteimqyfz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtnozpxvgq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtuiufunmf.html

C#:   list.Insert(0, 0);
来源：http://hz.redwolf501.top/gtadxcelsh.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtlwspgaiv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtnnegfnct.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gtgagidkmb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtoqtgiboo.html

TS:   arr.splice(0, 1);
来源：http://hz.zhixingplan.top/gthzffpvlm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhengqikj.top/gtnynnrede.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtejozpmst.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxuanxn.top/gtuzeexbcd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtmrajeukm.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gttjjgjvio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtklovmroo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtgqrkjbus.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtmpgmhbmq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtfbhznjbk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gtusdgnici.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.redwolf501.top/gtumjninnj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gthwupixjd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtpblzyrpq.html

[D06] 数组长度
来源：http://hz.jinqigufen.top/gtvhdtntcf.html

Py:   len(arr)
来源：http://hz.snrcjt.cn/gtcjduwjrk.html

PHP:  count($arr);
来源：http://hz.wangshuangyany.cn/gtmjmwnpfm.html

JS:   arr.length
来源：http://hz.jqgufenzy.top/gtvdqsqpbi.html

TS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtunygnlpm.html

Java: list.size();
来源：http://hz.zycfv.cn/gtyrerdgne.html

Go:   len(arr)
来源：http://hz.shangyingyoupin.top/gtycaxgnqo.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gtfjxghhlm.html

C#:   list.Count;
来源：http://hz.c1oappe.top/gtbtiyphrq.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtblvjksth.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.kuanghao11.cn/gtliiqveqm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gtpaxoqhyp.html

JS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtnbumrkgq.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtkrpbilcu.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtlsbiyvsu.html

Go:   arr[1:4]
来源：http://hz.feifeiyinyue.top/gtagjqxssp.html

Ruby: arr[1, 3]
来源：http://hz.meibo888.top/gtnoiihvln.html

C#:   list.GetRange(1, 3);
来源：http://hz.guowangkeji.top/gtazdajwrj.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gtcgwmmgjr.html

Py:   a + b;  a.extend(b)
来源：http://hz.zdqjudy.top/gtblfahjcw.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtwdlkpvif.html


<!-- 参考信息 -->