代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.wangdashe.top/gtdqecuhpt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinghuilouyu.cn/gtffpddnoe.html

[B07] while 循环
来源：http://hz.xuetiantiany.cn/gtkollxiij.html

Py:   while i < 10: i += 1
来源：http://hz.nwbrower.top/gtczfnqkvn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yangfankeji.com/gtpwzejuud.html

JS:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtrskpxfsu.html

TS:   while (i < 10) { i++; }
来源：http://hz.52xcode.cn/gtwvgpljne.html

Java: while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtwekqxzou.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangshuangyany.cn/gtnobqhgcy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shanyushiyangkeji.top/gtlsusuruu.html

C#:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtpigbxxwo.html

[B08] do-while（至少执行一次）
来源：http://hz.sxryk.cn/gtbmtsfqnr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.dianchejie.cn/gtmoyinuro.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnqzz.top/gtcvkohiyv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtfgeerkni.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtdqpfsmup.html

Java: do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtqonecacp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yanxiufei.cn/gtrzjnshyd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yvedp.cn/gtdlxsvypo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gthqfftwgl.html

[B09] break 与 continue
来源：http://hz.yonumen.top/gtnkzefkfa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jqgufenzy.top/gtzgbxpnxr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yuxming.cn/gtyfvxyibl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtxqhuuiyk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtzrjudwxb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtldjmompt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.dianchejie.cn/gtuehecsys.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.meibo888.top/gtufkdbzxr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtcryxfbey.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigfzy.top/gthlipwnwo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtdkzevgcn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jyoumei.cn/gthbxvijkk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigufen.top/gtckhfnzha.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtqroflhbn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj202588.top/gtzbxtrebp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zycfv.cn/gtkjprcbqn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtrnqpfrdo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ehwqpu.com/gtqmupnhhv.html

[B11] 生成数字序列 / 区间
来源：http://hz.ivvv.top/gttgqsgrfw.html

Py:   list(range(0, 10, 2))
来源：http://hz.yongpay.top/gtuweojftu.html

PHP:  range(0, 10, 2);
来源：http://hz.fzhhl.top/gtybgrytar.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuanzhike.top/gtdbvklswt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtpofmfvyn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgufenzy.top/gtqhftvmwt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtjiydxfml.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yongpay.top/gtrozosany.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yongpay.top/gtrptzduhd.html

[B12] 跳出多层循环
来源：http://hz.quarkkingdee.top/gtmlbppmde.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shuidangran.top/gtofdshkuj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnxiangtu.top/gtlmrlbohy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtjxuvdmke.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtrngwviyb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtcmhtvedn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhiwuduotai.top/gticyolipy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hfpthk.cn/gtgfqflbys.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aizwys.cn/gtplktnhzo.html

[B13] 判断是否为数字
来源：http://hz.cdnleiting.top/gttpcjroft.html

Py:   isinstance(x, (int, float))
来源：http://hz.mhx1999.top/gtinnznbpg.html

PHP:  is_numeric($x)
来源：http://hz.xylfe.cn/gtcujwvftu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gtoxhwlpyv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxinkj.top/gtcyemrydt.html

Java: x instanceof Number
来源：http://hz.xziqi.cn/gtlwxmwspc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.52xcode.cn/gtogdradty.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dashuyun.cn/gtgwcfrfqu.html

C#:   x is int or double or decimal
来源：http://hz.fzhhl.top/gtxiyeyphh.html

[B14] 判断值是否在集合内
来源：http://hz.shanyushiyangkeji.top/gtiuukkfoo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.svipenyu.cn/gtuulspigc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.c1oappe.top/gtjmjnidtl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tianlin.xyz/gtcwrchzwj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gttmmljzxx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtdunmauyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhiwuduotai.top/gtfxucfkih.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yongpay.top/gtmiecuprd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuetiantiany.cn/gtknjalygs.html

[B15] 布尔运算与取反
来源：http://hz.jyoumei.cn/gtmpfzfexv.html

