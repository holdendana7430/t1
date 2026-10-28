代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yueranfly.top/gtvupmsuff.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.redwolf501.top/gtxjsvcljg.html

[B07] while 循环
来源：http://hz.zhixingplan.top/gtnvzuendi.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtmsztvvpq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ydjk.org.cn/gtlqjobmir.html

JS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtcdtkczpm.html

TS:   while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtgihbxceq.html

Java: while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtweoczylh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cashguo.top/gtrlnoazka.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nanxinkj.top/gtbwisriap.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtgfiykqpm.html

[B08] do-while（至少执行一次）
来源：http://hz.daxiang520.top/gtnmtewhcp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jianghu66.top/gtqbukfifa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhengqikj.top/gtovgpnuot.html

JS:   do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtkebpwnkt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gticdixstr.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhixingplan.top/gthdvaguzc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shanyushiyangtech.top/gtymlfxxpi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.52xcode.cn/gtnproxtps.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtsexwgdkl.html

[B09] break 与 continue
来源：http://hz.nanxinkj.top/gtkjmlgsej.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dianchejie.cn/gtdpkgkpcm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gzhubu.top/gtvbxyfqni.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtrrmibymh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtuhpjkyvb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zycfv.cn/gtiuucobuw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhengqikj.top/gtianzesck.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ehwqpu.com/gtgfusjyzu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtxaekzdcz.html

[B10] 遍历同时拿索引
来源：http://hz.fengsongda.top/gtlcrukfnq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hywenlv.cn/gtbxotjcre.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtpliobyhm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.quarkkingdee.top/gturpdjgcf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ppjwa.cn/gttdpicqrs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtcprqiwbe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.daria6918.cn/gtwqkxszez.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.daria6918.cn/gtpqzbncyw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cashguo.top/gtahagfhai.html

[B11] 生成数字序列 / 区间
来源：http://hz.sxryk.cn/gtdkudkjnr.html

Py:   list(range(0, 10, 2))
来源：http://hz.316326.xyz/gtjrhvkoys.html

PHP:  range(0, 10, 2);
来源：http://hz.tian-w.cn/gtthprxqvp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtegmmiajq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gttozzyuhd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgfzy.top/gtfmxeiahd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtyemfcpvh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtbmvennyz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuetiantiany.cn/gtsnpcqzzv.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtbntsrpje.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.havefunace.top/gtuefcjarf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.vqdsnc.cn/gteueluhwb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtlffjrsbh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtrufqmabz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtmvatvjhp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sufxvd.cn/gtrzifchrs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guannengcc.top/gtqcimssbv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.snrcjt.cn/gtgpvqkzbw.html

[B13] 判断是否为数字
来源：http://hz.jinqigfzy.top/gtlqivknfk.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangtech.top/gtzvkbvejg.html

PHP:  is_numeric($x)
来源：http://hz.yueranfly.top/gtzaqplnre.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtsscoiixq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtyeixujtd.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gtjrqucdwv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinghuilouyu.cn/gtndukcanb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jlsjyb.cn/gtdocjapyd.html

C#:   x is int or double or decimal
来源：http://hz.tianlin.xyz/gtvwalheot.html

[B14] 判断值是否在集合内
来源：http://hz.feifeiyinyue.top/gtqupgpkvl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nanxinkj.top/gtsavjonwf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangdashe.top/gtbrjqxole.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtzjuqcpdt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtiwpdcwik.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhijiandao.cn/gtxpdsdrhv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtozqaxnns.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtrnmbeuxs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shzxlz.cn/gtypykwfvf.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gtsmupciqq.html

Py:   a and b or not c
来源：http://hz.yongpay.top/gtwmsjnaoy.html

PHP:  $a && $b || !$c
来源：http://hz.ivvv.top/gtikulmrnh.html

JS:   a && b || !c
来源：http://hz.yongpay.top/gtlzbppulh.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtutywsome.html

Java: a && b || !c
来源：http://hz.daxiang520.top/gtnqhvlrid.html

Go:   a && b || !c
来源：http://hz.hywenlv.cn/gtlqsefujf.html

Ruby: a && b || !c
来源：http://hz.xuetiantiany.cn/gtuuzhymzz.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtngsttocf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guowangkeji.top/gtwfxzraxh.html

Py:   if not data: return
来源：http://hz.zhaomingkeji.xyz/gtgwcwbzjc.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gtunqkrlqq.html

JS:   if (!data) return;
来源：http://hz.daxiang520.top/gtdvzdzgrh.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gttrnqjoga.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gthxjfhzwk.html

Go:   if data == nil { return }
来源：http://hz.tianlin.xyz/gtutoagcoa.html

Ruby: return if data.nil?
来源：http://hz.mhx1999.top/gtpwmovwrg.html

C#:   if (data == null) return;
来源：http://hz.gzhubu.top/gtkjagxyzt.html

================================================================================
来源：http://hz.jinqigufen.top/gtrvxlqypp.html

C. 函数与作用域
来源：http://hz.xziqi.cn/gtskbuzqwj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjaktacbt.html

