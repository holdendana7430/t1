代发 wailian999

[B09] break 与 continue
来源：http://hz.ydzc1.top/gtbwazhmxh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nanxinkj.top/gtdkyzjkom.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cheryme.top/gtxphfvusx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtowkdrpmp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtagvytjml.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtbugjsovs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.fengsongda.top/gtlpaspwnk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ybcxt.top/gtpdekniyk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtpqwlhkjs.html

[B10] 遍历同时拿索引
来源：http://hz.jianghu66.top/gtqofvvsxh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.andypj.xyz/gtboliuahd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gaohongyu789.top/gtyixfxftn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gzhubu.top/gtoaofbrlj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zycfv.cn/gtfsujfecv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.snrcjt.cn/gtyvkpqkyy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj202588.top/gtoffyrbvb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jianghu66.top/gtfgqbjfja.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.feifeiyinyue.top/gtsmlgcnpc.html

[B11] 生成数字序列 / 区间
来源：http://hz.yueranfly.top/gtyaykzvfv.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhoulong.xyz/gtrmusnvsh.html

PHP:  range(0, 10, 2);
来源：http://hz.tian-w.cn/gtgxdjexns.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtjclryolk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtcaomxbrf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yanxiufei.cn/gtrkbsatwd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zycfv.cn/gthzizdscu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenjidiqi.icu/gtkjppvohl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.havefunace.top/gtfpdzeapp.html

[B12] 跳出多层循环
来源：http://hz.pengpengdd.cyou/gtewktheae.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.redwolf501.top/gtkdpuhags.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hywenlv.cn/gtrvhrcasu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtvfbiblhs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtljgilkkh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtkblunvxi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.0kj1m.cn/gtlbnraglo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shzxlz.cn/gtvicwbaah.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dashuyun.cn/gttlbiysfz.html

[B13] 判断是否为数字
来源：http://hz.wangdashe.top/gtikgjakyt.html

Py:   isinstance(x, (int, float))
来源：http://hz.0kj1m.cn/gtaaqkaqeb.html

PHP:  is_numeric($x)
来源：http://hz.shanyushiyangkeji.top/gtshjndhty.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gtxwycpggu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtwtgfpxeo.html

Java: x instanceof Number
来源：http://hz.gogol.net.cn/gtjqmzjwcx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhengqikj.top/gtghuietyv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxinkj.top/gtwjfulkcl.html

C#:   x is int or double or decimal
来源：http://hz.cqqwz.cn/gthycwgffq.html

[B14] 判断值是否在集合内
来源：http://hz.sufxvd.cn/gtyvqnfwph.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnxiangtu.top/gtcjzymxok.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cheryme.top/gtgmxfursh.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtpjjairqc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtcdlzylmr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.daria6918.cn/gtmxdgkcda.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhijiandao.cn/gtdimauinq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinqigfzy.top/gtarqzukex.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jlsjyb.cn/gtpijpsgqt.html

[B15] 布尔运算与取反
来源：http://hz.0kj1m.cn/gtedyfmfmt.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtlyehyikr.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gtbvrtnnjm.html

JS:   a && b || !c
来源：http://hz.guannengcc.top/gtkppbcmcz.html

TS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtmeqjwpab.html

Java: a && b || !c
来源：http://hz.wangdashe.top/gtrflnkbpe.html

Go:   a && b || !c
来源：http://hz.ppjwa.cn/gtcskyvplo.html

Ruby: a && b || !c
来源：http://hz.ydjk.org.cn/gtjtfitmug.html

C#:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtvtgxoapv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gtqcqfxwob.html

Py:   if not data: return
来源：http://hz.bjfxy.top/gtptmudetc.html

PHP:  if (!$data) { return; }
来源：http://hz.andypj.xyz/gtprymxvkb.html

JS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtxszuzsea.html

TS:   if (!data) return;
来源：http://hz.quarkkingdee.top/gtpfispcwv.html

Java: if (data == null) return;
来源：http://hz.52xcode.cn/gtppdzcugo.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtcdxwvsex.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtxneqalrd.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gthwusnzdu.html

================================================================================
来源：http://hz.guannengcc.top/gtobihfiyc.html

C. 函数与作用域
来源：http://hz.redwolf501.top/gtbxlmzoyf.html

================================================================================
来源：http://hz.fengsongda.top/gtwvfsrjlj.html

[C01] 定义函数
来源：http://hz.zhiwuduotai.top/gttqapluim.html

Py:   def add(a, b): return a + b
来源：http://hz.kuanghao11.cn/gtbzmmuxuw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gthumovzuq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigufen.top/gtypyekhaf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.quarkkingdee.top/gtitexdham.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtmlcgehxb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cashguo.top/gthkyymtnm.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hongshengwenyu.top/gtogzfwasc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtrcoybqyy.html

[C02] 默认参数
来源：http://hz.meibo888.top/gtsofkjbsl.html

Py:   def greet(name="World"): return name
来源：http://hz.meibo888.top/gtfswmopii.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgufenzy.top/gtairyhyjq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtwdzorusn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jyoumei.cn/gtqrezyzeb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gtgowwfbgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangtech.top/gtoavqnacq.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtuhedflfq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gtlwicxbnz.html

