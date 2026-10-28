代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtzdbyvqeq.html

[B10] 遍历同时拿索引
来源：http://hz.sxryk.cn/gtfhlwmkef.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fzhhl.top/gtnrkrjhlw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tian-w.cn/gtjtnhczlw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuanzx.com/gtpdjlzneo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.guannengcc.top/gtgeygwmku.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jqgufenzy.top/gtcqrcwudl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cucudq.cn/gtnbfvpliz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shuidangran.top/gtkhfbajou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yvedp.cn/gtphiborlf.html

[B11] 生成数字序列 / 区间
来源：http://hz.yueranfly.top/gtedtnksmc.html

Py:   list(range(0, 10, 2))
来源：http://hz.andypj.xyz/gtvhijdyxk.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgfzy.top/gtuurkdayh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtxozdfdku.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtyraecqzj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.daxiang520.top/gttqhwpbzu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinyuanbaomall.cn/gticxmhvui.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hammf.cn/gtmdhbhfpv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.feifeiyinyue.top/gtqgqyshgk.html

[B12] 跳出多层循环
来源：http://hz.0kj1m.cn/gtuofggmih.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zycfv.cn/gtsgyydvts.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj202588.top/gtggwgeiac.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtpfbbtzlm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtzpyzlsnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtesrfnbor.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhijiandao.cn/gthzsvktoa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gthvpxfuhq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ehwqpu.com/gtgqbrmzog.html

[B13] 判断是否为数字
来源：http://hz.quarkkingdee.top/gtamwndvbt.html

Py:   isinstance(x, (int, float))
来源：http://hz.haohaochexian.top/gtnmlaqzai.html

PHP:  is_numeric($x)
来源：http://hz.daria6918.cn/gthgetjebd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtcwhjjtsg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtlgqyktzc.html

Java: x instanceof Number
来源：http://hz.yj202588.top/gtfamdyzjv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.haohaochexian.top/gtgwdwpyxe.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ivvv.top/gtxvcdyptm.html

C#:   x is int or double or decimal
来源：http://hz.yangfankeji.com/gtbefizbxn.html

[B14] 判断值是否在集合内
来源：http://hz.yuxming.cn/gtrrvzwdqe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pengpengdd.cyou/gtzuxydvps.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.smart0.xyz/gtyirbbkjm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtyminnpas.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtlyvcdikg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hammf.cn/gtxejhlfif.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gttvwxshgj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinghuilouyu.cn/gtjblofayc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cqqwz.cn/gtkspszeno.html

[B15] 布尔运算与取反
来源：http://hz.xuetiantiany.cn/gtkyybvqar.html

Py:   a and b or not c
来源：http://hz.zycfv.cn/gtphsndlhe.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gtpzfelbea.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtweyucdwk.html

TS:   a && b || !c
来源：http://hz.andypj.xyz/gtydxomvlk.html

Java: a && b || !c
来源：http://hz.yueranfly.top/gtjpusmktu.html

Go:   a && b || !c
来源：http://hz.yuanzhike.top/gthuggnqsx.html

Ruby: a && b || !c
来源：http://hz.jyoumei.cn/gtuqkcymny.html

C#:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtwmsqafux.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigfzy.top/gtyneascux.html

Py:   if not data: return
来源：http://hz.yueranfly.top/gtlcdhubwt.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gtwpfugvmn.html

JS:   if (!data) return;
来源：http://hz.shuidangran.top/gtawxkbjvm.html

TS:   if (!data) return;
来源：http://hz.c1oappe.top/gtqmiyavpr.html

Java: if (data == null) return;
来源：http://hz.nwbrower.top/gtmcdfhfad.html

Go:   if data == nil { return }
来源：http://hz.ppjwa.cn/gtafmgaaib.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtozjliqqs.html

C#:   if (data == null) return;
来源：http://hz.cheryme.top/gtebrozggy.html

================================================================================
来源：http://hz.birdmap.top/gtxdspvuoo.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtiiwwebav.html

