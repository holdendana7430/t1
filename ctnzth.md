代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtqohxhzez.html

[B10] 遍历同时拿索引
来源：http://hz.hongshengwenyu.top/gttybitesm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daria6918.cn/gtacohwcox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.0kj1m.cn/gtrylfnmzd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinyuanbaomall.cn/gtrzhrcvvm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenjidiqi.icu/gtetwjvdhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.daria6918.cn/gtregpalef.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.9152youxi.cn/gtufhusled.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgufenzy.top/gtwgkvixbp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.svipenyu.cn/gtcyeedkdy.html

[B11] 生成数字序列 / 区间
来源：http://hz.guannengcc.top/gttkxbjpyt.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhijiandao.cn/gtxmvpbtxu.html

PHP:  range(0, 10, 2);
来源：http://hz.feifeiyinyue.top/gtmfcmpobg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yongpay.top/gtbjnnwzpo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtorwasijs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cqqwz.cn/gtwtkbafkh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xinyue.icu/gtrtzpxxth.html

Ruby: (0...10).step(2).to_a
来源：http://hz.redwolf501.top/gtbajokpyg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xziqi.cn/gtcsqootfh.html

[B12] 跳出多层循环
来源：http://hz.gotoacloud.top/gtfxdjnjis.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yueranfly.top/gtwbqltksk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ybcxt.top/gtzvpfirmg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtadczadwt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gttiqdejjq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtqjnvggol.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yonumen.top/gthpfoxtyt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258888.top/gthwnqlezq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xuetiantiany.cn/gtbbeizahw.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gtwdbnvyzo.html

Py:   isinstance(x, (int, float))
来源：http://hz.jyoumei.cn/gtbqmksnah.html

PHP:  is_numeric($x)
来源：http://hz.jiagoushi.top/gtwvzsiiqx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtjyfsmgrq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gaohongyu789.top/gtlwikzwgw.html

Java: x instanceof Number
来源：http://hz.sufxvd.cn/gtaacunsaq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258.top/gtkzgnhutj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxuanxn.top/gtycloyfoc.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gthszztwgk.html

[B14] 判断值是否在集合内
来源：http://hz.cucudq.cn/gtgfytyaco.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tian-w.cn/gtdnzwmqyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xingfuxueyuan.xyz/gtxwlsfojs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.vqdsnc.cn/gthjutkwhc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtyapnslcm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinghuilouyu.cn/gtxoeammcu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhiwuduotai.top/gtcshlclmy.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gtljovtufy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nwbrower.top/gtkglokwlt.html

[B15] 布尔运算与取反
来源：http://hz.sufxvd.cn/gtzzifvpbo.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtnlvwrcfm.html

PHP:  $a && $b || !$c
来源：http://hz.hammf.cn/gtrirseqya.html

JS:   a && b || !c
来源：http://hz.chenlongwang.top/gtpawnfcac.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtxkpglamm.html

Java: a && b || !c
来源：http://hz.yj20258.top/gtplkcnhbz.html

Go:   a && b || !c
来源：http://hz.gotoacloud.top/gtbyddrbmk.html

Ruby: a && b || !c
来源：http://hz.yonumen.top/gtmlfneumw.html

C#:   a && b || !c
来源：http://hz.yj20258.top/gtohsemuqb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nanxuanxn.top/gtusieyivp.html

Py:   if not data: return
来源：http://hz.52xcode.cn/gthzcmekfp.html

PHP:  if (!$data) { return; }
来源：http://hz.tian-w.cn/gtzjcivcee.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gtodpoxsfj.html

TS:   if (!data) return;
来源：http://hz.ydjk.org.cn/gtrhrxrzxj.html

Java: if (data == null) return;
来源：http://hz.xinyue.icu/gtapfblstq.html

Go:   if data == nil { return }
来源：http://hz.jinghuilouyu.cn/gtwjkdiizn.html

Ruby: return if data.nil?
来源：http://hz.hongshengwenyu.top/gtdfoonnvu.html

C#:   if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtklfgjvfl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtldwpvptt.html

C. 函数与作用域
来源：http://hz.chenjidiqi.icu/gtiockmmkb.html

================================================================================
来源：http://hz.dianchejie.cn/gtlsgzkobv.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtosotyini.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtfemrufmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtcvimcywm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtocpgslfm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtpvoqltmx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtonmhjqxb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gaohongyu789.top/gtxxysquvf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yangfankeji.com/gtffrjawdt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtwcsndkro.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gtngwkgimz.html

Py:   def greet(name="World"): return name
来源：http://hz.gotoacloud.top/gtulerggrh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daxiang520.top/gttydfrelx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hywenlv.cn/gtspkdgxah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gtpmoonghe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sysykeji.top/gtlxemxlir.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.0kj1m.cn/gtcvuynfzz.html

Ruby: def greet(name = "World") = name
来源：http://hz.pycfn.com/gthajdbzch.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxuanxn.top/gtggaopzdf.html

[C03] 可变参数
来源：http://hz.hongshengwenyu.top/gtkhuwggcs.html