Py:   a and b or not c
来源：http://hz.xuetiantiany.cn/gtdepraguq.html

PHP:  $a && $b || !$c
来源：http://hz.hysaishi.cn/gttkzejugz.html

JS:   a && b || !c
来源：http://hz.yvedp.cn/gtlxhbitye.html

TS:   a && b || !c
来源：http://hz.yuanzhike.top/gtkndrotrf.html

Java: a && b || !c
来源：http://hz.zhengqikj.top/gtdlocidop.html

Go:   a && b || !c
来源：http://hz.birdmap.top/gtbtnvscbm.html

Ruby: a && b || !c
来源：http://hz.hammf.cn/gtllscazkp.html

C#:   a && b || !c
来源：http://hz.shuidangran.top/gtofgdcolh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gttbourxyt.html

Py:   if not data: return
来源：http://hz.pycfn.com/gttbhcbyrb.html

PHP:  if (!$data) { return; }
来源：http://hz.chenjidiqi.icu/gtahhxwpck.html

JS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtmrwmsjmz.html

TS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtkiwsrmtr.html

Java: if (data == null) return;
来源：http://hz.hnqzz.top/gtwkcsccmf.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtybqurwph.html

Ruby: return if data.nil?
来源：http://hz.meibo888.top/gtgyvjlaze.html

C#:   if (data == null) return;
来源：http://hz.vqdsnc.cn/gtgdxrpqes.html

================================================================================
来源：http://hz.hywenlv.cn/gtqlesfryj.html

C. 函数与作用域
来源：http://hz.hnxiangtu.top/gtkfwfhcod.html

================================================================================
来源：http://hz.iojbl.cn/gtdmgctpxo.html

[C01] 定义函数
来源：http://hz.gaohongyu789.top/gtlkeqeuln.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtmukooewc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtrzckllfs.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fengsongda.top/gtnikfwpwe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtjlfzeiaq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtfroueqhe.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtsbhpwlwi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yvedp.cn/gtayuyjtzh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtjzmkyzvx.html

[C02] 默认参数
来源：http://hz.zhiwuduotai.top/gtaqfztuyh.html

Py:   def greet(name="World"): return name
来源：http://hz.xuetiantiany.cn/gtqbsvfuic.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtiqxnrahh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cashguo.top/gtjcicetgv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtjdhrkbvf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.0kj1m.cn/gterdmgkuh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtktjqisai.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuxming.cn/gtsaowgktn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.birdmap.top/gtoblqnhjf.html

[C03] 可变参数
来源：http://hz.cqqwz.cn/gtwxtdkoek.html

Py:   def total(*args): return sum(args)
来源：http://hz.gotoacloud.top/gtaajqnsgy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtgjaadoyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtxvkbcibd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gttzyubtyx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.52xcode.cn/gtosafroea.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtqbyvkoph.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangdashe.top/gtqfdmcpca.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinghuilouyu.cn/gtaabmxugf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhixingplan.top/gtsfofpsvz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhijiandao.cn/gtwodfkskk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dashuyun.cn/gtgkssrfms.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtzuaynqje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ywan-chungtsiang.top/gtazrddzyt.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cheryme.top/gtqzhmuhvm.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenlongwang.top/gtdxqeytvx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtunynifwl.html

C#:   f(a: 1, b: 2)
来源：http://hz.xingfuxueyuan.xyz/gtgmyzolgu.html

[C05] 返回多个值
来源：http://hz.cdnleiting.top/gtvykugtgk.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtengmqqut.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtjtwrxzny.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hongshengwenyu.top/gtjwuwfddd.html

TS:   return { a, b };
来源：http://hz.9152youxi.cn/gtqifuxrfm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuanzhike.top/gtlxossmmn.html

Go:   return a, b
来源：http://hz.cdnleiting.top/gtgvnsmmwa.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gtdfimibsp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pycfn.com/gtqnieuldw.html

[C06] 匿名函数 / lambda
来源：http://hz.9152youxi.cn/gtituskqbo.html

