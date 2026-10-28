代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.c1oappe.top/gtivxdygzh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.svipenyu.cn/gttudrqwtf.html

C#:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtypykujzu.html

[B08] do-while（至少执行一次）
来源：http://hz.jqgfzy.top/gtcrukxhkl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxuanxn.top/gtmykkkqpj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cheryme.top/gtliwkeufo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtzpqglmur.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtsxjawfev.html

Java: do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtdbbmqxeo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.fengsongda.top/gtqgwucskx.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ppjwa.cn/gtralepvwa.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtrbbrvojq.html

[B09] break 与 continue
来源：http://hz.shanyushiyangtech.top/gtzdqfwaoz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.haohaochexian.top/gtoriepifw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hammf.cn/gtrnsuzxdq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gttphrofym.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtqwiujgzc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtribozmxg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.dashuyun.cn/gtnffultwc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jlsjyb.cn/gteosnqhtz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gthfdamkbp.html

[B10] 遍历同时拿索引
来源：http://hz.sysykeji.top/gtotpmttsj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zdqjudy.top/gtyhxntuli.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jianghu66.top/gtzlaycccu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hywenlv.cn/gtrfjbmvhy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hywenlv.cn/gtlrpbmdlq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.9152youxi.cn/gtlnzyaolw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tianlin.xyz/gtvjvggyqj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj202588.top/gtiupnoucv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.mhx1999.top/gtamegkyrb.html

[B11] 生成数字序列 / 区间
来源：http://hz.gaohongyu789.top/gtlaqikpjm.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxuanxn.top/gtiltrqxkg.html

PHP:  range(0, 10, 2);
来源：http://hz.wangdashe.top/gtodxbmnkr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gotoacloud.top/gtdzdithji.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtcqohxomc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenjidiqi.icu/gtpejbxesb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhengqikj.top/gtwdfgwdtl.html

Ruby: (0...10).step(2).to_a
来源：http://hz.smart0.xyz/gtlxbtpxun.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yanxiufei.cn/gtlhdgappo.html

[B12] 跳出多层循环
来源：http://hz.andypj.xyz/gtnkvcqkaf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zycfv.cn/gteexuclxv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenlongwang.top/gtmgbljpoo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtgmmxgefy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtvpuldjlc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtznjtagnz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jyoumei.cn/gtybrwnfaa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ydzc1.top/gtmdncmibb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jlsjyb.cn/gtuufmatej.html

[B13] 判断是否为数字
来源：http://hz.guowangkeji.top/gtmxzoaeoi.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj20258888.top/gtdxorfbvx.html

PHP:  is_numeric($x)
来源：http://hz.fengsongda.top/gtcjmicpmq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gaohongyu789.top/gtykxisjsu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtzwqjnjsp.html

Java: x instanceof Number
来源：http://hz.c1oappe.top/gtifdzztvz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dianchejie.cn/gtzwzpbsle.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhengqikj.top/gtuzazanje.html

C#:   x is int or double or decimal
来源：http://hz.meibo888.top/gtgbnqazmt.html

[B14] 判断值是否在集合内
来源：http://hz.andypj.xyz/gthmneiaye.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cqqwz.cn/gtkhwssfze.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gttolhzxsw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gtbgqtvznt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtiiotavgr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.daxiang520.top/gtdguqijgf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigufen.top/gtkawsagxt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.316326.xyz/gtdjaxjahd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sufxvd.cn/gtrleszqvz.html

[B15] 布尔运算与取反
来源：http://hz.jinghuilouyu.cn/gtblvtrnym.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtvvnbhusa.html

PHP:  $a && $b || !$c
来源：http://hz.cucudq.cn/gtybpbfbsr.html

JS:   a && b || !c
来源：http://hz.xinyue.icu/gtuwkdrlhn.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gthyatzhnu.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtntugljwu.html

Go:   a && b || !c
来源：http://hz.hywenlv.cn/gtwfsjxoyh.html

Ruby: a && b || !c
来源：http://hz.hysaishi.cn/gtzaqfiuuu.html

C#:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtqywrubtt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.chenjidiqi.icu/gtdbaixfpv.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gttsmsqzlm.html

PHP:  if (!$data) { return; }
来源：http://hz.iojbl.cn/gtrzdwfaby.html

JS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtxsrwhvbl.html

TS:   if (!data) return;
来源：http://hz.xuanzx.com/gtafzokaie.html

Java: if (data == null) return;
来源：http://hz.yonumen.top/gtrsmlikwt.html

Go:   if data == nil { return }
来源：http://hz.hysaishi.cn/gtehtzuyvo.html

Ruby: return if data.nil?
来源：http://hz.yj20258.top/gtvuupwexb.html

C#:   if (data == null) return;
来源：http://hz.jianghu66.top/gtovzbhlye.html

================================================================================
来源：http://hz.yangfankeji.com/gtrieypibh.html

C. 函数与作用域
来源：http://hz.jinqigfzy.top/gtaaklotxq.html

================================================================================
来源：http://hz.cucudq.cn/gtyeahdxtn.html

