代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtavpzmwit.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shuidangran.top/gtfoqawlwk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ydzc1.top/gtxfwllxgv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtqtiuhcwf.html

[B09] break 与 continue
来源：http://hz.iojbl.cn/gtfhfreiob.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gtkzmydaud.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.pycfn.com/gtmgyxflyh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtewvefohu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtubexdkmf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtutcfitky.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhengqikj.top/gtpygztpki.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtcoxjhraz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtxnmerziv.html

[B10] 遍历同时拿索引
来源：http://hz.daxiang520.top/gtkacxbnux.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cqqwz.cn/gtepsegocv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.wangshuangyany.cn/gtoaukrbal.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtmfledokq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtrhlmowee.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gtfyxullwh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigufen.top/gtpnimlbji.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cheryme.top/gtzuvdikyp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigufen.top/gtjpscdyfy.html

[B11] 生成数字序列 / 区间
来源：http://hz.feifeiyinyue.top/gtavmahfnz.html

Py:   list(range(0, 10, 2))
来源：http://hz.yuanzhike.top/gtfeesxmtb.html

PHP:  range(0, 10, 2);
来源：http://hz.xuanzx.com/gteqdkbrys.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtimdmsakt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtpjxibybr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ehwqpu.com/gtoqoozqje.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.feifeiyinyue.top/gtjldpoqgr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dashuyun.cn/gteybxaejd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tanke756.top/gtiobwrgdt.html

[B12] 跳出多层循环
来源：http://hz.yongpay.top/gtauwowfii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.iojbl.cn/gtmbezzpcb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jlsjyb.cn/gtisrqycfy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gttkroitrv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtkvwscayd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtcookoisb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cqqwz.cn/gtcherigcv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ivvv.top/gthfojpaff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gaohongyu789.top/gtsygqzevt.html

[B13] 判断是否为数字
来源：http://hz.andypj.xyz/gtciebubbx.html

Py:   isinstance(x, (int, float))
来源：http://hz.daxiang520.top/gtasagsdvd.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtcjrujnxv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenzaomai.com/gtgpkutfpk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtoojajrds.html

Java: x instanceof Number
来源：http://hz.guannengcc.top/gtrqfpytuk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zycfv.cn/gtisgbnttl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtpihkiacy.html

C#:   x is int or double or decimal
来源：http://hz.jinqigufen.top/gtvmrglxbq.html

[B14] 判断值是否在集合内
来源：http://hz.ppjwa.cn/gtuplsmfzk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guannengcc.top/gtwugwnwek.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhiwuduotai.top/gtqvwayqxu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj202588.top/gtvfuvhnfr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtehmpsvde.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yonumen.top/gtubqscruj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.haohaochexian.top/gtwvnchluz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ybcxt.top/gtfseqqjoc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtvpiunvbq.html

[B15] 布尔运算与取反
来源：http://hz.jlsjyb.cn/gtfpwwmkvo.html

Py:   a and b or not c
来源：http://hz.zhixingplan.top/gtodcrsclh.html

PHP:  $a && $b || !$c
来源：http://hz.yueranfly.top/gtoozjxtkg.html

JS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtrzfhvgsb.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gtdjeajrvo.html

Java: a && b || !c
来源：http://hz.nanxuanxn.top/gtbbkaojhf.html

Go:   a && b || !c
来源：http://hz.kuanghao11.cn/gttmdzcsfl.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gtupjlyhte.html

C#:   a && b || !c
来源：http://hz.andypj.xyz/gtguisycfe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtdlwrodvh.html

Py:   if not data: return
来源：http://hz.pengpengdd.cyou/gtpvkhdlmq.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gteoncbjkx.html

JS:   if (!data) return;
来源：http://hz.fengsongda.top/gtlheupbyb.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtbufuopeq.html

Java: if (data == null) return;
来源：http://hz.gogol.net.cn/gtuytfzzak.html

Go:   if data == nil { return }
来源：http://hz.ehwqpu.com/gtxygliurp.html

Ruby: return if data.nil?
来源：http://hz.yueranfly.top/gtzwmirdyp.html

C#:   if (data == null) return;
来源：http://hz.jqgfzy.top/gtzebjqvbh.html

================================================================================
来源：http://hz.xziqi.cn/gtxqdzgaqm.html

C. 函数与作用域
来源：http://hz.shangyingyoupin.top/gtrzofaeis.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwkxpldcr.html

[C01] 定义函数
来源：http://hz.wangshuangyany.cn/gtjtmmvnqu.html

Py:   def add(a, b): return a + b
来源：http://hz.shuidangran.top/gtdwdvjmip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtjtqkahsj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hammf.cn/gtgkzrmild.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtvvlkkkwk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gteyrmllwl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sweek.top/gthdlhaeaq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shangyingyoupin.top/gtcxycxdge.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtoaxftlxf.html