================================================================================
来源：http://hz.fengsongda.top/gtupdjespk.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gtxkqlfpnx.html

Py:   def add(a, b): return a + b
来源：http://hz.hongshengwenyu.top/gteumdiuwm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtfqigthaw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj202588.top/gtjgqelckm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtitsniczh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtmkmalgkh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gotoacloud.top/gtbksdsipw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.c1oappe.top/gtvwrmiycz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtygpdfryp.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gtieqrvwuu.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtxddsrjwh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhiwuduotai.top/gtchwzasys.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gtidvnataf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtcgnaynef.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.bjfxy.top/gtjzknxhfm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtlmaoswri.html

Ruby: def greet(name = "World") = name
来源：http://hz.sysykeji.top/gtwqdryqpi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guannengcc.top/gtgolvntdd.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtkpyqwkzt.html

Py:   def total(*args): return sum(args)
来源：http://hz.jlsjyb.cn/gtojqcgowa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gzhubu.top/gtwqwgkhzs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtgxoqitpr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtliawwagv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj202588.top/gtebvazvax.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.meibo888.top/gtdhotgupz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtwgfabfrx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigfzy.top/gtobycwtia.html

[C04] 命名参数 / 关键字参数
来源：http://hz.birdmap.top/gteeedocxb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gtyurwpflp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aizwys.cn/gtlxjzryew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gthlljdmqw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.snrcjt.cn/gtrbktdumx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guannengcc.top/gtnjrmuflz.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtdprdfjzs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtdtsjndbf.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtrcfbmlev.html

[C05] 返回多个值
来源：http://hz.quarkkingdee.top/gtegogieab.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gtzfgmibvx.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtkplyxmgy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtsfepswyb.html

TS:   return { a, b };
来源：http://hz.hywenlv.cn/gtiqungvtg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtogbbyhue.html

Go:   return a, b
来源：http://hz.xziqi.cn/gtfgtzxtis.html

Ruby: return a, b
来源：http://hz.kuanghao11.cn/gtjauzqjgu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gzhubu.top/gtajjvttzi.html

[C06] 匿名函数 / lambda
来源：http://hz.jyoumei.cn/gtesuioatp.html

Py:   square = lambda x: x * x
来源：http://hz.daria6918.cn/gtmxjilzas.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtuvbsxpat.html

JS:   const square = x => x * x;
来源：http://hz.haohaochexian.top/gtgflkqgfh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinyuanbaomall.cn/gtkwepzlkj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.smart0.xyz/gtvxtguxgh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.dashuyun.cn/gtvnbdvrdu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.haohaochexian.top/gtswvcxtol.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.316326.xyz/gtlwmwiihp.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtsndfabwp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhijiandao.cn/gtyvtwesmg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenzaomai.com/gtppzcwnbj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.kuanghao11.cn/gtjerjqnsj.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtilxqpvtm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jiagoushi.top/gtpaydvfhd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtipnirgrn.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangdashe.top/gtmwplglgh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hywenlv.cn/gtbemrbzwz.html

[C08] 闭包
来源：http://hz.iojbl.cn/gtyskcrvao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daria6918.cn/gtbkfiebur.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guannengcc.top/gtlgevergz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtbjbuebmm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gttfgtjcks.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.birdmap.top/gtbocufhxm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shangyingyoupin.top/gtrckfdyxs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zdqjudy.top/gtrijmcpzi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtsgkhybam.html

[C09] 递归
来源：http://hz.jyoumei.cn/gtjgvxhigp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gttduocpkd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtbjfytrje.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtffkigrvv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtfuaewzuu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dianchejie.cn/gtcmnnhurf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hfpthk.cn/gtwxblzgxp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydzc1.top/gtgnlwaibn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yongpay.top/gtfmfilxcg.html

[C10] 变量作用域
来源：http://hz.wangdashe.top/gtailnxmgh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gttwpnzssn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtdwfesurb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guannengcc.top/gtideahqxk.html

