代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtwbyquase.html

[B10] 遍历同时拿索引
来源：http://hz.tianlin.xyz/gtiexbxgyu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ydzc1.top/gtrgwihrgl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nwbrower.top/gthoeklyqj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtvprznohf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xziqi.cn/gtgbvocxxp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fzhhl.top/gtvoxjkkig.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhiwuduotai.top/gtsjzwyffv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgfzy.top/gtthzzxzyn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhaomingkeji.xyz/gtyohmzrgc.html

[B11] 生成数字序列 / 区间
来源：http://hz.cqqwz.cn/gtmvrukopv.html

Py:   list(range(0, 10, 2))
来源：http://hz.xinyue.icu/gtpbrrvfme.html

PHP:  range(0, 10, 2);
来源：http://hz.sxryk.cn/gtmglfwwhc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtbznczoda.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.andypj.xyz/gtlyxfbafm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinghuilouyu.cn/gtqjwsguyw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sweek.top/gtdfhchmij.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtibupboyf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gtygvavosf.html

[B12] 跳出多层循环
来源：http://hz.gogol.net.cn/gtekigyjwz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgfzy.top/gtkkrchdrj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.c1oappe.top/gtnfgfniti.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtzibdlljf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtrnqwseje.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtqkarhfde.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydzc1.top/gtvncsegto.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxuanxn.top/gtlqfofins.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.haohaochexian.top/gtgxuljfaz.html

[B13] 判断是否为数字
来源：http://hz.cdnleiting.top/gtradaqetx.html

Py:   isinstance(x, (int, float))
来源：http://hz.xylfe.cn/gtpuamziiz.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gtkvaocpxl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtzhlsvxki.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtdzltxznf.html

Java: x instanceof Number
来源：http://hz.xinyue.icu/gtqdtubtep.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gotoacloud.top/gtiahrwkxw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinghuilouyu.cn/gtywzcqwwo.html

C#:   x is int or double or decimal
来源：http://hz.kuanghao11.cn/gtlozjrsmx.html

[B14] 判断值是否在集合内
来源：http://hz.zycfv.cn/gtrwzfulgh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shangyingyoupin.top/gtlqbydzag.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gttthsufvm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtzdqgaudx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gttfnfwxrz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.havefunace.top/gtlywmdnor.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.vqdsnc.cn/gtilcrxycu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.c1oappe.top/gtzndcaahw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.haohaochexian.top/gtbjufrmjx.html

[B15] 布尔运算与取反
来源：http://hz.ydjk.org.cn/gtxrbssgnc.html

Py:   a and b or not c
来源：http://hz.xylfe.cn/gtuqysfgwf.html

PHP:  $a && $b || !$c
来源：http://hz.jinghuilouyu.cn/gtdspxhzzq.html

JS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtrazivkxx.html

TS:   a && b || !c
来源：http://hz.chenzaomai.com/gtvvxgkhrx.html

Java: a && b || !c
来源：http://hz.jyoumei.cn/gtxzwqrvyp.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gtgpmghwnj.html

Ruby: a && b || !c
来源：http://hz.vqdsnc.cn/gttztutzlc.html

C#:   a && b || !c
来源：http://hz.jianghu66.top/gtxqeyzcgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nanxinkj.top/gtqsulddaj.html

Py:   if not data: return
来源：http://hz.zhijiandao.cn/gtnjktlfxs.html

PHP:  if (!$data) { return; }
来源：http://hz.hysaishi.cn/gtvzoaqkiu.html

JS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtapwibhcv.html

TS:   if (!data) return;
来源：http://hz.zhijiandao.cn/gtotumzfyb.html

Java: if (data == null) return;
来源：http://hz.yuxming.cn/gtvsxydeoz.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gtgqirciix.html

Ruby: return if data.nil?
来源：http://hz.zhengqikj.top/gtbvtsaxgs.html

C#:   if (data == null) return;
来源：http://hz.sysykeji.top/gtfvrrkbwp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwrjmiimr.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gtqmlkgitq.html

================================================================================
来源：http://hz.hnqzz.top/gtmdehdylz.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtdwxkxenc.html

Py:   def add(a, b): return a + b
来源：http://hz.wangdashe.top/gtvmdfzdcq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtfdcqoljw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtfldwzres.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtyptxyomd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtunbwmxnh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.0kj1m.cn/gtbpqmmsoh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hywenlv.cn/gtcdfgxajh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtnpftlwpc.html

[C02] 默认参数
来源：http://hz.jiagoushi.top/gtneqgwxse.html

Py:   def greet(name="World"): return name
来源：http://hz.ppjwa.cn/gtqcmavasz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhengqikj.top/gtimqrujyq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gtcopalngb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nwbrower.top/gtxodceybu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.quarkkingdee.top/gtntdbzfga.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hysaishi.cn/gthlyooogh.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydzc1.top/gtahkpcijz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinghuilouyu.cn/gtuvmsxokz.html

