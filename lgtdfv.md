代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtuokecndk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtrqbhbsuv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xziqi.cn/gtsnudjtnv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.guannengcc.top/gtdqchmfmt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtjntlthbe.html

[B10] 遍历同时拿索引
来源：http://hz.wangshuangyany.cn/gtgorrtswe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yuanzhike.top/gtlppthpby.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cqqwz.cn/gtvvxasyar.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jyoumei.cn/gtudeiyjcf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.pycfn.com/gtjdxaupag.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guowangkeji.top/gtvtlwzsng.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinghuilouyu.cn/gtrpvfxukd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenlongwang.top/gtdxqjwqub.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.haohaochexian.top/gtimvkigxs.html

[B11] 生成数字序列 / 区间
来源：http://hz.ydzc1.top/gttjmvgmvr.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtutmxbzjj.html

PHP:  range(0, 10, 2);
来源：http://hz.hfpthk.cn/gtgsknojoc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtgxttzkqy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtpjwiwknq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtlemanpyr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fengsongda.top/gttpxngmxf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shangyingyoupin.top/gtrjzacrtm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtltzsmihb.html

[B12] 跳出多层循环
来源：http://hz.xylfe.cn/gtmkdyinmz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtyfdfjgjs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.kuanghao11.cn/gtbnmoyewj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtptrkoqum.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtsbnuypnl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtbnwpcyei.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xinyue.icu/gtojxfkjnd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxinkj.top/gthevqywks.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dianchejie.cn/gtwllibwfq.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtgnzwehkz.html

Py:   isinstance(x, (int, float))
来源：http://hz.gaohongyu789.top/gtbrbsnfvr.html

PHP:  is_numeric($x)
来源：http://hz.c1oappe.top/gtutjwhpbx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtbwnempvp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtaaqiddpk.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtbfzvinow.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gtwpduaofp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hywenlv.cn/gtlggqclrr.html

C#:   x is int or double or decimal
来源：http://hz.nanxinkj.top/gtdnwoamsn.html

[B14] 判断值是否在集合内
来源：http://hz.hnxiangtu.top/gtbugnebfn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ydjk.org.cn/gtwoabitvd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.bjfxy.top/gtbirnscus.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nanxinkj.top/gtyyiegosi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtrcuwgacs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigufen.top/gtwsxqvnnp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sysykeji.top/gtzkxeewbc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yongpay.top/gtvxyqdtsd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuanzx.com/gtsdcecrfg.html

[B15] 布尔运算与取反
来源：http://hz.316326.xyz/gttpamvnko.html

Py:   a and b or not c
来源：http://hz.gotoacloud.top/gtpainqwxb.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gtiuagomja.html

JS:   a && b || !c
来源：http://hz.yuxming.cn/gtzkszqrul.html

TS:   a && b || !c
来源：http://hz.dianchejie.cn/gtbqgrsmfd.html

Java: a && b || !c
来源：http://hz.hywenlv.cn/gtyjlpsvzg.html

Go:   a && b || !c
来源：http://hz.hammf.cn/gthcbtdryz.html

Ruby: a && b || !c
来源：http://hz.fzhhl.top/gtsnxtlwes.html

C#:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gttkfelomd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tian-w.cn/gtfhthguaa.html

Py:   if not data: return
来源：http://hz.havefunace.top/gtdeezkwrf.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtgbkwwbtk.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gtlbqsjjej.html

TS:   if (!data) return;
来源：http://hz.svipenyu.cn/gtpcmfglpw.html

Java: if (data == null) return;
来源：http://hz.andypj.xyz/gtpvisevxg.html

Go:   if data == nil { return }
来源：http://hz.ehwqpu.com/gtxqzseggq.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtsdfjzkej.html

C#:   if (data == null) return;
来源：http://hz.jqgfzy.top/gttcoipwqf.html

================================================================================
来源：http://hz.pycfn.com/gtqsluaiee.html