TS:   同 JS
来源：http://hz.iojbl.cn/gtzvreiewl.html

Java: 方法内为块级作用域
来源：http://hz.andypj.xyz/gtkwezcqor.html

Go:   花括号块级作用域
来源：http://hz.jyoumei.cn/gtsgcwprfg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258888.top/gtuhequjin.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gtgdqaohkj.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtaobzwggb.html

Py:   from module import func
来源：http://hz.chenjidiqi.icu/gtohcuvtxu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gttdwrdmow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pengpengdd.cyou/gtdvzsfgdo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxuanxn.top/gtzejhxbwj.html

Java: import java.util.List;
来源：http://hz.zhijiandao.cn/gthwllrevb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jianghu66.top/gtmbctunrl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtfegrgavu.html

C#:   using System.Text;
来源：http://hz.jqgufenzy.top/gtgppxgyvl.html

[C12] 立即执行函数 IIFE
来源：http://hz.c1oappe.top/gtqchqlluh.html

Py:   (lambda: print("run"))()
来源：http://hz.jyoumei.cn/gtjbmynpwz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258.top/gtdemrknhn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtlcnqnxwj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtybrhahfy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.mhx1999.top/gtljgvearp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zdqjudy.top/gtmnvhibru.html

Ruby: -> { puts "run" }.call
来源：http://hz.xinyue.icu/gtoyazixer.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtwozvslfh.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuanzhike.top/gtzemmkdwu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuanzhike.top/gtdnedozql.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtxfqxydid.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtcsymwfra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtgnqkkxik.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtdlkjtsvz.html

Go:   func add(a, b int) int
来源：http://hz.iojbl.cn/gtmzqjumes.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxuanxn.top/gtkfyjujso.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.316326.xyz/gtzmtgzmhg.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtnyspknqu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daria6918.cn/gtsswvxxmo.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtugyqlwlb.html

JS:   // 无泛型
来源：http://hz.hongshengwenyu.top/gtbfgdpbyd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gttllkngzs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hammf.cn/gtcmeuqcvw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtajkulvfw.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtbumrzyqe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtlopvzjvo.html

[C15] 解构 / 展开参数
来源：http://hz.cdnleiting.top/gtnrbpksbp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cashguo.top/gtrgxhniwu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtguzbaubp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gttjeyfies.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aizwys.cn/gthohuhfic.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtovhyktqy.html

Go:   // 无解构
来源：http://hz.ybcxt.top/gttwkfikuy.html

Ruby: a, b = pair
来源：http://hz.hammf.cn/gtzlpubgbq.html

C#:   var (a, b) = pair;
来源：http://hz.ywan-chungtsiang.top/gtvdvjxdez.html

[C16] 函数 / 方法重载
来源：http://hz.shuidangran.top/gtnepixfdn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtpjqzcono.html

PHP:  // 无重载
来源：http://hz.zycfv.cn/gtoinyiiwa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cqqwz.cn/gtarebupbu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtwdvuilku.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jlsjyb.cn/gtxroglgsa.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtmosnhygj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gtjixfdqfm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fzhhl.top/gtdwpzgjcp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttkmzilcc.html

D. 数组 / 列表 / 集合
来源：http://hz.sufxvd.cn/gtknloudlx.html

================================================================================
来源：http://hz.xuanzx.com/gtmvdfqtup.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtjaeokjel.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yangfankeji.com/gtoetsmtms.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gtsbxjvois.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pengpengdd.cyou/gttdirllkt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tianlin.xyz/gtumnkcnth.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtdgemypue.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuanzx.com/gtwtoqcxkw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtlceuhgnj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtmyxeemiq.html

[D02] 追加元素到末尾
来源：http://hz.ppjwa.cn/gtzdarwcww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtymmrfsyn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnxiangtu.top/gtuiatgnid.html

JS:   arr.push(4);
来源：http://hz.shuidangran.top/gtvqqlosbg.html

TS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gtqfusnbnw.html