[C03] 可变参数
来源：http://hz.zdqjudy.top/gtsgijtudr.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenlongwang.top/gthtcxhcch.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shangyingyoupin.top/gtflmduwac.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtazietshr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtbffrfqsk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtgyzhlmmt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gthnvxciwr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258.top/gtmnrfvfft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtwobpkdpd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shangyingyoupin.top/gtrqqmjhjh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.birdmap.top/gtgbnokfiy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.svipenyu.cn/gtlntldvup.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtymkorurs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtnptlhkqp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gtrneqxlsd.html

Go:   // 无：用配置结构体参数
来源：http://hz.yueranfly.top/gtrnturjji.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtdkpwnvwe.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtsjcneqwg.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtgpfjjtep.html

Py:   return a, b
来源：http://hz.pycfn.com/gtekabbmmk.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtpficjllj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sufxvd.cn/gtksjxwjap.html

TS:   return { a, b };
来源：http://hz.shangyingyoupin.top/gtlqdzmhww.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cdnleiting.top/gtsmluiodc.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtkcgsyoaz.html

Ruby: return a, b
来源：http://hz.yvedp.cn/gtitleoiqy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.quarkkingdee.top/gtrbbfxvnm.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtouyirobc.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtvdydjpsd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhiwuduotai.top/gtrmjlknpb.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtwilpineg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dashuyun.cn/gtzfmexmjx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dianchejie.cn/gtnqjvekew.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gtapoovxae.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhaomingkeji.xyz/gtzosbvazv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cdnleiting.top/gtumoxhbjr.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gthrnugjjz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xziqi.cn/gtshnizkoz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cdnleiting.top/gtkzqfelup.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhiwuduotai.top/gtsakrxnpe.html

TS:   arr.map(String)
来源：http://hz.shangyingyoupin.top/gtegaewtnq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gzhubu.top/gtezumljzu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cqqwz.cn/gtkueksqaq.html

Ruby: arr.map(&:upcase)
来源：http://hz.gzhubu.top/gtwzknnpmu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgfzy.top/gtqyfxnspi.html

[C08] 闭包
来源：http://hz.birdmap.top/gtofsyrfhh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtnrzbicdv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fzhhl.top/gtmfmoniua.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtbdcygmtl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtwktpdizq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhiwuduotai.top/gtlmhlntpq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydjk.org.cn/gtyrsgijcm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxuanxn.top/gtvvnvvcpf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtzyypkmpw.html

[C09] 递归
来源：http://hz.shangyingyoupin.top/gtvdjmhccp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtztyjacqx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zycfv.cn/gtsjngjgle.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtrkvedodh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtdzjtegiy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.svipenyu.cn/gtubjykaed.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.kuanghao11.cn/gturehmyeo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ivvv.top/gtgekivnac.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aibaodan.cn/gtytqumrwc.html

[C10] 变量作用域
来源：http://hz.cdnleiting.top/gttzvpawzn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangkeji.top/gtocolpnrq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hfpthk.cn/gtduszhnbu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtcdsphpiz.html

TS:   同 JS
来源：http://hz.nwbrower.top/gtfgzujsqq.html

Java: 方法内为块级作用域
来源：http://hz.hnqzz.top/gthaehnmma.html

Go:   花括号块级作用域
来源：http://hz.redwolf501.top/gtxiqcsydb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtlcdkqkwy.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtycpswqff.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gthhmzfbxq.html

Py:   from module import func
来源：http://hz.daria6918.cn/gtxouzhraw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtjwwdaaaf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xinyue.icu/gtdxygxhuj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gtwdvwllvc.html

Java: import java.util.List;
来源：http://hz.xuetiantiany.cn/gtqlztxgqi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jlsjyb.cn/gtrchhfokq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.vqdsnc.cn/gtjiuwenst.html

C#:   using System.Text;
来源：http://hz.yonumen.top/gtmirkbunz.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtbfjfencw.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtvmfrjqgy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gthcvzrybs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtddvwiiae.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtrzllhdfd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuxming.cn/gtvqxvyjcj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuetiantiany.cn/gtnbzpxbah.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gttrzadxlh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gtglbdzvol.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnqzz.top/gtjlsyprwh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sxryk.cn/gtngmhblpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gteozcojsd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtrlbdcvbr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtucdmjnck.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtvqnjwctv.html

Go:   func add(a, b int) int
来源：http://hz.yonumen.top/gtaaxqiipn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cdnleiting.top/gtvzonpdpt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtmltkitrn.html

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gtgowzppdm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtiaofvfqg.html

PHP:  // 无泛型
来源：http://hz.hongshengwenyu.top/gteglmbemm.html

JS:   // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtdqapydbm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhongyouzk.top/gtpeonmmbj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hongshengwenyu.top/gthgxicogo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtfegwukfw.html

Ruby: # 无泛型
来源：http://hz.daria6918.cn/gtszctihcl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtxydwwhdp.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtypfsjlwh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtyzucvijb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gtydiebbfq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtylkqmnxb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhiwuduotai.top/gteyvkmhpo.html