[C01] 定义函数
来源：http://hz.bjfxy.top/gtnkejrvex.html

Py:   def add(a, b): return a + b
来源：http://hz.yonumen.top/gtctuktuqe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtafvvcczu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.52xcode.cn/gtaydkzmvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtaxstcuml.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtfkqlgreb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tanke756.top/gtxrfjrzin.html

Ruby: def add(a, b); a + b; end
来源：http://hz.kuanghao11.cn/gtgdpxjmcz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gturbqcjlt.html

[C02] 默认参数
来源：http://hz.jinqigufen.top/gtamfldnhq.html

Py:   def greet(name="World"): return name
来源：http://hz.9152youxi.cn/gtrjvlmqna.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258.top/gtaofkfazf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gtcdaptlky.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.meibo888.top/gtrontvwhc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.vqdsnc.cn/gtygeneauu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtwhavnslj.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtfwpwyrhk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aizwys.cn/gtrfsfqzjx.html

[C03] 可变参数
来源：http://hz.jinqigufen.top/gthklcueku.html

Py:   def total(*args): return sum(args)
来源：http://hz.daxiang520.top/gtmamgrdjz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gtspyoqwva.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtvcufktbg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtrawbnytr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cashguo.top/gtfeedzknw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhijiandao.cn/gtzmcgexzo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhijiandao.cn/gtaydpiqgc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenzaomai.com/gtdfwwtvhk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhixingplan.top/gtyzrtwvmw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gtgzhdbkpr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.havefunace.top/gtdnydewdd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtsmmhzgik.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guowangkeji.top/gtstjyyejh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gtvggreptu.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gteyiugglo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtrsbyjhwq.html

C#:   f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtqlobptne.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtyeygrzik.html

Py:   return a, b
来源：http://hz.xuanzx.com/gtvoeemhtg.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtfpucpoqz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenlongwang.top/gtwwmdbdfx.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gttxlhyavk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhixingplan.top/gtbncxjweh.html

Go:   return a, b
来源：http://hz.sufxvd.cn/gtlqilrgwi.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtgjpbwwbv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gotoacloud.top/gtblyvxenq.html

[C06] 匿名函数 / lambda
来源：http://hz.zhaomingkeji.xyz/gtrbgdjvft.html

Py:   square = lambda x: x * x
来源：http://hz.yongpay.top/gtouypnxjo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.haohaochexian.top/gtpqczhehh.html

JS:   const square = x => x * x;
来源：http://hz.xylfe.cn/gtragnhauy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zycfv.cn/gtxquozbta.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenlongwang.top/gtoelfrlke.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxinkj.top/gtbubepsro.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtqgskiekd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuanzhike.top/gtwncopfsi.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtosselauc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jiagoushi.top/gtcdjmqoqx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.havefunace.top/gtxcpadtpy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtvffydmqg.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtdqqwyxkc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj202588.top/gtgbcvlitb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuetiantiany.cn/gtggidlrnn.html

Ruby: arr.map(&:upcase)
来源：http://hz.sufxvd.cn/gtoizwgzmv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtdszdnovp.html

[C08] 闭包
来源：http://hz.yangfankeji.com/gtqezsxtcp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gtmndiqhif.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.mhx1999.top/gtrjinbrsf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtlohrajob.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtxhcskkze.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dashuyun.cn/gttadkujkk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.daxiang520.top/gtmcwbtuzb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhaomingkeji.xyz/gtvvkcueoy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtnqfqgvhf.html

[C09] 递归
来源：http://hz.tianlin.xyz/gtcpavzaxr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.birdmap.top/gtkylqnniz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtlrjyvmep.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gtxyjnfwku.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtwrisvjyk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yongpay.top/gtlhasscbx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cucudq.cn/gtqooiwgei.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gtddrfstlc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.haohaochexian.top/gttgduigys.html

[C10] 变量作用域
来源：http://hz.quarkkingdee.top/gtffkwuxjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.havefunace.top/gtiixvxfth.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtueyvmhrh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtavrkdoru.html

TS:   同 JS
来源：http://hz.zhengqikj.top/gtcmaqooyp.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtptcdlosa.html

Go:   花括号块级作用域
来源：http://hz.xuanzx.com/gtehbnozng.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gtwwryyxsu.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gtocvqncgq.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtsikycmla.html

Py:   from module import func
来源：http://hz.wangshuangyany.cn/gtqckrwpsv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtdyxfcdck.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydzc1.top/gtuguzckat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnqzz.top/gtdefoiqwr.html

Java: import java.util.List;
来源：http://hz.smart0.xyz/gtebafcozu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtixmzdtwj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guannengcc.top/gtlxqrnosu.html

C#:   using System.Text;
来源：http://hz.c1oappe.top/gtltyycgay.html

[C12] 立即执行函数 IIFE
来源：http://hz.havefunace.top/gtbnyenwet.html

Py:   (lambda: print("run"))()
来源：http://hz.vqdsnc.cn/gtgmquoiyq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jianghu66.top/gtorpjcviq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtejolxrhy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtluobuqka.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangshuangyany.cn/gtwucyovfl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aibaodan.cn/gtvmaniuky.html