C. 函数与作用域
来源：http://hz.guowangkeji.top/gtbhluzhko.html

================================================================================
来源：http://hz.yanxiufei.cn/gtozicdwyo.html

[C01] 定义函数
来源：http://hz.jiagoushi.top/gtohxfgdgw.html

Py:   def add(a, b): return a + b
来源：http://hz.fzhhl.top/gtqrxqbkeh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtfxtrtwmy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.9152youxi.cn/gtwkpowlaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtzlhlqlgd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtksyxqvdy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtqynnenlx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuxming.cn/gtfskhtort.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtxoubtjqs.html

[C02] 默认参数
来源：http://hz.gotoacloud.top/gtfjjtduzx.html

Py:   def greet(name="World"): return name
来源：http://hz.redwolf501.top/gtwxeglcbz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtnbgvnspp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtyzlnxmyt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sufxvd.cn/gtizdkvigh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtwswsoocf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhengqikj.top/gtsyecmskv.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtdyvbbyvo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gteiqymqlb.html

[C03] 可变参数
来源：http://hz.yanxiufei.cn/gtyvperfjr.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gtchrwkjkt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhixingplan.top/gtjinkqjqt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtgatkvqnr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtmdhjtusm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cheryme.top/gteqvhlcza.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ehwqpu.com/gthgrzrgbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtpbcaxger.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.meibo888.top/gtbltauqrh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj202588.top/gtllpmtwrc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtbbckbkpv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shangyingyoupin.top/gtsigkcjoc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtpxvqnhos.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.iojbl.cn/gtpamjygop.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cqqwz.cn/gtheokwygu.html

Go:   // 无：用配置结构体参数
来源：http://hz.shangyingyoupin.top/gtpovkuviw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guowangkeji.top/gtqmdjszvu.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtusowwxzi.html

[C05] 返回多个值
来源：http://hz.zhaomingkeji.xyz/gtiolfzyug.html

Py:   return a, b
来源：http://hz.ivvv.top/gtcdoclpmk.html

PHP:  return [$a, $b];
来源：http://hz.cashguo.top/gtxszanrws.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtsselqmvf.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtkdxfnzlf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangdashe.top/gtuxlarfkh.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtcsfnwrmv.html

Ruby: return a, b
来源：http://hz.jiagoushi.top/gthqyadoku.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tianlin.xyz/gtjyaxnchv.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtkyswnqvu.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtvjjfrhfx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhengqikj.top/gtdilbdfbx.html

JS:   const square = x => x * x;
来源：http://hz.cqqwz.cn/gtdyrennul.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinqigufen.top/gtitnnqcfm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cdnleiting.top/gtfchdnjau.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenjidiqi.icu/gtjedmsmca.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtasexjdra.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.feifeiyinyue.top/gtsjaumngn.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigfzy.top/gteigujkvq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yongpay.top/gtlecebepy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtvvazoxnv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.haohaochexian.top/gtukkmnfqk.html

TS:   arr.map(String)
来源：http://hz.yueranfly.top/gtxlhmmsij.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenjidiqi.icu/gtdyyloyqc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hywenlv.cn/gtxewtmesf.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258.top/gtxviwdlty.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tian-w.cn/gtcicacbdk.html

[C08] 闭包
来源：http://hz.jinghuilouyu.cn/gtrcdjvqyk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.316326.xyz/gtvmtzhoih.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gthbreksyv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtowjytcro.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtzjdngsno.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtpdtocqia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtzvudgocy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gtlidcfmom.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtmniemdvy.html

[C09] 递归
来源：http://hz.shanyushiyangtech.top/gtqmostkfs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtnkjhpdhx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ybcxt.top/gtszvsbowf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtmmndbjth.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gtyxcoawoe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangdashe.top/gtxygzfbvv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtdnosbhmg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtsejxquun.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtwuyqmseh.html

[C10] 变量作用域
来源：http://hz.xingfuxueyuan.xyz/gtmirhsffy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gttegbdaoh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtyfgtcjku.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtpbkhdzah.html