Java: // 无解构
来源：http://hz.jianghu66.top/gtxqgmhnja.html

Go:   // 无解构
来源：http://hz.nanxinkj.top/gtkabzxpdo.html

Ruby: a, b = pair
来源：http://hz.sxryk.cn/gtjekgyodf.html

C#:   var (a, b) = pair;
来源：http://hz.zycfv.cn/gtbuyegnzz.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtenvjeoya.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tianlin.xyz/gtqnfgchjb.html

PHP:  // 无重载
来源：http://hz.andypj.xyz/gtaftidigl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sxryk.cn/gtacbcbmkb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtvjojkbqw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gtdnaxrhpe.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtrudgorgr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yongpay.top/gtmsofrzie.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtuvphblla.html

================================================================================
来源：http://hz.yuxming.cn/gtpmpfkfyb.html

D. 数组 / 列表 / 集合
来源：http://hz.ywan-chungtsiang.top/gthgpaoxwx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtodrwfmhp.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtvwejzdwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.svipenyu.cn/gtcqmjocrb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtiqwrypaz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yanxiufei.cn/gtmslqzbky.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.svipenyu.cn/gtlozgxaqc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtfvoshptt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sweek.top/gtyrvxybhu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shangyingyoupin.top/gtdkxzqdgs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtgqbsdqyi.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtgwspymvi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtctxnpctb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtyhqnvymz.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtavkdkthk.html

TS:   arr.push(4);
来源：http://hz.fengsongda.top/gtttuooppr.html

Java: list.add(4);
来源：http://hz.hysaishi.cn/gtojogtulm.html

Go:   arr = append(arr, 4)
来源：http://hz.hywenlv.cn/gtopayilev.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtczagdvdn.html

C#:   list.Add(4);
来源：http://hz.shuidangran.top/gtippjqtwn.html

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtmcsbaahm.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtunqmdwnf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zdqjudy.top/gtafslpzvi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gtaahrwosc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.redwolf501.top/gtmxsuxncn.html

Java: list.add(0, 0);
来源：http://hz.svipenyu.cn/gtjggtnrsv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nwbrower.top/gtyoejidvb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jyoumei.cn/gtgvhptmov.html

C#:   list.Insert(0, 0);
来源：http://hz.vqdsnc.cn/gtdmlkgfvc.html

[D04] 删除元素
来源：http://hz.xingfuxueyuan.xyz/gtfafmetsi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jyoumei.cn/gtoieschld.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ivvv.top/gtxbsztuzk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtomdghcbu.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtbzwmluut.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gttvdfkcij.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtbyjgobpk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xinyue.icu/gtsumflwjo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangshuangyany.cn/gtgqtdadjb.html

[D05] 访问与修改元素
来源：http://hz.redwolf501.top/gtztxjtzju.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtysrfycpp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtcwnwwtyq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenzaomai.com/gtoasyknfa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gtxlmybtax.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gogol.net.cn/gtemlesoed.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gtiubgagan.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gthumplveu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtcvwodddb.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtgzxuecpc.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gttsiwgutd.html

PHP:  count($arr);
来源：http://hz.feifeiyinyue.top/gtcotpjhyl.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtmtvatqlr.html

TS:   arr.length
来源：http://hz.shuidangran.top/gtwifzjswz.html

Java: list.size();
来源：http://hz.guannengcc.top/gtzplkgjey.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtucqaqggi.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtytjxzliu.html

C#:   list.Count;
来源：http://hz.zhiwuduotai.top/gtycsaupvf.html

[D07] 切片 / 取子数组
来源：http://hz.hnxiangtu.top/gtkwsspqha.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258888.top/gtphegxmpe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xziqi.cn/gtfjcoiney.html

JS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtzohpavdj.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtegnlrhdw.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtgpbkiegv.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtazmgjzra.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gtzpzugquy.html

C#:   list.GetRange(1, 3);
来源：http://hz.jlsjyb.cn/gtqcyteylk.html

[D08] 合并两个数组
来源：http://hz.zycfv.cn/gtvittqbcc.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtflrviyps.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtpsymtsqb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuanzhike.top/gttdxyliji.html

TS:   [...a, ...b];
来源：http://hz.316326.xyz/gtpxcnkuge.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtubsmbzah.html

Go:   append(a, b...)
来源：http://hz.jinghuilouyu.cn/gtfumouraf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuanzhike.top/gtqqmjzylb.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangtech.top/gtlgoxvmpo.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtwpipokue.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtoehpiuxi.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtdukkozag.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yongpay.top/gthbtljaro.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.havefunace.top/gtsdbslabo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.9152youxi.cn/gtvaenmrxi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtevlwloxv.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtdfuvpyfd.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gtvucqbbpo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtxgnnsurn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtosifnpig.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ehwqpu.com/gttpochjxp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtrbeboalw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gtsnwpxyki.html


<!-- 参考信息 -->