[C02] 默认参数
来源：http://hz.shanyushiyangkeji.top/gtpzxqugzl.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtueththvz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.smart0.xyz/gtcyrxaxsr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dianchejie.cn/gtynsqyajf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cucudq.cn/gtqebzhtmd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtgtomozbk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cdnleiting.top/gtsevoulqx.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtzkzrxkeg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pycfn.com/gtsnrpbtyi.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gtouzvaequ.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj202588.top/gtsmpcjzdm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yonumen.top/gtmziqkeme.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtqpbnkyoa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtwzwwvvsw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.svipenyu.cn/gtrhdrnihk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenzaomai.com/gtogqkkgke.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gogol.net.cn/gtdqwmmuaj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhixingplan.top/gtnipezdbv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtzdqehrmt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gtwaqdxfoj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gtlawwwtpr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtebedwxgr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daria6918.cn/gtawoaxlxn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtepujauyy.html

Go:   // 无：用配置结构体参数
来源：http://hz.xziqi.cn/gtqfcxzajq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gttrrobyzw.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtntjlhdah.html

[C05] 返回多个值
来源：http://hz.ppjwa.cn/gthfzkovhq.html

Py:   return a, b
来源：http://hz.jinqigfzy.top/gtgaihohhk.html

PHP:  return [$a, $b];
来源：http://hz.iojbl.cn/gtilaoveud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtewgfhcwd.html

TS:   return { a, b };
来源：http://hz.shuidangran.top/gtytprwrqs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gogol.net.cn/gtzzsuahjc.html

Go:   return a, b
来源：http://hz.hammf.cn/gtbdbwnfpa.html

Ruby: return a, b
来源：http://hz.jianghu66.top/gtvafsycgu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhixingplan.top/gtrvmpoumv.html

[C06] 匿名函数 / lambda
来源：http://hz.kuanghao11.cn/gtznmcxwao.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtprrjiciy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxinkj.top/gtzsyarqja.html

JS:   const square = x => x * x;
来源：http://hz.fzhhl.top/gtxjkslyso.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtkxjtuebk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenlongwang.top/gtbyzmfnig.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnxiangtu.top/gttxrpxbcz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ywan-chungtsiang.top/gtasnukgam.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtbadabxla.html

[C07] 把函数作为参数传入
来源：http://hz.dianchejie.cn/gtclsftzbc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gogol.net.cn/gtkleefmkn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.vqdsnc.cn/gtpfxczsyt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gtrjgofulu.html

TS:   arr.map(String)
来源：http://hz.hammf.cn/gtwryfrksw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgfzy.top/gtndczunpz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ywan-chungtsiang.top/gtlhtymoxq.html

Ruby: arr.map(&:upcase)
来源：http://hz.smart0.xyz/gtbcslrpja.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sysykeji.top/gtlgxackxu.html

[C08] 闭包
来源：http://hz.fengsongda.top/gtaqzcrpyt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sufxvd.cn/gtebunaikw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.316326.xyz/gtgzhlsyzt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtshfpdqlq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtzppljzdu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gttfldfmii.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgfzy.top/gthfrcmoae.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gtncswjkjl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gteskxfvem.html

[C09] 递归
来源：http://hz.aizwys.cn/gttpjhquvy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj202588.top/gtkaiflmdl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhoulong.xyz/gtpdnshfgl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtkwvrnfem.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtnriazdkj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigufen.top/gtnujetcqt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtwdakwhwu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gtygnuaqqn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.vqdsnc.cn/gtaqkvtwyn.html

[C10] 变量作用域
来源：http://hz.yonumen.top/gtibljunuu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtaixerkaj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinghuilouyu.cn/gthmtrzxbs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yangfankeji.com/gtwjkjudov.html

TS:   同 JS
来源：http://hz.xingfuxueyuan.xyz/gtojglovtj.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtouhzqtwi.html

Go:   花括号块级作用域
来源：http://hz.zhiwuduotai.top/gtktftjjzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.birdmap.top/gteutkwqka.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtqeoxmctj.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gthujqidqg.html

Py:   from module import func
来源：http://hz.sweek.top/gthuosamjx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuanzx.com/gtlrakutbc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhongyouzk.top/gtgfmoupdj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtwkmfrwlj.html

Java: import java.util.List;
来源：http://hz.jinqigufen.top/gtjctgcqkl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gtooxmahlm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtqombbhzw.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtsjjlyagn.html

[C12] 立即执行函数 IIFE
来源：http://hz.fzhhl.top/gtjbfbgqze.html

Py:   (lambda: print("run"))()
来源：http://hz.yongpay.top/gtzuburrhk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zdqjudy.top/gtwsgydtml.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtrcspuncx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtfpjipggl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gtlmmgqiey.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gttcyxccfu.html

Ruby: -> { puts "run" }.call
来源：http://hz.shuidangran.top/gtookyglxk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtofmlugym.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhongyouzk.top/gtarmxumdp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtvifrfmll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtktsfqefb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigfzy.top/gtvajveilj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtoqexjhem.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtpcbpfjwb.html

Go:   func add(a, b int) int
来源：http://hz.cheryme.top/gtdrswavij.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtouswexbl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gteblrxlpr.html