Py:   square = lambda x: x * x
来源：http://hz.cucudq.cn/gtkpexmxon.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gogol.net.cn/gtvjweryue.html

JS:   const square = x => x * x;
来源：http://hz.svipenyu.cn/gtrliorwcf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.tianlin.xyz/gtguddyuyp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shzxlz.cn/gtqdgxynig.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gtxfpodqwj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.9152youxi.cn/gteyirmpvm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnqzz.top/gtdvxfvqen.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtkqdlafab.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gtsmogizxt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhiwuduotai.top/gtfscdpdes.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtrwsdcszy.html

TS:   arr.map(String)
来源：http://hz.shuidangran.top/gtqwdtqopz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangshuangyany.cn/gtrzkbsikh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cucudq.cn/gtwadebrpp.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxinkj.top/gtiyrsmptq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sxryk.cn/gtaqicpdzw.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gthopfszpn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xinyue.icu/gttgctstob.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtbphoqwpm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gttgsxihyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtcakuhava.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtwwbndjtm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuanzx.com/gtkdtssdsp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pycfn.com/gtjardpgmo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtyshhjrkt.html

[C09] 递归
来源：http://hz.xingfuxueyuan.xyz/gtfyerrrza.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtbjjekzfj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jianghu66.top/gtnhghycca.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtevyixfes.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtucglkukk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hammf.cn/gtjrbicfpl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gtkhfqxcfi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtmkhyuozh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yongpay.top/gtemtcfxao.html

[C10] 变量作用域
来源：http://hz.tianlin.xyz/gtodzntubs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daria6918.cn/gtopivxchz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.vqdsnc.cn/gtvorfsotg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.52xcode.cn/gtzshuvxuy.html

TS:   同 JS
来源：http://hz.kuanghao11.cn/gtbwqohfym.html

Java: 方法内为块级作用域
来源：http://hz.xuetiantiany.cn/gttamrjivb.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtwcfcdaft.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtttclhcpe.html

C#:   块级作用域
来源：http://hz.cqqwz.cn/gtsfvekpls.html

[C11] 模块导入与导出
来源：http://hz.tianlin.xyz/gtlhmlkjgk.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtlbakxmjv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.316326.xyz/gtafejrwyz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtmuglfnke.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtzmkpsauq.html

Java: import java.util.List;
来源：http://hz.haohaochexian.top/gtthwyluok.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gotoacloud.top/gtbdkomkmu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gotoacloud.top/gtdoyblzbg.html

C#:   using System.Text;
来源：http://hz.andypj.xyz/gtwrubgpbz.html

[C12] 立即执行函数 IIFE
来源：http://hz.shzxlz.cn/gthuqqubss.html

Py:   (lambda: print("run"))()
来源：http://hz.jiagoushi.top/gtzqqlhywb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jianghu66.top/gtsizinxqa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtkjyfgfgr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtrtcilkdk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gtnvozbyit.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtfxlhhbfa.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtofdflvoz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtrgvtwzdx.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtvztfzfsg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.smart0.xyz/gtuajmfzns.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtqghauehx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yvedp.cn/gtlcdmxdry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtthnozovm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtszaryedl.html

Go:   func add(a, b int) int
来源：http://hz.jinqigufen.top/gtzjiymlgs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenjidiqi.icu/gtazpidtiw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gtfpnlkpbo.html

[C14] 泛型函数
来源：http://hz.nwbrower.top/gtjjrkpval.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.mhx1999.top/gtstyqylkr.html

PHP:  // 无泛型
来源：http://hz.cashguo.top/gtgqudikfk.html

JS:   // 无泛型
来源：http://hz.yj20258888.top/gttpsmuyqj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gogol.net.cn/gtoowplrjs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hammf.cn/gtbqgqqgzf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258888.top/gtqtdsisyk.html

Ruby: # 无泛型
来源：http://hz.guannengcc.top/gtrircceqb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtznkcoydb.html

[C15] 解构 / 展开参数
来源：http://hz.yuxming.cn/gtlzhclznf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gaohongyu789.top/gtjvwgkqov.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gtemslpwpn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtjzmrtioj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhoulong.xyz/gtcliodiri.html