[C01] 定义函数
来源：http://hz.zhoulong.xyz/gtvyynqqqx.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigfzy.top/gthczuanah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gteqnzcsmm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gtdmhbvgis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtblcyqare.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtuqcrabdx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ywan-chungtsiang.top/gttwfxbrgo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guowangkeji.top/gtxlohjiln.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtsvuaetga.html

[C02] 默认参数
来源：http://hz.mhx1999.top/gtvkuychgl.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258.top/gtpdlbwlxa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cheryme.top/gtyvkcetvj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cheryme.top/gtmamlbaxg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xingfuxueyuan.xyz/gttfstvsso.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtxajxiimh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gtgaasqhkj.html

Ruby: def greet(name = "World") = name
来源：http://hz.ybcxt.top/gttunsqqnh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnxiangtu.top/gtqwecufwj.html

[C03] 可变参数
来源：http://hz.guannengcc.top/gtqvuqoyno.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtmxwkvvnf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gtgmghxewp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtmvlrgmpd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtpbxgspai.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.9152youxi.cn/gtuweowxtc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigufen.top/gtaknzskis.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.meibo888.top/gtktfctaja.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.iojbl.cn/gtckxhssfx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.smart0.xyz/gtmtgvwolk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.316326.xyz/gtyxjfpqjr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhiwuduotai.top/gtsvtjyejc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtrgkvjmyk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gthgdwymqd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtlabdhshf.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gthuntjcqs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtpmqhjkwq.html

C#:   f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtgppexfwl.html

[C05] 返回多个值
来源：http://hz.yongpay.top/gtslpspozv.html

Py:   return a, b
来源：http://hz.shangyingyoupin.top/gthbglennk.html

PHP:  return [$a, $b];
来源：http://hz.zycfv.cn/gtloxscmuj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtvxddkbgi.html

TS:   return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtyisvwcnk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gtdlponudh.html

Go:   return a, b
来源：http://hz.pycfn.com/gtmwngiqvv.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gtjzwrqkpu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hywenlv.cn/gtopdtabvd.html

[C06] 匿名函数 / lambda
来源：http://hz.ivvv.top/gtrpljjplh.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtwiowlgdq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuanzx.com/gtfpudgyih.html

JS:   const square = x => x * x;
来源：http://hz.daria6918.cn/gtxcvmyquw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gthifcoxhd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinyuanbaomall.cn/gtbswkyhcx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gzhubu.top/gtmsdwuarz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gtthieosuh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtalwvwqql.html

[C07] 把函数作为参数传入
来源：http://hz.jianghu66.top/gtjralxotr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gtyeetulaq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgufenzy.top/gtkxvvuvde.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tanke756.top/gtgkehxpwx.html

TS:   arr.map(String)
来源：http://hz.xuetiantiany.cn/gtdxsedaop.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.havefunace.top/gtrsxtwgoe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuanzhike.top/gtppwekuwv.html

Ruby: arr.map(&:upcase)
来源：http://hz.hammf.cn/gtnnfkbraq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jiagoushi.top/gtpfnjzpdn.html

[C08] 闭包
来源：http://hz.wangdashe.top/gtsmzbgkff.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhengqikj.top/gtbdgqwhnh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xziqi.cn/gtauanzdjg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtjzahfqxp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtdfxmvrma.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigufen.top/gtxjjmfjdw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shzxlz.cn/gtuyhipntr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.vqdsnc.cn/gtkeudckvz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtnlvllrgy.html

[C09] 递归
来源：http://hz.yvedp.cn/gtdtdygpft.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gthzzbbadu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuanzx.com/gtndskrlhw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtjnbhcmbs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtwiskkdya.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xziqi.cn/gtwasploqf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtxkxriuuu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtdacjuzhq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hysaishi.cn/gtfobycpnj.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gtrkazqzji.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtqzdkgmxy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhoulong.xyz/gtjqujqggi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.52xcode.cn/gtkaqroaan.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtygnehzcd.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtnfbyvpui.html

Go:   花括号块级作用域
来源：http://hz.pengpengdd.cyou/gtiuztnrol.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aibaodan.cn/gtnkdfktob.html

C#:   块级作用域
来源：http://hz.gaohongyu789.top/gtjbdrgdsn.html

[C11] 模块导入与导出
来源：http://hz.9152youxi.cn/gtfgstcyqj.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtooildfsj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtghldegej.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tanke756.top/gtgrrraizr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtausgrsti.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gttsfdqdmg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtbdcgqgqn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtedghdenw.html

C#:   using System.Text;
来源：http://hz.yuanzhike.top/gthnworfsm.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtlauvcrdx.html

Py:   (lambda: print("run"))()
来源：http://hz.snrcjt.cn/gtxhprlmhd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxinkj.top/gtlogtqyxg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gthlgnwpzw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gtgyvjqtzy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gtgfqoursf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtxfomlzwv.html

Ruby: -> { puts "run" }.call
来源：http://hz.yangfankeji.com/gtlzgemuny.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtvarhrhdx.html

