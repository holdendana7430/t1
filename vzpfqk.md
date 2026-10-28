代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuetiantiany.cn/gtsrvtgaeu.html

JS:   while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtieyjqmzx.html

TS:   while (i < 10) { i++; }
来源：http://hz.ehwqpu.com/gtmcyqzswa.html

Java: while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtksjbtigv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinyuanbaomall.cn/gtmhxttejl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinyuanbaomall.cn/gtwpsiasqf.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtounduypl.html

[B08] do-while（至少执行一次）
来源：http://hz.hnqzz.top/gtfqbiaxgc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenlongwang.top/gtzaxybcmg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ydzc1.top/gtnqwdsmlj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gttxxgavwr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gticbahljb.html

Java: do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtfxduhuug.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.snrcjt.cn/gthndydzaq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sxryk.cn/gtvcdguwqc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtlfspwzml.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtckuuqihe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pengpengdd.cyou/gtfkoxraod.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigfzy.top/gtmmbnvayk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gteogaczlg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtcidmumju.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtadyjeqqj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenlongwang.top/gtagtkiyhf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shzxlz.cn/gtqyurhqmz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtqxsnlefz.html

[B10] 遍历同时拿索引
来源：http://hz.ydzc1.top/gtmtmfoste.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.svipenyu.cn/gttxmiibqs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cashguo.top/gteywwdrxx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhiwuduotai.top/gtgjttjhnf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhengqikj.top/gtdvnsfmeg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.chenjidiqi.icu/gtgktuoxpe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hysaishi.cn/gtyusyotqu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.9152youxi.cn/gtentvxaky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.birdmap.top/gtxgitjrua.html

[B11] 生成数字序列 / 区间
来源：http://hz.havefunace.top/gttnrrhjkl.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenjidiqi.icu/gtkzqngpny.html

PHP:  range(0, 10, 2);
来源：http://hz.nanxuanxn.top/gtndfkmnsy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ivvv.top/gtyqggyywz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cqqwz.cn/gtenemboak.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gtbqbqbnho.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yvedp.cn/gtvsnklahp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dashuyun.cn/gtnugsusif.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ppjwa.cn/gtqdocdbzy.html

[B12] 跳出多层循环
来源：http://hz.zhaomingkeji.xyz/gtkrbvwkhe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.dashuyun.cn/gtryaqtmwy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gtlsgelxgb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtdmcxuain.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gthcozynte.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtsskiimpy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.pengpengdd.cyou/gtpqkfxijb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tian-w.cn/gtugfasver.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.quarkkingdee.top/gtovmmvegc.html

[B13] 判断是否为数字
来源：http://hz.svipenyu.cn/gttquhtyth.html

Py:   isinstance(x, (int, float))
来源：http://hz.nwbrower.top/gtaqxppghw.html

PHP:  is_numeric($x)
来源：http://hz.yj20258.top/gtasmvmzhd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gttshhpzoe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gthihckpna.html

Java: x instanceof Number
来源：http://hz.0kj1m.cn/gtuilnelgc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.c1oappe.top/gtsacjwscp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.redwolf501.top/gtazzsatgd.html

C#:   x is int or double or decimal
来源：http://hz.jyoumei.cn/gttkyjmlsm.html

[B14] 判断值是否在集合内
来源：http://hz.shangyingyoupin.top/gtldgjerza.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuanzx.com/gtbtikzmjz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sxryk.cn/gttfkscydf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtwqwhutfr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtefaavrwc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtvojvttqp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuetiantiany.cn/gtgxcucgzq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuanzx.com/gtcmthswtg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.52xcode.cn/gtokkforfs.html

[B15] 布尔运算与取反
来源：http://hz.hnxiangtu.top/gtiipiexdb.html

Py:   a and b or not c
来源：http://hz.vqdsnc.cn/gtxarwzomc.html

PHP:  $a && $b || !$c
来源：http://hz.yvedp.cn/gtnirkabws.html

JS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtmqziblmv.html

TS:   a && b || !c
来源：http://hz.ehwqpu.com/gtvzxingko.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtbtinrqkd.html

Go:   a && b || !c
来源：http://hz.ppjwa.cn/gtcbwfslab.html

Ruby: a && b || !c
来源：http://hz.52xcode.cn/gtdfsqitbl.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtrpiftbmw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tianlin.xyz/gtjgvapffd.html

Py:   if not data: return
来源：http://hz.sweek.top/gturhrwesf.html

PHP:  if (!$data) { return; }
来源：http://hz.shanyushiyangkeji.top/gtueqekzqi.html

JS:   if (!data) return;
来源：http://hz.andypj.xyz/gtquqpqfeu.html

TS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtwkuzadvb.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gtoruxebgv.html

Go:   if data == nil { return }
来源：http://hz.ydzc1.top/gtchpquuvd.html

Ruby: return if data.nil?
来源：http://hz.nanxuanxn.top/gtbvxhsurq.html

C#:   if (data == null) return;
来源：http://hz.shuidangran.top/gtjyjbayde.html

================================================================================
来源：http://hz.andypj.xyz/gtpwaywrio.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtxhbggven.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjtsvuxoi.html