Py:   def total(*args): return sum(args)
来源：http://hz.xinyue.icu/gtodezxstr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gtksnklovb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtdxcrhjuy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtpynmdcyk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.9152youxi.cn/gtvkfacnbo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangtech.top/gtanjiascv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guowangkeji.top/gtlfyzeiyj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtqrmzdkwc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtiavbepxh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fzhhl.top/gtjflevtgp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gzhubu.top/gtqqgfpwil.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtsijprwvk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtynboshon.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuanzx.com/gtzpsfewhi.html

Go:   // 无：用配置结构体参数
来源：http://hz.dianchejie.cn/gthyseoumo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtogdlmbfe.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtxwmcsagl.html

[C05] 返回多个值
来源：http://hz.0kj1m.cn/gtqvcmswah.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtnvwxzwdq.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtbtxeqopo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtopmgosyn.html

TS:   return { a, b };
来源：http://hz.yuanzhike.top/gtcwifxnzf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtbcgrsjix.html

Go:   return a, b
来源：http://hz.0kj1m.cn/gtxmvjysmv.html

Ruby: return a, b
来源：http://hz.fengsongda.top/gtyqdydexp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuetiantiany.cn/gtuliblufu.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtgedvfvij.html

Py:   square = lambda x: x * x
来源：http://hz.zhongyouzk.top/gtyqymimub.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nwbrower.top/gtthjepsdz.html

JS:   const square = x => x * x;
来源：http://hz.shangyingyoupin.top/gtybjwgtfc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.andypj.xyz/gtkcdgmzss.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gthwepbosk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258888.top/gtmnyecpmo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgufenzy.top/gtnfvlbcfw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtbdaqnxit.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtjczgseiy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hongshengwenyu.top/gthkulfezl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.smart0.xyz/gtjhyhejop.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.fzhhl.top/gtyxyiaadg.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtgwduftay.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gotoacloud.top/gtunjpwrsg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtkgggdvhv.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gtxkznvzoh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nanxinkj.top/gtkoaxnqkc.html

[C08] 闭包
来源：http://hz.sxryk.cn/gtvrrahseu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yvedp.cn/gtrqzlfvlz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnxiangtu.top/gtlsspqkqg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtbrktvnvn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtbvqecqdw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtmeosxrkm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.andypj.xyz/gtopmwljha.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.birdmap.top/gtsyuhjzeq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtnkgnemtt.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gtuoqivlft.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zycfv.cn/gtrcexylpa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gtheeossqy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtqinjszbv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtrxjebfyx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtcpboptoa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenzaomai.com/gttzqehsrf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtkujgbaee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ivvv.top/gthytqsmbv.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtqgjiblhr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jianghu66.top/gtlcbwicny.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tian-w.cn/gtavgotuge.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtccxhppeq.html

TS:   同 JS
来源：http://hz.hnqzz.top/gtviqmctvm.html

Java: 方法内为块级作用域
来源：http://hz.daria6918.cn/gtptwzlopz.html

Go:   花括号块级作用域
来源：http://hz.yj20258.top/gttqhtogys.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daxiang520.top/gtupimybip.html

C#:   块级作用域
来源：http://hz.chenjidiqi.icu/gtmgudjlmk.html

[C11] 模块导入与导出
来源：http://hz.pycfn.com/gtcdszinwx.html

Py:   from module import func
来源：http://hz.c1oappe.top/gtrqarsokd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jlsjyb.cn/gtjkckobfc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtuvcktqdb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shzxlz.cn/gtqdvxokux.html

Java: import java.util.List;
来源：http://hz.chenlongwang.top/gtdwzudxft.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtvwbcjmay.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtwsqvcdss.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtruqbzeyj.html

[C12] 立即执行函数 IIFE
来源：http://hz.havefunace.top/gthvitgrno.html

Py:   (lambda: print("run"))()
来源：http://hz.daria6918.cn/gtvrpftlsj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtssbwisdh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtiaooelrb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtmqcjtyle.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtulxutxes.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.mhx1999.top/gtqjcyfxjb.html

Ruby: -> { puts "run" }.call
来源：http://hz.redwolf501.top/gtvxtpdipi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tianlin.xyz/gtcgxybpdg.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gthjxocnqu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtxufezxiv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtcrxfhwhs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnqzz.top/gtuwypqgnd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtgfasfiqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtyaejsfgb.html

Go:   func add(a, b int) int
来源：http://hz.aizwys.cn/gtxfgvmbxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.52xcode.cn/gtrkdvbwns.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ehwqpu.com/gtxnkntmxn.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtyjsdyjsy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtirwelrxq.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtnrcrfcsn.html

JS:   // 无泛型
来源：http://hz.smart0.xyz/gtctlqpfzq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtjmpnfsjw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtsingvhhn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xinyue.icu/gtlxkuziuu.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gthnuyfsqw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gtlulyssfu.html

[C15] 解构 / 展开参数
来源：http://hz.aibaodan.cn/gtoqnvkfja.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtcoyvvltz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtzvukqqcd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gthrmrrwed.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.52xcode.cn/gtwudpaeqr.html

Java: // 无解构
来源：http://hz.cheryme.top/gtyetfudyd.html