[C14] 泛型函数
来源：http://hz.jinqigufen.top/gthohiaknf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.meibo888.top/gtyydtspkk.html

PHP:  // 无泛型
来源：http://hz.zhijiandao.cn/gtrmbdfjbn.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtxuqjaior.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gtaagttofl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dianchejie.cn/gtehkrqgvx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtrahzghzk.html

Ruby: # 无泛型
来源：http://hz.yueranfly.top/gtumqdyquk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.9152youxi.cn/gtnfntzrhm.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtymkyyngw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtweqtojmj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gtjjighneu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtvuslqkkj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.feifeiyinyue.top/gtemsvbcfe.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtoiztbvaz.html

Go:   // 无解构
来源：http://hz.pengpengdd.cyou/gtkcjzozxv.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtqwoonhig.html

C#:   var (a, b) = pair;
来源：http://hz.gogol.net.cn/gtewlbzqha.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtmfgpdfvy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigfzy.top/gtrmkwhhrl.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gtihygamfw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xingfuxueyuan.xyz/gtmkqkpudk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhaomingkeji.xyz/gtdenpkgup.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtelrwlcox.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gtysnhbssc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtmvoiqxit.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.dianchejie.cn/gtwailbrzz.html

================================================================================
来源：http://hz.tian-w.cn/gtntmkzryw.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gthngzvnsx.html

================================================================================
来源：http://hz.tianlin.xyz/gtfrvpfbpx.html

[D01] 创建数组 / 列表
来源：http://hz.xylfe.cn/gthttllgaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtcoknokqd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gaohongyu789.top/gtbtdzjnfp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtduderwmm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtaizmbjao.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zycfv.cn/gtnbfbbfpo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtsfozujvs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.quarkkingdee.top/gtldhrcdvj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtcttjixey.html

[D02] 追加元素到末尾
来源：http://hz.ydjk.org.cn/gtjuxswgwy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigfzy.top/gtbqkbguea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ywan-chungtsiang.top/gtriyphmnq.html

JS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtbkkwrofq.html

TS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtzogweygt.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gthmvukxls.html

Go:   arr = append(arr, 4)
来源：http://hz.gotoacloud.top/gtkswwinlg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtzzymjiia.html

C#:   list.Add(4);
来源：http://hz.gzhubu.top/gtyowjaklq.html

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtiiqmmjej.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gtjxesdfdd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigfzy.top/gtozzqwiwl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guowangkeji.top/gtcennjcfd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuanzx.com/gtgzusaonj.html

Java: list.add(0, 0);
来源：http://hz.ppjwa.cn/gtzetszxww.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jlsjyb.cn/gtjloyisqt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtsmdwwdxr.html

C#:   list.Insert(0, 0);
来源：http://hz.jianghu66.top/gtiawajdre.html

[D04] 删除元素
来源：http://hz.vqdsnc.cn/gtqfxwrzrj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.quarkkingdee.top/gtfbzjvdgv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gaohongyu789.top/gtmpblsyjy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhengqikj.top/gttowcwkej.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtbkexsbim.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtdaalfolf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gogol.net.cn/gtlmleqprz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtxtlwtfhd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigufen.top/gthkvtaosj.html

[D05] 访问与修改元素
来源：http://hz.aizwys.cn/gtkrvzsuqg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtalwyrbzl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hywenlv.cn/gtyzpnbzmk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtppxeadvy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hongshengwenyu.top/gtgzikxfxu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtiuzncvfh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtxacvveda.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gttrvfidnv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtrdhsusqa.html

[D06] 数组长度
来源：http://hz.hammf.cn/gtncqkmlwg.html

Py:   len(arr)
来源：http://hz.hywenlv.cn/gtfvixuyby.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtfpndbpad.html

JS:   arr.length
来源：http://hz.nanxinkj.top/gteghqwlmz.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gthbolcubs.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtlxvqvryd.html

Go:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtjiofdgnm.html

Ruby: arr.length; arr.size
来源：http://hz.0kj1m.cn/gtfbrnrkji.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtibojgsrr.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtuyhorchr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daria6918.cn/gtrmomwffc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydjk.org.cn/gtmkrdqgea.html

JS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtbzncsrkn.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gttaztobhw.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtsqoxbtso.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gtrmyzvzdd.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gtvfswopwv.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtwevayxhr.html

[D08] 合并两个数组
来源：http://hz.smart0.xyz/gtxijwlmdi.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gtrexgjskg.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxuanxn.top/gtcxjfshhx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hfpthk.cn/gtaoewlsvq.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtfgkzmvmy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nwbrower.top/gtlvkfzsky.html

Go:   append(a, b...)
来源：http://hz.jlsjyb.cn/gttvfdppvo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jiagoushi.top/gtqfdiainu.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtujrlwtcg.html

[D09] 排序（升序）
来源：http://hz.ydzc1.top/gtxgziwxbp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtrmlgdiyk.html


<!-- 参考信息 -->