[C01] 定义函数
来源：http://hz.xziqi.cn/gtlhtdhogr.html

Py:   def add(a, b): return a + b
来源：http://hz.hysaishi.cn/gtyobwmoib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gttmgfzxqg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtuctnmorv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtlrfifvjo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtojrdzvfk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cheryme.top/gthgssauja.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jiagoushi.top/gtlyrlsncw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtnvtsaygn.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtzwaqhmng.html

Py:   def greet(name="World"): return name
来源：http://hz.chenjidiqi.icu/gtnvvtljuq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydzc1.top/gtygywvobw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtemjuykma.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtaigdgibu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shuidangran.top/gthizznlnq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtrbsmfnbi.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhiwuduotai.top/gtuoxeiksz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gtpzjnuzst.html

[C03] 可变参数
来源：http://hz.nanxinkj.top/gtftteytnc.html

Py:   def total(*args): return sum(args)
来源：http://hz.daria6918.cn/gtpalwxuil.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangdashe.top/gtpmyivesr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtscdwsqbq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtvuvfxenn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydjk.org.cn/gtfswhczij.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnxiangtu.top/gtwagvkpro.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258.top/gtxmzcfdxo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtgwnqdbfp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sysykeji.top/gtvvwatjqw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtgitheldo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj202588.top/gtovbsullq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtbaqtoloj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangdashe.top/gtiujfizol.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtcdroytyk.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtjxinhima.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtdkckszue.html

C#:   f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtlgfuoacr.html

[C05] 返回多个值
来源：http://hz.tian-w.cn/gtaxaorzpm.html

Py:   return a, b
来源：http://hz.yj202588.top/gtrtacrkgu.html

PHP:  return [$a, $b];
来源：http://hz.snrcjt.cn/gtlbcoswnt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxinkj.top/gtaqseqohl.html

TS:   return { a, b };
来源：http://hz.yuxming.cn/gthjuzkqno.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.meibo888.top/gtrrhltweh.html

Go:   return a, b
来源：http://hz.cqqwz.cn/gtsylszzbd.html

Ruby: return a, b
来源：http://hz.zhaomingkeji.xyz/gtntrrjxey.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yanxiufei.cn/gtrjrgyonv.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gtqwavtcrn.html

Py:   square = lambda x: x * x
来源：http://hz.chenjidiqi.icu/gtbaqlnbpv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtquhnejuc.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gthynnqdew.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtpvscnxjj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.c1oappe.top/gtxbckjovf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxuanxn.top/gtqnusdwgm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtgnrvfope.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtperqturj.html

[C07] 把函数作为参数传入
来源：http://hz.316326.xyz/gttcsojkmr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gthnlojzic.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ivvv.top/gtxtxnsgbl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtlkauikqc.html

TS:   arr.map(String)
来源：http://hz.cucudq.cn/gtdztrdxzg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yonumen.top/gtwgkjejww.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.birdmap.top/gtktxiplym.html

Ruby: arr.map(&:upcase)
来源：http://hz.hammf.cn/gthwhetdjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtwcwpxvts.html

[C08] 闭包
来源：http://hz.zhongyouzk.top/gtbrtbdgzn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtitamdcil.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydjk.org.cn/gtagijdvit.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtpdlxoiog.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtpgkqfqhx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinghuilouyu.cn/gtuemabaac.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.dashuyun.cn/gtnxrobvpk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj202588.top/gtlndxxnpa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtirvqlozz.html

[C09] 递归
来源：http://hz.andypj.xyz/gtnswbxoav.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aizwys.cn/gtgieuurqx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.svipenyu.cn/gtjtencihs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtdfbvbryy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtbiozfqko.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtjivvrsjm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gttndgeckt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jianghu66.top/gtssibfier.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtfswmplqf.html

[C10] 变量作用域
来源：http://hz.aizwys.cn/gtutpfxuyj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dianchejie.cn/gtlxvgjhbv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gttqenehdf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinghuilouyu.cn/gthgrusilo.html

TS:   同 JS
来源：http://hz.jlsjyb.cn/gtqaxcqqgg.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtxeqideww.html

Go:   花括号块级作用域
来源：http://hz.gotoacloud.top/gtvhyehxun.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tianlin.xyz/gtlturvlgn.html

C#:   块级作用域
来源：http://hz.wangshuangyany.cn/gtqpattpfb.html

[C11] 模块导入与导出
来源：http://hz.yuxming.cn/gtnqzgidcn.html

Py:   from module import func
来源：http://hz.gaohongyu789.top/gtjfsenybb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cucudq.cn/gtqcdompmc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jianghu66.top/gtitkuxykn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtnmbeyeud.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtbbsrvswg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtikrrihrj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhiwuduotai.top/gtoihctnoi.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtbwnbtfqw.html

[C12] 立即执行函数 IIFE
来源：http://hz.cheryme.top/gtkpbtsjst.html