Go:   // 无解构
来源：http://hz.bjfxy.top/gtwtodlcpp.html

Ruby: a, b = pair
来源：http://hz.zhoulong.xyz/gtcanansmn.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtenlnodlb.html

[C16] 函数 / 方法重载
来源：http://hz.guowangkeji.top/gtfoyhruie.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sweek.top/gtucrzwqfz.html

PHP:  // 无重载
来源：http://hz.sysykeji.top/gtuftbgsvh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.smart0.xyz/gtxjthbwgk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.pengpengdd.cyou/gtpjyqrkqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sysykeji.top/gtkrxgujrk.html

Go:   // 无重载：用不同函数名
来源：http://hz.xylfe.cn/gtkawaxoqz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cdnleiting.top/gtseybbpix.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gaohongyu789.top/gtoushzjmr.html

================================================================================
来源：http://hz.jqgufenzy.top/gtajfgdogr.html

D. 数组 / 列表 / 集合
来源：http://hz.kuanghao11.cn/gtwwofkeoz.html

================================================================================
来源：http://hz.daxiang520.top/gtiydurhuc.html

[D01] 创建数组 / 列表
来源：http://hz.yj202588.top/gtosonncjy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtcalxlpjh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gtajyerurx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.9152youxi.cn/gtidthyydi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtqaldrumq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhengqikj.top/gtpjlgbwma.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sweek.top/gtmbrriqhe.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtgmcvegic.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.9152youxi.cn/gtufqeuutb.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gthskvmhbu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hywenlv.cn/gtqccoavnk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigufen.top/gtznhalvya.html

JS:   arr.push(4);
来源：http://hz.yuxming.cn/gtvnfsoozq.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtemdnljda.html

Java: list.add(4);
来源：http://hz.yvedp.cn/gtbqrcnffn.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gtccjoiosc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtuqggaajz.html

C#:   list.Add(4);
来源：http://hz.jyoumei.cn/gtlghiakja.html

[D03] 在指定位置插入元素
来源：http://hz.hfpthk.cn/gtqrzcgead.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtvkqzwgfs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtoywuqgoi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtvqqejwjm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ybcxt.top/gtjdhshtrt.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtekmjzhdw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydzc1.top/gtfparyhlr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangshuangyany.cn/gtvisyldhj.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtmljokinh.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtpufwfmyj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtdkvlkjum.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gtvwiurnmq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gttksxudas.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtphgownxr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jlsjyb.cn/gtzyhhypjh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtcgdoirgz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtmqirtbey.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daxiang520.top/gtttjekech.html

[D05] 访问与修改元素
来源：http://hz.shangyingyoupin.top/gttkfcacgu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtsztxoorw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jiagoushi.top/gthfxpmmnl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.9152youxi.cn/gtqmupvjor.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtewshjxfc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gaohongyu789.top/gtaztyygxg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtbtgedtvu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtosirjcai.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gtadtkttkp.html

[D06] 数组长度
来源：http://hz.zdqjudy.top/gtoyccahvn.html

Py:   len(arr)
来源：http://hz.wangdashe.top/gtpjexqibi.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtwblrqtro.html

JS:   arr.length
来源：http://hz.havefunace.top/gtjyiclsee.html

TS:   arr.length
来源：http://hz.ybcxt.top/gtjhvvhdum.html

Java: list.size();
来源：http://hz.gogol.net.cn/gtiqhuryvf.html

Go:   len(arr)
来源：http://hz.wangshuangyany.cn/gtbcnnwyhd.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtiskulnis.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtjebkoiat.html

[D07] 切片 / 取子数组
来源：http://hz.jlsjyb.cn/gtnxxfgyto.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gtbhrmdwqi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxinkj.top/gtyrqcrojr.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtwaywmvdx.html

TS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtixvivuvn.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtxlobubek.html

Go:   arr[1:4]
来源：http://hz.yj20258.top/gtuzkaucup.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gthsxeiuli.html

C#:   list.GetRange(1, 3);
来源：http://hz.cheryme.top/gtpmcnhjga.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtngahulut.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtdvhxbydp.html

PHP:  array_merge($a, $b);
来源：http://hz.xingfuxueyuan.xyz/gtmqienapm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guowangkeji.top/gtuhuujkfy.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtcsdmopom.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtyyimqsek.html

Go:   append(a, b...)
来源：http://hz.pengpengdd.cyou/gtshtzwzex.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtdutljlnh.html

C#:   a.Concat(b).ToList()
来源：http://hz.tanke756.top/gtdzdkvykj.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtttfldwwl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtljaiibym.html

PHP:  sort($arr);
来源：http://hz.wangdashe.top/gtvprqowif.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtixeuoaod.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhaomingkeji.xyz/gtjpqfmjbb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xylfe.cn/gtlbelalnh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtbkewhxof.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtoppolbth.html

C#:   list.Sort();
来源：http://hz.dianchejie.cn/gtltwrsexx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtnstwoxvw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daria6918.cn/gtiysltqpb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtfiekjkoh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtnbzeotlk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtbyribfqu.html


<!-- 参考信息 -->