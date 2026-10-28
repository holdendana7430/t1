代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cheryme.top/gtpbhsbrml.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aizwys.cn/gtbtyokwmp.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtxtizycwz.html

[B08] do-while（至少执行一次）
来源：http://hz.gaohongyu789.top/gtiurrwjhs.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuanzhike.top/gtdzbzxmaz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gaohongyu789.top/gtigpauzis.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtynuvrkma.html

TS:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtvdhrzfwb.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtkoaytusn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.quarkkingdee.top/gtzznqvfqq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinghuilouyu.cn/gtmrbzqcfp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtcmrhoqbw.html

[B09] break 与 continue
来源：http://hz.zhoulong.xyz/gtkbgehiaa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gotoacloud.top/gtjarwspcf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yangfankeji.com/gtvofamcxc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtmcfandvj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtlxuewxhc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtglnrunxw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigufen.top/gtcdbttigq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtnufgerzr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtuqpcelcs.html

[B10] 遍历同时拿索引
来源：http://hz.zhixingplan.top/gtijnrsxbz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cashguo.top/gtnfqkimro.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinqigufen.top/gtrduoxkgz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daxiang520.top/gtpvsvnxdl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ybcxt.top/gttfydlzat.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gaohongyu789.top/gthjzlpkyf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xuanzx.com/gtfhlqjwqy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zdqjudy.top/gtiaptjdbo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jqgfzy.top/gtppincneh.html

[B11] 生成数字序列 / 区间
来源：http://hz.birdmap.top/gtyzhdgcnm.html

Py:   list(range(0, 10, 2))
来源：http://hz.cdnleiting.top/gtxpecthof.html

PHP:  range(0, 10, 2);
来源：http://hz.zhaomingkeji.xyz/gtltyxszrw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtayzyjypb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jlsjyb.cn/gtdedywpme.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtniqslvhp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.guowangkeji.top/gtszyfixzw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtftcjxvgi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shangyingyoupin.top/gthgbiskxs.html

[B12] 跳出多层循环
来源：http://hz.cucudq.cn/gtbeomfiac.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cucudq.cn/gtqcqisgmq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nanxuanxn.top/gtyafhswfd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtxpnofwif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtahrfydmo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtrxqbfthb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ivvv.top/gtplwkptsx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtwduyakji.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydzc1.top/gtwscucfct.html

[B13] 判断是否为数字
来源：http://hz.dashuyun.cn/gtbnousogl.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenzaomai.com/gtmlhhatxy.html

PHP:  is_numeric($x)
来源：http://hz.havefunace.top/gtzaaydcmh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtwnbulhic.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtupoeywye.html

Java: x instanceof Number
来源：http://hz.xuanzx.com/gtlhprpnmu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hongshengwenyu.top/gtsvtscbun.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuanzx.com/gtchnpyufa.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtmpptjkmf.html

[B14] 判断值是否在集合内
来源：http://hz.daxiang520.top/gtymuhttjl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuxming.cn/gtngjcinte.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtyfqemyyr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtljivkihn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.smart0.xyz/gtpbflgoot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gaohongyu789.top/gtbaykguzs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hywenlv.cn/gtzwocytgi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinyuanbaomall.cn/gtrtkqffzz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.iojbl.cn/gttxmdpshy.html

[B15] 布尔运算与取反
来源：http://hz.fzhhl.top/gtxthpgllq.html

Py:   a and b or not c
来源：http://hz.shanyushiyangkeji.top/gtfpigoqic.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gtkyosrgtq.html

JS:   a && b || !c
来源：http://hz.cucudq.cn/gtsolcxpai.html

TS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtiaqxyadt.html

Java: a && b || !c
来源：http://hz.hfpthk.cn/gtzxslvhey.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gttnikjwij.html

Ruby: a && b || !c
来源：http://hz.smart0.xyz/gtvcwsqpgc.html