Ruby: -> { puts "run" }.call
来源：http://hz.shangyingyoupin.top/gtprxdqhte.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sufxvd.cn/gttiprwcjv.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuanzhike.top/gtrpyqgnyj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenlongwang.top/gtkovsgzkn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtnrxkktcm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ydjk.org.cn/gtzhcqzcqt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtlcilsxro.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtoohgjsgk.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtncgxhokf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.haohaochexian.top/gtdtpazaju.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gaohongyu789.top/gtdbkqmren.html

[C14] 泛型函数
来源：http://hz.yuxming.cn/gtzovowyxu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.birdmap.top/gtujgnxwdu.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtbtcwjuzp.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gtxbceejrs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtixzbxplu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtqqfavrme.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gttdrionxt.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtgjnkgiya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtgedjmsbp.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gtqlwlfeon.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yonumen.top/gtdbyetply.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tian-w.cn/gtjmniumwu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtpmebnvwn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yonumen.top/gtvwszikzl.html

Java: // 无解构
来源：http://hz.xylfe.cn/gtciululse.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gtpbaolhjy.html

Ruby: a, b = pair
来源：http://hz.xziqi.cn/gtpagmqyeh.html

C#:   var (a, b) = pair;
来源：http://hz.jyoumei.cn/gtvdhvbpse.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtncmdijfw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gtvbgwwwcu.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtofpebflg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.mhx1999.top/gtpzfuibyl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.feifeiyinyue.top/gtvdqhffnd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shuidangran.top/gtcpqjdgqg.html

Go:   // 无重载：用不同函数名
来源：http://hz.sweek.top/gtyprcoswr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtekkpbmvq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yonumen.top/gtotvyhljh.html

================================================================================
来源：http://hz.yuanzhike.top/gtybdrfije.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtcwkkqfjg.html

================================================================================
来源：http://hz.52xcode.cn/gtqwxnrhzp.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtgyswyjuv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.c1oappe.top/gtopzgiade.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtpdvhdvlx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yvedp.cn/gtdgaxhbkf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fengsongda.top/gtgeacctho.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tanke756.top/gthidgkcmm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hammf.cn/gtxcoqwsvh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.vqdsnc.cn/gtysieftdj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenjidiqi.icu/gtxkkdxzvb.html

[D02] 追加元素到末尾
来源：http://hz.nwbrower.top/gtehjnfkxj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhengqikj.top/gtbirtzxqh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtaqnsycnk.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtskkamhdf.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtjcdiyvgh.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtegwmvcxp.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtjyxwtkej.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.havefunace.top/gtjpszizyl.html

C#:   list.Add(4);
来源：http://hz.yuxming.cn/gtgwmydeex.html

[D03] 在指定位置插入元素
来源：http://hz.hnqzz.top/gtehqzxmcl.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtblupvetw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigufen.top/gtjjhgizjd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hongshengwenyu.top/gtjgrtidcd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hfpthk.cn/gthgobuvvv.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtvoqashxy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258888.top/gtvdazceyc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gogol.net.cn/gtvvskoaat.html

C#:   list.Insert(0, 0);
来源：http://hz.havefunace.top/gtlxabzhtz.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gtzntosxaa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtmcvmuhqx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xylfe.cn/gtifljdgbh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.feifeiyinyue.top/gtmhdvcqcl.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtuqigsgli.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydzc1.top/gtdlmetpvk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gtguuiyhet.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhongyouzk.top/gtbqwxuzst.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sweek.top/gtpswgnjux.html

[D05] 访问与修改元素
来源：http://hz.jinqigfzy.top/gteblxlusf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtjzeirbgy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.316326.xyz/gtfiatncjk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtabpiwkuy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtmuhubtgz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cheryme.top/gtydhxmook.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtnktoqbup.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtrfbgvijc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenjidiqi.icu/gtlrrnehjn.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtklkccxmd.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtaejypupz.html

PHP:  count($arr);
来源：http://hz.9152youxi.cn/gtmngaqnxu.html

JS:   arr.length
来源：http://hz.ivvv.top/gtlfgsnovr.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtxrbdcwrf.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtidtpgvup.html

Go:   len(arr)
来源：http://hz.aibaodan.cn/gtxftckvet.html

Ruby: arr.length; arr.size
来源：http://hz.meibo888.top/gtxmoepjvc.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gtefbolaoc.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258.top/gtjxlksptl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtglpgpsvy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydzc1.top/gtnmwolcma.html

JS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtiecqfhgn.html

TS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtcgmvdzhe.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtlhosowje.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtqjjofpga.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtbdaetrta.html

C#:   list.GetRange(1, 3);
来源：http://hz.316326.xyz/gttlljwwxi.html

[D08] 合并两个数组
来源：http://hz.gogol.net.cn/gtttxshjep.html

Py:   a + b;  a.extend(b)
来源：http://hz.gogol.net.cn/gtpmcodguf.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangtech.top/gtxzxmwxqc.html


<!-- 参考信息 -->