TS:   同 JS
来源：http://hz.xylfe.cn/gtkbeczvbq.html

Java: 方法内为块级作用域
来源：http://hz.jqgfzy.top/gtdepibfbf.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtcpqvgihr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.kuanghao11.cn/gtvzgzuqey.html

C#:   块级作用域
来源：http://hz.havefunace.top/gtirxfsueu.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtxjrkrfkj.html

Py:   from module import func
来源：http://hz.kuanghao11.cn/gtrcvmyqtg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtagpxwpcs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gtklnbtxxz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj20258.top/gtwklznriq.html

Java: import java.util.List;
来源：http://hz.ybcxt.top/gtppjhenqm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cheryme.top/gtqmoqztam.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtopmeobpu.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gtebzszxjb.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtuzztprkk.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtbxidinwc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtmamjalhx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gtmdnayksn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtdltxjsxi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258888.top/gtixuaaidh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtlgklfpgx.html

Ruby: -> { puts "run" }.call
来源：http://hz.yanxiufei.cn/gtuktbzsfy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.c1oappe.top/gtnfkggtxh.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtxnacvkzc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuanzhike.top/gtnwtrszkm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtelwkguck.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shangyingyoupin.top/gtarvvngvd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtkhnmcvid.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtabqzurbu.html

Go:   func add(a, b int) int
来源：http://hz.mhx1999.top/gtbnlaytqz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dianchejie.cn/gtrxkqydvj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gthmwkogvw.html

[C14] 泛型函数
来源：http://hz.ywan-chungtsiang.top/gtcwbwfnfz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hongshengwenyu.top/gtxaohaiuu.html

PHP:  // 无泛型
来源：http://hz.wangshuangyany.cn/gtwfvxpkpm.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtqukqbiqd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtjmquymgi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigufen.top/gtnsnkruoy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.iojbl.cn/gtylahlhun.html

Ruby: # 无泛型
来源：http://hz.jinyuanbaomall.cn/gtlrmvukrr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtzsedciul.html

[C15] 解构 / 展开参数
来源：http://hz.zhijiandao.cn/gteywkpikv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jyoumei.cn/gtiaijcyak.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtybrtecdr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtvsigyukf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtizmyoxga.html

Java: // 无解构
来源：http://hz.haohaochexian.top/gtjtlxuksn.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtkvoadmru.html

Ruby: a, b = pair
来源：http://hz.yvedp.cn/gtotircksi.html

C#:   var (a, b) = pair;
来源：http://hz.yangfankeji.com/gtbccryayt.html

[C16] 函数 / 方法重载
来源：http://hz.316326.xyz/gttyhxlypa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtugtrlrxq.html

PHP:  // 无重载
来源：http://hz.hongshengwenyu.top/gtsfjeczcs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gttntfolwc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gtinuupoig.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.52xcode.cn/gtcnlulpgk.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtabjfzezl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gtkddymbdu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydjk.org.cn/gtrxolgocb.html

================================================================================
来源：http://hz.yuanzhike.top/gtfzfdkqyu.html

D. 数组 / 列表 / 集合
来源：http://hz.yueranfly.top/gttiwvtoey.html

================================================================================
来源：http://hz.yj202588.top/gtlkprrtsh.html

[D01] 创建数组 / 列表
来源：http://hz.wangshuangyany.cn/gtpsulvjgw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.vqdsnc.cn/gtsyeuhcqw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.mhx1999.top/gtpqhyenpc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtaqhxnbxr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nwbrower.top/gtfnybsftx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtsmmfgkcd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ybcxt.top/gtcnlosstm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtmveuqcry.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtsafiutnd.html

[D02] 追加元素到末尾
来源：http://hz.fzhhl.top/gtudbzkfyo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnxiangtu.top/gtpkzikpsv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtcfebwtyp.html

JS:   arr.push(4);
来源：http://hz.xuanzx.com/gtarukowfx.html