C#:   a && b || !c
来源：http://hz.hnqzz.top/gtzajtguow.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhaomingkeji.xyz/gtbfsflfxa.html

Py:   if not data: return
来源：http://hz.jiagoushi.top/gtdojewkgy.html

PHP:  if (!$data) { return; }
来源：http://hz.birdmap.top/gtuffkojkx.html

JS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtufpzwmep.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gthsgjtpeq.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtwuihudqb.html

Go:   if data == nil { return }
来源：http://hz.ydzc1.top/gtqwyvtksc.html

Ruby: return if data.nil?
来源：http://hz.ydjk.org.cn/gtnqtfmwiq.html

C#:   if (data == null) return;
来源：http://hz.jinqigfzy.top/gtlmavktki.html

================================================================================
来源：http://hz.ybcxt.top/gtvpktvhzv.html

C. 函数与作用域
来源：http://hz.xylfe.cn/gtegcvfosl.html

================================================================================
来源：http://hz.yvedp.cn/gtrhfbbdkw.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtzfxuhejb.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtnmcxxkjg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtjwqthdju.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtouxmnvij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtelepbmfa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtzccdvixm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtohsyffka.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ehwqpu.com/gtwijodvey.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtuvghpnek.html

[C02] 默认参数
来源：http://hz.yongpay.top/gtnkswsrno.html

Py:   def greet(name="World"): return name
来源：http://hz.yuxming.cn/gthktizvpi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.52xcode.cn/gtazffzpzr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhijiandao.cn/gtdtcjzcik.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cheryme.top/gtxdfnvsfh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtvksyaocu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nwbrower.top/gtsyullmyw.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydzc1.top/gtwsxbolmp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zdqjudy.top/gtzxqntlye.html

[C03] 可变参数
来源：http://hz.shanyushiyangtech.top/gtavkovegj.html

Py:   def total(*args): return sum(args)
来源：http://hz.xziqi.cn/gtiszyxacz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258.top/gtdrmehszf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtvbylgvvt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtazmcegag.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtwdvrxwsb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenzaomai.com/gtzrsnuodv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtpxvifjcc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guowangkeji.top/gtpeuvvsem.html

[C04] 命名参数 / 关键字参数
来源：http://hz.meibo888.top/gtjbjmgzju.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtndwnkedc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yvedp.cn/gtqqfejxwy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtpyvhaxnu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ywan-chungtsiang.top/gtgjlmttdu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.haohaochexian.top/gtbxfspoxp.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydjk.org.cn/gthghocppr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtqkjklikg.html

C#:   f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtjhmkuynf.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtqvslwzxr.html

Py:   return a, b
来源：http://hz.wangdashe.top/gtxsmklfsc.html

PHP:  return [$a, $b];
来源：http://hz.kuanghao11.cn/gturortlyf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cheryme.top/gtvuwozoba.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtzfsyukit.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258888.top/gtxkfmqxce.html

Go:   return a, b
来源：http://hz.c1oappe.top/gthvbyvyuy.html

Ruby: return a, b
来源：http://hz.hnqzz.top/gtghjybmus.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydzc1.top/gteyrltaka.html

[C06] 匿名函数 / lambda
来源：http://hz.zhoulong.xyz/gtrpetvgye.html

Py:   square = lambda x: x * x
来源：http://hz.birdmap.top/gtvccyezmv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ywan-chungtsiang.top/gtlmkhzlqn.html

JS:   const square = x => x * x;
来源：http://hz.jinqigfzy.top/gtmqnyiktg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.tian-w.cn/gtbekbnjpe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.kuanghao11.cn/gtxeemfykw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxinkj.top/gtmmnghatq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tianlin.xyz/gtcmbyznao.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nwbrower.top/gtcromqzyt.html