Java: list.add(4);
来源：http://hz.jianghu66.top/gtjmwpbsxd.html

Go:   arr = append(arr, 4)
来源：http://hz.hnqzz.top/gtiazaopab.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtspqntnxg.html

C#:   list.Add(4);
来源：http://hz.xinyue.icu/gttbcfodtu.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtdcgmfbzw.html

Py:   arr.insert(0, 0)
来源：http://hz.ywan-chungtsiang.top/gtygfakoxg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gttpcyspyw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aizwys.cn/gtbuhsbzzv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.andypj.xyz/gtoyisytly.html

Java: list.add(0, 0);
来源：http://hz.yj20258.top/gtaxzkrhgc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangdashe.top/gtgfuwolnq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.c1oappe.top/gthiwmomhp.html

C#:   list.Insert(0, 0);
来源：http://hz.ydjk.org.cn/gtckahwubp.html

[D04] 删除元素
来源：http://hz.ydjk.org.cn/gtxxqaawcg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxuanxn.top/gtimzavhea.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gticcmsyds.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dianchejie.cn/gtinfeyexm.html

TS:   arr.splice(0, 1);
来源：http://hz.sufxvd.cn/gtbzlpocle.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yueranfly.top/gtvvonvdqm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtjkntwzig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtpxbbivdw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhixingplan.top/gtlgvjflco.html

[D05] 访问与修改元素
来源：http://hz.shuidangran.top/gtszzzuela.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtlhsesdrb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aizwys.cn/gtqejptzxw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtjstwkelo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinghuilouyu.cn/gtkgevbbcd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtywkglegx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yonumen.top/gtuslabvri.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtyaaldmsz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtszozsscc.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtxizsavqf.html

Py:   len(arr)
来源：http://hz.zhiwuduotai.top/gtzpzekuko.html

PHP:  count($arr);
来源：http://hz.gogol.net.cn/gtbmlaeuqr.html

JS:   arr.length
来源：http://hz.smart0.xyz/gtclatftna.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtxpubgzln.html

Java: list.size();
来源：http://hz.guannengcc.top/gtxkkmgpod.html

Go:   len(arr)
来源：http://hz.yvedp.cn/gttgcxyuzo.html

Ruby: arr.length; arr.size
来源：http://hz.aizwys.cn/gtaridjhhe.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtjqnecefk.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtsoitmckk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.quarkkingdee.top/gtezfzptsg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gtsceqzbai.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtjnbbfvuk.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtujvwteex.html

Java: list.subList(1, 4);
来源：http://hz.316326.xyz/gtqoxqwmtr.html

Go:   arr[1:4]
来源：http://hz.jqgufenzy.top/gtglzebyoa.html

Ruby: arr[1, 3]
来源：http://hz.jinyuanbaomall.cn/gtnappoaqc.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gtghaamizw.html

[D08] 合并两个数组
来源：http://hz.zhiwuduotai.top/gtpxuwjyes.html

Py:   a + b;  a.extend(b)
来源：http://hz.xziqi.cn/gtznmraxqk.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtegpleuck.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtxnxkhlah.html

TS:   [...a, ...b];
来源：http://hz.ivvv.top/gtahrnkecj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtyblclndt.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gtrqhzzsed.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guannengcc.top/gtcsqftfbf.html

C#:   a.Concat(b).ToList()
来源：http://hz.quarkkingdee.top/gtjktjzfpc.html

[D09] 排序（升序）
来源：http://hz.c1oappe.top/gtqlzbecdr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gthpfeqsql.html

PHP:  sort($arr);
来源：http://hz.xuetiantiany.cn/gtmlwxsclu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yonumen.top/gtpcfvtawg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtsujwobtl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gtqydjtazx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.52xcode.cn/gtexnkzmfe.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtrcqtytji.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtnepokjir.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aizwys.cn/gtvpthedsu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtqybeaxqe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtdsnmputb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gthlruivui.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtcvvfapcu.html


<!-- 参考信息 -->