Java: // 无解构
来源：http://hz.ydjk.org.cn/gtacjtrccw.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtgckwkpvw.html

Ruby: a, b = pair
来源：http://hz.fengsongda.top/gtwuxbkzkk.html

C#:   var (a, b) = pair;
来源：http://hz.sysykeji.top/gtprxelsze.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gtyvkwrnik.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuanzhike.top/gtvxnnietf.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtfeezrhns.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuxming.cn/gtqgnqchqd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtvegpqaie.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.0kj1m.cn/gtvnmrtiwy.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtivbntfzk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangdashe.top/gtrrmzguuk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ppjwa.cn/gtupxxbdlb.html

================================================================================
来源：http://hz.daxiang520.top/gtfzyvoysb.html

D. 数组 / 列表 / 集合
来源：http://hz.hfpthk.cn/gtvquepnub.html

================================================================================
来源：http://hz.hnqzz.top/gtbobhpwvk.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtxbubvmcu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtaxglklbb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtyiplqpsu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhoulong.xyz/gtexlmixoi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtcknnsqwp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tianlin.xyz/gtfjohfkhr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yvedp.cn/gtajncynlh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.0kj1m.cn/gtlfwefrgh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtxcikcdvt.html

[D02] 追加元素到末尾
来源：http://hz.yuanzhike.top/gttqakjybu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtqkewpuyg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daria6918.cn/gtpzjwnpnk.html

JS:   arr.push(4);
来源：http://hz.xuanzx.com/gtlemkpksy.html

TS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtedwidxss.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gtieyawxrn.html

Go:   arr = append(arr, 4)
来源：http://hz.yonumen.top/gtcklqnriv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtrwmvyrre.html

C#:   list.Add(4);
来源：http://hz.hnxiangtu.top/gtypswvrfy.html

[D03] 在指定位置插入元素
来源：http://hz.zhoulong.xyz/gtivuzudfz.html

Py:   arr.insert(0, 0)
来源：http://hz.cdnleiting.top/gtenpboguu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.bjfxy.top/gtkupepqun.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgufenzy.top/gtbcfryuzh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtpfzrnkiz.html

Java: list.add(0, 0);
来源：http://hz.meibo888.top/gtiysvgnkj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhijiandao.cn/gthkhohtht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenzaomai.com/gtltxvihsx.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigufen.top/gtuaaqjkov.html

[D04] 删除元素
来源：http://hz.aibaodan.cn/gtyfbvicyi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtsmlgtwsf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhiwuduotai.top/gtslldtylb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.haohaochexian.top/gthbtrbrqm.html

TS:   arr.splice(0, 1);
来源：http://hz.sufxvd.cn/gtgbjfgiht.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.316326.xyz/gttywlftsh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pengpengdd.cyou/gtuyezmxhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhengqikj.top/gtzzwzwams.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.haohaochexian.top/gtzurcwbow.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gteikueiwe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtxjmxjzkn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtijdkjwes.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtiynpdpjk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtvdcugpxx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtlstxzsnb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtwdpvihpy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtyfdrrxjs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gtuayoxcdg.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtjbxbpaiu.html

Py:   len(arr)
来源：http://hz.shangyingyoupin.top/gtquominsq.html

PHP:  count($arr);
来源：http://hz.9152youxi.cn/gtvfxsfxxv.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtpoellxmp.html

TS:   arr.length
来源：http://hz.pengpengdd.cyou/gtbywctsvt.html

Java: list.size();
来源：http://hz.jqgufenzy.top/gtdufzxxic.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gttejucmtz.html

Ruby: arr.length; arr.size
来源：http://hz.gotoacloud.top/gtmovljpyu.html

C#:   list.Count;
来源：http://hz.birdmap.top/gtvtrglgrn.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gtaqxaixtb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtyxbnzpkq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xinyue.icu/gttofrsvnp.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtnowatklo.html


<!-- 参考信息 -->