[C07] 把函数作为参数传入
来源：http://hz.cashguo.top/gttrufwrcs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cucudq.cn/gtiocpygej.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gtksbqaied.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guowangkeji.top/gtukkgewhp.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gtezlvpyfs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hammf.cn/gtjznkvxrf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.kuanghao11.cn/gtbhbbtglp.html

Ruby: arr.map(&:upcase)
来源：http://hz.hongshengwenyu.top/gtlohevzod.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtoszlpsmc.html

[C08] 闭包
来源：http://hz.ivvv.top/gtvymqjsbw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhoulong.xyz/gtgfofctbd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shangyingyoupin.top/gtmjgtspwc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtnxyezase.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtpepufkii.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtwewzydqq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aizwys.cn/gtpaktnxfv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sxryk.cn/gtcgouudqt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtkcvsepif.html

[C09] 递归
来源：http://hz.hnqzz.top/gtmoxfjroc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xziqi.cn/gtgkpqhfxd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtcnoghlac.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gttwadgbnx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhongyouzk.top/gtfleloery.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nwbrower.top/gteibilzfo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gotoacloud.top/gtfihdrdek.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtuimqhiua.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.vqdsnc.cn/gtabbrdgfk.html

[C10] 变量作用域
来源：http://hz.birdmap.top/gtbbpiopgq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtkhvodasx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zycfv.cn/gtprzfuaiz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhoulong.xyz/gtqhsihukz.html

TS:   同 JS
来源：http://hz.ybcxt.top/gtxwzkbdjd.html

Java: 方法内为块级作用域
来源：http://hz.hfpthk.cn/gtfjzulgbr.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtsxczjdyb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sxryk.cn/gthprfvrbu.html

C#:   块级作用域
来源：http://hz.birdmap.top/gtyljvrckh.html

[C11] 模块导入与导出
来源：http://hz.bjfxy.top/gtzwzdipyy.html

Py:   from module import func
来源：http://hz.kuanghao11.cn/gtgkoyjdfk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangdashe.top/gttdkdqsuf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cdnleiting.top/gtqciiwczg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtovqxmzml.html

Java: import java.util.List;
来源：http://hz.ydjk.org.cn/gtavsrxyfz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zdqjudy.top/gtwbapvvfk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhixingplan.top/gtxnwkvada.html

C#:   using System.Text;
来源：http://hz.316326.xyz/gtdpfrxhgv.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtnextogcd.html

Py:   (lambda: print("run"))()
来源：http://hz.ehwqpu.com/gtsmjyweed.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangdashe.top/gtjigqjwuv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtwhcbbyza.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtlkuzlkjk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jyoumei.cn/gtylkyrghx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.vqdsnc.cn/gtxhflmuib.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtribfunbf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenzaomai.com/gtlrcirdip.html

[C13] 类型声明 / 类型注解
来源：http://hz.tianlin.xyz/gtmzthiooj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj202588.top/gtcqhnezxa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtbqgkplpy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtpihmrxof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtxdzgpocx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtqmtboeyu.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gtvkqttfvx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtlqsupkta.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tianlin.xyz/gtnepqatfe.html

[C14] 泛型函数
来源：http://hz.tianlin.xyz/gtlzmbxwqb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtmlukeemf.html

PHP:  // 无泛型
来源：http://hz.cdnleiting.top/gtemeiygwh.html

JS:   // 无泛型
来源：http://hz.jiagoushi.top/gttzwbqjeq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtddseclha.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhongyouzk.top/gtpiqgxsve.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xylfe.cn/gtnynihusw.html

Ruby: # 无泛型
来源：http://hz.xuetiantiany.cn/gtuxtedrlq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtuvmobciw.html

[C15] 解构 / 展开参数
来源：http://hz.fengsongda.top/gteubxlttj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.9152youxi.cn/gtkbzohurg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hammf.cn/gtyyqntrfd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtezsqbmyi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xylfe.cn/gtuvryhtix.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtxbbgcgnd.html

Go:   // 无解构
来源：http://hz.pycfn.com/gtsznwhiln.html