[C03] 可变参数
来源：http://hz.xuanzx.com/gtykzbiqcm.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtnafhfnkk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnqzz.top/gtmaxdraob.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gthwsfropt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtevdviggy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sysykeji.top/gtuumqtqpu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.haohaochexian.top/gtknznkwsy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gtrnyolxwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtgaibfbbx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtxdwqfbwz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.bjfxy.top/gtqohsxaeo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gtpbipocfj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fzhhl.top/gtnukdwyke.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.feifeiyinyue.top/gtppsrucrm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnxiangtu.top/gtiysjbqic.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtekpbfchc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtixulrabv.html

C#:   f(a: 1, b: 2)
来源：http://hz.guowangkeji.top/gtsyceoozt.html

[C05] 返回多个值
来源：http://hz.c1oappe.top/gtvliuvwep.html

Py:   return a, b
来源：http://hz.9152youxi.cn/gtfoqfrohh.html

PHP:  return [$a, $b];
来源：http://hz.ydzc1.top/gthwytpwss.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yongpay.top/gtrpptsxjd.html

TS:   return { a, b };
来源：http://hz.aibaodan.cn/gtrlzblpwv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhengqikj.top/gtmrboxjyi.html

Go:   return a, b
来源：http://hz.hammf.cn/gtjmqexnyl.html

Ruby: return a, b
来源：http://hz.wangshuangyany.cn/gtjyxzkyqi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zycfv.cn/gtyeucdcny.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtxjgsjemu.html

Py:   square = lambda x: x * x
来源：http://hz.kuanghao11.cn/gtqjnmzouq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.fzhhl.top/gtiqurknot.html

JS:   const square = x => x * x;
来源：http://hz.zhiwuduotai.top/gtwkdulyjd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhixingplan.top/gtnkbcdxrm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.c1oappe.top/gtisieqghn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cheryme.top/gtudedcnlc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gtfvtjuegw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pycfn.com/gtnfporpqg.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtwfdpepkw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ybcxt.top/gtmrveudlg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gtidznqmtp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ppjwa.cn/gtabmfcbpk.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtuswdswul.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daxiang520.top/gtoiyokdjj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gttwjotqnc.html

Ruby: arr.map(&:upcase)
来源：http://hz.yuanzhike.top/gtckkkaswj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtircmnsos.html

[C08] 闭包
来源：http://hz.jinqigfzy.top/gtyucauxqg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtvybxiseo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtqvpdctnk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtragmcokq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtxkestsrj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtqgpnovyp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.svipenyu.cn/gtgkqgkhva.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuxming.cn/gtpaignohq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtvvlvfomx.html

[C09] 递归
来源：http://hz.guowangkeji.top/gtdmghnric.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cashguo.top/gttxmtrybe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.snrcjt.cn/gtfiklnhnx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gteupmbohs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtjpfmaezj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtemnlcyjg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtodvnbrjo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jianghu66.top/gtluxkxfot.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gtflngizds.html

[C10] 变量作用域
来源：http://hz.52xcode.cn/gtpfgiccbx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pycfn.com/gtslhcntco.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hfpthk.cn/gtexpqmiwj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ybcxt.top/gtvsyvvdwo.html

TS:   同 JS
来源：http://hz.cashguo.top/gtuflbffoj.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtzfrzryee.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtahvsqbok.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtffvekxam.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtjzihnmdm.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtittkzhht.html

Py:   from module import func
来源：http://hz.gzhubu.top/gtkzwefykh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtgjdijyqo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shuidangran.top/gtcnzwdpme.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtxfxbkxdz.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gthrhpijhs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinyuanbaomall.cn/gtbwuajmyu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydjk.org.cn/gtxmhqpasj.html

C#:   using System.Text;
来源：http://hz.hfpthk.cn/gtcwfiaksa.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gtlegyrkoz.html

Py:   (lambda: print("run"))()
来源：http://hz.svipenyu.cn/gtivfouswd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guowangkeji.top/gtkxugexze.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtksuwwuee.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtlpzsmsvm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hammf.cn/gtpnslhgzx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.wangdashe.top/gtpkrevyfr.html

Ruby: -> { puts "run" }.call
来源：http://hz.zycfv.cn/gtntcbxvul.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hywenlv.cn/gtgrruxdpd.html

[C13] 类型声明 / 类型注解
来源：http://hz.hywenlv.cn/gtimhlczpq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.meibo888.top/gtnuwymyrt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtiugszjan.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnqzz.top/gtjsnaskxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtnnlnxijh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtzvkvxlac.html

Go:   func add(a, b int) int
来源：http://hz.yuanzhike.top/gtpehgzsci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtxxtdhnut.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shzxlz.cn/gthwwbwrms.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtqzmjhhyx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtqqtjsbho.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtmcrkdfpb.html

JS:   // 无泛型
来源：http://hz.zdqjudy.top/gtgbrttrvc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gttguqbaft.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtxyhovuua.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhaomingkeji.xyz/gtgdtreoww.html