TS:   arr.push(4);
来源：http://hz.hammf.cn/gtqidmkgpv.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtrkyxdpyv.html

Go:   arr = append(arr, 4)
来源：http://hz.sufxvd.cn/gtjngpztyy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuxming.cn/gtksmohadx.html

C#:   list.Add(4);
来源：http://hz.cucudq.cn/gtjugbfksv.html

[D03] 在指定位置插入元素
来源：http://hz.gzhubu.top/gtjggmqaxk.html

Py:   arr.insert(0, 0)
来源：http://hz.tianlin.xyz/gtcgjepeqn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gtlhqvmfjz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtylnsmghp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtskiyvfnm.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtagsnmpxi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.haohaochexian.top/gtzlkgkyse.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj202588.top/gtccmglrzo.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtwzkiovah.html

[D04] 删除元素
来源：http://hz.jinyuanbaomall.cn/gtmuhkcktr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtabwtfitm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gttirmcogi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yanxiufei.cn/gtssthqzoo.html

TS:   arr.splice(0, 1);
来源：http://hz.wangshuangyany.cn/gtlqufkqjs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhongyouzk.top/gtqbrzrjly.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtsxdsoqhu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtctlxqhln.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sweek.top/gtjqyrxyah.html

[D05] 访问与修改元素
来源：http://hz.gaohongyu789.top/gtifrnspaz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gticodrqyp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtufbpuumk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtyyhfoogb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zycfv.cn/gtaacactmp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hysaishi.cn/gtafpimprn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtasolxsdq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtgfibhkma.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gtcabvwbcf.html

[D06] 数组长度
来源：http://hz.jqgufenzy.top/gtkqzfjrqd.html

Py:   len(arr)
来源：http://hz.yangfankeji.com/gtfsdnnhsp.html

PHP:  count($arr);
来源：http://hz.shangyingyoupin.top/gtsybuudox.html

JS:   arr.length
来源：http://hz.dianchejie.cn/gtwvgtjkvc.html

TS:   arr.length
来源：http://hz.ivvv.top/gtkzdfudgl.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtshiqwrau.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gtcouwpsmh.html

Ruby: arr.length; arr.size
来源：http://hz.haohaochexian.top/gtxgikoeih.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtlkxggfvm.html

[D07] 切片 / 取子数组
来源：http://hz.yanxiufei.cn/gtfomrojcz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.pengpengdd.cyou/gtufmsswtx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dashuyun.cn/gtfwxqvhox.html

JS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtgtpaluqe.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gthrqcrcll.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gtjgqjsnlk.html

Go:   arr[1:4]
来源：http://hz.yueranfly.top/gtdqcnjojc.html

Ruby: arr[1, 3]
来源：http://hz.ehwqpu.com/gtfyvygdyj.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinyuanbaomall.cn/gtspgfxcxx.html

[D08] 合并两个数组
来源：http://hz.fengsongda.top/gtdthwdiac.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gtwdhmfxmh.html

PHP:  array_merge($a, $b);
来源：http://hz.hysaishi.cn/gtdowcbksg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtanfzafdz.html

TS:   [...a, ...b];
来源：http://hz.wangdashe.top/gtpizyjcqm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtxuiicdya.html

Go:   append(a, b...)
来源：http://hz.ywan-chungtsiang.top/gtawrbppmn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxuanxn.top/gtiynrastr.html

C#:   a.Concat(b).ToList()
来源：http://hz.jlsjyb.cn/gtrtrbbfmc.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtywstacuz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtvvvvqsmr.html

PHP:  sort($arr);
来源：http://hz.hongshengwenyu.top/gtitqkgjob.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtcnhmyozd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtdqwvclst.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xingfuxueyuan.xyz/gtknlgxwgb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258888.top/gtrkzgeqft.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gthhskasgm.html

C#:   list.Sort();
来源：http://hz.zhengqikj.top/gtldmjuqea.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hnxiangtu.top/gtmpkiylje.html


<!-- 参考信息 -->