Ruby: a, b = pair
来源：http://hz.ywan-chungtsiang.top/gtcvnxiwfj.html

C#:   var (a, b) = pair;
来源：http://hz.jqgfzy.top/gtculsqeui.html

[C16] 函数 / 方法重载
来源：http://hz.yonumen.top/gtavljmmbn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gtvuhmkeyw.html

PHP:  // 无重载
来源：http://hz.yonumen.top/gtumvfsvbu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dianchejie.cn/gtethmyqej.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.9152youxi.cn/gtauscaqig.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gtsqcxymsl.html

Go:   // 无重载：用不同函数名
来源：http://hz.xingfuxueyuan.xyz/gtrsejdyqr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhoulong.xyz/gtrnvexzhk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cheryme.top/gtziodkyvy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgdhaynhx.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtyknjthlq.html

================================================================================
来源：http://hz.zhengqikj.top/gtvvjxksqv.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtbjhhhfeg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gtzomumrph.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtvznrxyrv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dashuyun.cn/gtjhcckybn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pycfn.com/gtuvmsmyel.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtfjvygsli.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gtrozmkkth.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj202588.top/gtymhsxnlb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtejkvkbjp.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtjhhzgdnq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shzxlz.cn/gtgujfokht.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aizwys.cn/gtxqffzimo.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtxlgnxttw.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtacwhvjwb.html

Java: list.add(4);
来源：http://hz.ppjwa.cn/gtbkuaswab.html

Go:   arr = append(arr, 4)
来源：http://hz.xuanzx.com/gtnmjwknyb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fengsongda.top/gtsjzhnoif.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtuzzrcpcl.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigufen.top/gtcupgkyhn.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtzxlqmufk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtmxmpxrdb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gtoahpdjjo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jianghu66.top/gtrujpuaje.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtbequhsex.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtplmfjsvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuxming.cn/gtcgfqiewl.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gterbtrxyo.html

[D04] 删除元素
来源：http://hz.9152youxi.cn/gtcownvoks.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hfpthk.cn/gtrwlznmmh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.redwolf501.top/gtlmhktxqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydjk.org.cn/gtwfzacsno.html

TS:   arr.splice(0, 1);
来源：http://hz.cqqwz.cn/gtdzpvocss.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnxiangtu.top/gtyatlbtjq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtwhhhoxdj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtzmhcszgy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhengqikj.top/gtwdiwjonj.html

[D05] 访问与修改元素
来源：http://hz.dashuyun.cn/gtsfghyssh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtyxafageb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtdiinbywh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gtjcazsdja.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtttcttyml.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtdtgrpwbm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtqppzmvaa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gttklqjdod.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gturtddjvt.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtihajmmir.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtxajgwikv.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtxvzxbpkn.html

JS:   arr.length
来源：http://hz.cheryme.top/gtkcwbidru.html

TS:   arr.length
来源：http://hz.yj20258.top/gtjcsgmyxz.html

Java: list.size();
来源：http://hz.9152youxi.cn/gtwblauxqj.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gthwsnwxtl.html

Ruby: arr.length; arr.size
来源：http://hz.zhoulong.xyz/gtggvhkssq.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtxdewfidy.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gttzpidlkh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ivvv.top/gtpebhctfc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtnqkkffyj.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gttxgtcspf.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtmnuxwqsc.html

Java: list.subList(1, 4);
来源：http://hz.chenlongwang.top/gtzhgkfhzb.html

Go:   arr[1:4]
来源：http://hz.cheryme.top/gtachxkwnl.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtgmajfcxx.html

C#:   list.GetRange(1, 3);
来源：http://hz.quarkkingdee.top/gtgenrrrex.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtuobtzabw.html

Py:   a + b;  a.extend(b)
来源：http://hz.yangfankeji.com/gtbryqomng.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigfzy.top/gtuxeoibkc.html


<!-- 参考信息 -->