Py:   (lambda: print("run"))()
来源：http://hz.chenjidiqi.icu/gtneqjfhww.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgufenzy.top/gtejxvgtac.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtrfubowod.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtznmtumll.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.quarkkingdee.top/gtalacofod.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtyforosml.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtxejbwbef.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ydjk.org.cn/gtsgjrnyaf.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtjjryytfq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.mhx1999.top/gtjsedsmvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtpnqefqli.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtwzdrokfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gtwrmuleof.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtxidhfpvf.html

Go:   func add(a, b int) int
来源：http://hz.nanxuanxn.top/gtvaynvweg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gthsryicwj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtnjfocwwx.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtugodfzxo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuxming.cn/gtecxowuan.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gtueyniqrb.html

JS:   // 无泛型
来源：http://hz.iojbl.cn/gtkmugdqej.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtnamcuqwl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gtdhmbmwqh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.vqdsnc.cn/gtcsziufmg.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtaxgjxtci.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gtoqywadss.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtbpcbpthw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnqzz.top/gtzooxoglb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtneypgnma.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.birdmap.top/gtnnsjbmjn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xziqi.cn/gtofyjezif.html

Java: // 无解构
来源：http://hz.aibaodan.cn/gtifmykiwe.html

Go:   // 无解构
来源：http://hz.shanyushiyangtech.top/gtocssgedv.html

Ruby: a, b = pair
来源：http://hz.zhaomingkeji.xyz/gtponefglx.html

C#:   var (a, b) = pair;
来源：http://hz.cheryme.top/gtcipiscfh.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtuayziyli.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtzyosuhok.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtjrfevtgy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtplmnjndz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yongpay.top/gtyudcqwow.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xziqi.cn/gtjrbrzfca.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtaykwuvjy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgufenzy.top/gtuimniwbg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gttgukecww.html

================================================================================
来源：http://hz.ivvv.top/gtqjillwwf.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtfyyourug.html

================================================================================
来源：http://hz.cdnleiting.top/gtiaujhjxm.html

[D01] 创建数组 / 列表
来源：http://hz.yuxming.cn/gtsuysgxjg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guowangkeji.top/gtfidglywn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtbckoqaxv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ivvv.top/gtylgxkyne.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.aibaodan.cn/gtquqqdkxg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtcbefezzx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtqomwltdl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgfzy.top/gthutqeanj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangdashe.top/gtbrzjreeu.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtyzepbhwo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zdqjudy.top/gtxrxvmjfy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cdnleiting.top/gtrjhentrn.html

JS:   arr.push(4);
来源：http://hz.sxryk.cn/gtyrnseusk.html

TS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtgdnqrkzm.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtkmyjgoza.html

Go:   arr = append(arr, 4)
来源：http://hz.xziqi.cn/gtfcbdzleh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.wangdashe.top/gtzxaykdnb.html

C#:   list.Add(4);
来源：http://hz.xuanzx.com/gtozyojmor.html

[D03] 在指定位置插入元素
来源：http://hz.ywan-chungtsiang.top/gtdhyioreo.html

Py:   arr.insert(0, 0)
来源：http://hz.9152youxi.cn/gtgufucylo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtbyarwkdw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhiwuduotai.top/gtcmehktdy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtdpjpkroo.html

Java: list.add(0, 0);
来源：http://hz.quarkkingdee.top/gtojxoftug.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtwmkvyfsh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hammf.cn/gthwcofbmh.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtrirtztfv.html

[D04] 删除元素
来源：http://hz.jinyuanbaomall.cn/gtbatppfsb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zdqjudy.top/gtcsxpdyez.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtigmaytvr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gtuscefvrp.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtmgflqsvl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guowangkeji.top/gtadxjknai.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtdqtwtehx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.bjfxy.top/gthcpmfuso.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenlongwang.top/gtwuntsxzm.html

[D05] 访问与修改元素
来源：http://hz.hongshengwenyu.top/gtvgmfdbww.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtjwyseeet.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuanzhike.top/gtzwbsabdp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jiagoushi.top/gtiutlewur.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jianghu66.top/gteyohardg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.feifeiyinyue.top/gtsicjifco.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtsdymuwxv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtrdwcdzkl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtkievuqah.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gthtgbsfse.html

Py:   len(arr)
来源：http://hz.hongshengwenyu.top/gtfiljutga.html

PHP:  count($arr);
来源：http://hz.shuidangran.top/gtbhzypbbs.html

JS:   arr.length
来源：http://hz.zhoulong.xyz/gtmrsvsqye.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtkuhxtglp.html

Java: list.size();
来源：http://hz.jqgfzy.top/gtizytgcnh.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gtkqwfphfd.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtwvcwsadb.html

C#:   list.Count;
来源：http://hz.316326.xyz/gtlhldrrpm.html

[D07] 切片 / 取子数组
来源：http://hz.gaohongyu789.top/gtvgdsckxk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.vqdsnc.cn/gtmffivdwl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigfzy.top/gttbdoewkd.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtifhebphq.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtnezvubgf.html

Java: list.subList(1, 4);
来源：http://hz.shangyingyoupin.top/gtydamzxse.html

Go:   arr[1:4]
来源：http://hz.hnqzz.top/gtseqoxqcw.html

Ruby: arr[1, 3]
来源：http://hz.daria6918.cn/gtvmkunygr.html


<!-- 参考信息 -->