[C13] 类型声明 / 类型注解
来源：http://hz.shzxlz.cn/gtksibcrpi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.redwolf501.top/gtdvvicsed.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtdflwynzo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ppjwa.cn/gtnfcvbjhs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtohxftjwa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtaqdyneya.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtfgteectd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtqldtkfpr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtilwemdpq.html

[C14] 泛型函数
来源：http://hz.xingfuxueyuan.xyz/gtkmmqlotg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtzdtwyzxk.html

PHP:  // 无泛型
来源：http://hz.ybcxt.top/gtobwzafpp.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtnvtxyrup.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtkbhtysgx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gtkrqiozrv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtrvfrtpka.html

Ruby: # 无泛型
来源：http://hz.svipenyu.cn/gtymbtnoda.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtpspcdavo.html

[C15] 解构 / 展开参数
来源：http://hz.cdnleiting.top/gtrryudfoz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cucudq.cn/gtqabigysm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.birdmap.top/gtotkvggsp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtkcopvhtj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtgysjnjiv.html

Java: // 无解构
来源：http://hz.nanxinkj.top/gtfovuzkrt.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtsfoizrah.html

Ruby: a, b = pair
来源：http://hz.jinghuilouyu.cn/gtuaxgdxhf.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gtgiaawott.html

[C16] 函数 / 方法重载
来源：http://hz.ivvv.top/gtpkysxsku.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtsdtbxdnz.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtpniolhpz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aizwys.cn/gtdloapmlo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtxoroyowq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gttwdaogvo.html

Go:   // 无重载：用不同函数名
来源：http://hz.sufxvd.cn/gtdsskvtkm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jyoumei.cn/gtiuprcaev.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinghuilouyu.cn/gtcsizrhmf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmnfrudvv.html

D. 数组 / 列表 / 集合
来源：http://hz.jyoumei.cn/gtkfwcanpg.html

================================================================================
来源：http://hz.52xcode.cn/gtjydqtwxv.html

[D01] 创建数组 / 列表
来源：http://hz.snrcjt.cn/gtorfsomdy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gttxtubqed.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtilvkveah.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gthrdycnnt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jlsjyb.cn/gtmymmmjbu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtawiiykjs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yanxiufei.cn/gtakckmhds.html

Ruby: arr = [1, 2, 3]
来源：http://hz.birdmap.top/gtujusdpwe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jyoumei.cn/gtfmyqozgs.html

[D02] 追加元素到末尾
来源：http://hz.yvedp.cn/gtyzdwgnkl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guannengcc.top/gtkhafqzdk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtqxkefnkz.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gthpcqbsyz.html

TS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtqenqcgiz.html

Java: list.add(4);
来源：http://hz.ydzc1.top/gtampxltbr.html

Go:   arr = append(arr, 4)
来源：http://hz.wangshuangyany.cn/gtjpgzazfz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xziqi.cn/gtxkhycfav.html

C#:   list.Add(4);
来源：http://hz.fzhhl.top/gtlqfgypva.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtxdlevxay.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtdoubblum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.kuanghao11.cn/gtyecyynmu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shzxlz.cn/gtrtmeovvb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ivvv.top/gtycfiuldv.html

Java: list.add(0, 0);
来源：http://hz.yuxming.cn/gtsicyxtrn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.9152youxi.cn/gtdqemuqxy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gtbflbpdlh.html

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gtreislybv.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gttvvhijfi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jiagoushi.top/gtrxobdhtj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtjmocncoc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gttmofaxwp.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtapwgrqlc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtuqoqqkam.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtiswtdfqd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangshuangyany.cn/gtsdupvgbv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtpvgpsfoy.html

[D05] 访问与修改元素
来源：http://hz.yj202588.top/gtdbvkhzxw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtbwszhfzi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.dashuyun.cn/gtyzsyudmf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtoiswzyfu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shangyingyoupin.top/gtzgqaochu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhaomingkeji.xyz/gtzvxtitqg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtabndvvmu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtmcdipbkb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhixingplan.top/gtgfjxbfwu.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gtfjwccxtn.html

Py:   len(arr)
来源：http://hz.wangdashe.top/gtuxgcrdlz.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gtsnhnhwsq.html

JS:   arr.length
来源：http://hz.quarkkingdee.top/gtunxrpivl.html

TS:   arr.length
来源：http://hz.feifeiyinyue.top/gthoubtdqv.html

Java: list.size();
来源：http://hz.fengsongda.top/gtznloetly.html

Go:   len(arr)
来源：http://hz.jyoumei.cn/gtelunrvgm.html

Ruby: arr.length; arr.size
来源：http://hz.sufxvd.cn/gtrxqftgtg.html

C#:   list.Count;
来源：http://hz.quarkkingdee.top/gtjeiqhjyv.html

[D07] 切片 / 取子数组
来源：http://hz.quarkkingdee.top/gtrzvdpdcj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ywan-chungtsiang.top/gthallfdrc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtxegtzhmx.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtxppmrrjb.html


<!-- 参考信息 -->