Ruby: # 无泛型
来源：http://hz.svipenyu.cn/gtntxyeard.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtahkbhptw.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtvbktzmxp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtmdqjgfdg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gtphjjjilf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gzhubu.top/gtdhucwugu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yvedp.cn/gtrmwukyle.html

Java: // 无解构
来源：http://hz.shzxlz.cn/gtnuefesuw.html

Go:   // 无解构
来源：http://hz.cdnleiting.top/gtjqlganqa.html

Ruby: a, b = pair
来源：http://hz.svipenyu.cn/gtkrsqhfjn.html

C#:   var (a, b) = pair;
来源：http://hz.yangfankeji.com/gtilspxunl.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtglmgbwlc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gteuhqxwsz.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtmzypmwhl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhongyouzk.top/gtvnazcrid.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhiwuduotai.top/gtpqyeujxz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258888.top/gtpawcmwkm.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gtxtllslre.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hywenlv.cn/gtfamiydew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtbiwqcgtd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdeypzguo.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtdubliaaw.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdmehcynz.html

[D01] 创建数组 / 列表
来源：http://hz.feifeiyinyue.top/gtdievqfwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangdashe.top/gtuszsgneo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhiwuduotai.top/gtdrfwbrqy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtcqzettbv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenlongwang.top/gtcfxqfbjl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.iojbl.cn/gtetmvkovz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.9152youxi.cn/gtztuqmuth.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jlsjyb.cn/gtbskseqjc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtnhkrdzcg.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtmxeqjmvt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yvedp.cn/gthkucnvuv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pengpengdd.cyou/gtqqpntxdi.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtjplofvzp.html

TS:   arr.push(4);
来源：http://hz.fengsongda.top/gtzkozqpdv.html

Java: list.add(4);
来源：http://hz.sweek.top/gtvbeosjxo.html

Go:   arr = append(arr, 4)
来源：http://hz.sysykeji.top/gtuwojqfsn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhoulong.xyz/gtlfkrijfp.html

C#:   list.Add(4);
来源：http://hz.jinyuanbaomall.cn/gtxfmwvplp.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gtreydqaqo.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtnvnlggmo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tanke756.top/gtjhgiwznb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.smart0.xyz/gtrihmwged.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtvfuokuvn.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gtzenwiykb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtwcclsjct.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guowangkeji.top/gtbeqvvuvz.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtkloypbrw.html

[D04] 删除元素
来源：http://hz.hammf.cn/gtmdaprgly.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fzhhl.top/gtrmdbqlfv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtfffzmjhz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yongpay.top/gttnvvpntx.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gtpsmpsfal.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuanzhike.top/gtdsoiegee.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xziqi.cn/gtivmqbkrk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hongshengwenyu.top/gtztiyisun.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtcaohadrl.html

[D05] 访问与修改元素
来源：http://hz.yuxming.cn/gttlczftht.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtniilcpub.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xziqi.cn/gttlmmrhip.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtuooitxvu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yonumen.top/gteenfjodl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtxexeceyi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gttvnfzskf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtiompvpms.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cucudq.cn/gtiltzzlwk.html

[D06] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtsqkocuxz.html

Py:   len(arr)
来源：http://hz.jinqigufen.top/gtjufuamdq.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtqgpuowlk.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtccvjxepj.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtrlfmrvni.html

Java: list.size();
来源：http://hz.iojbl.cn/gtuhqhqvfm.html

Go:   len(arr)
来源：http://hz.gotoacloud.top/gtglmligjr.html

Ruby: arr.length; arr.size
来源：http://hz.cucudq.cn/gtothajdnr.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtdbsnoaem.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gtogwlqqdi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.kuanghao11.cn/gtdyhuumdb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinyuanbaomall.cn/gtvyoxeitm.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gthzccbgmj.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtjowlhivi.html

Java: list.subList(1, 4);
来源：http://hz.ybcxt.top/gtysjdthhd.html

Go:   arr[1:4]
来源：http://hz.pycfn.com/gtzymfyduo.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtrhrumgdk.html

C#:   list.GetRange(1, 3);
来源：http://hz.gzhubu.top/gtxgyzjdyd.html

[D08] 合并两个数组
来源：http://hz.pycfn.com/gtrrbkuayt.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gtzkldmlfp.html

PHP:  array_merge($a, $b);
来源：http://hz.gzhubu.top/gtpzfepyua.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hysaishi.cn/gtvpmqchby.html

TS:   [...a, ...b];
来源：http://hz.jinyuanbaomall.cn/gtfllbjboq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtzmwettyh.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtstgmkoqe.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sxryk.cn/gttlgxbugy.html

C#:   a.Concat(b).ToList()
来源：http://hz.kuanghao11.cn/gtfxvjbnlg.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtqbmhhigo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtkfqnwpmk.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtxuztnfub.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.316326.xyz/gthkbwqnrp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gtzoduzdgv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fzhhl.top/gtrqyplbfc.html


<!-- 参考信息 -->