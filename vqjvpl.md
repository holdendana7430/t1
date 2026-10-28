代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtyqnyaxcu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nwbrower.top/gtgnomkmue.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.svipenyu.cn/gtniesiseh.html

[B12] 跳出多层循环
来源：http://hz.zhijiandao.cn/gtedjhlvrr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pycfn.com/gtoejiueyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinyuanbaomall.cn/gtvikclniu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtqkqjexpc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtwkqbsran.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gogol.net.cn/gtkxyqjhrb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtvfvuthhi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cucudq.cn/gtsmjffhhr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.mhx1999.top/gtwcvxxljy.html

[B13] 判断是否为数字
来源：http://hz.cqqwz.cn/gtiwpwwuhl.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhoulong.xyz/gtacymdhrg.html

PHP:  is_numeric($x)
来源：http://hz.dianchejie.cn/gtbrerqimj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jianghu66.top/gtvbbkgzkl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gthjczdrny.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtcvogbzfh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daxiang520.top/gtxdwjgjnu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangdashe.top/gtxiozvmar.html

C#:   x is int or double or decimal
来源：http://hz.shuidangran.top/gtsvtkafta.html

[B14] 判断值是否在集合内
来源：http://hz.zdqjudy.top/gtwgcpmfrq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.c1oappe.top/gtmypgfgdf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sufxvd.cn/gtmwwysuai.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtjladtqeq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yuxming.cn/gtywnurmvv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hammf.cn/gtgaomhbya.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinyuanbaomall.cn/gtvcaopxam.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenjidiqi.icu/gtsjsfhctk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.316326.xyz/gtidlzdbxs.html

[B15] 布尔运算与取反
来源：http://hz.jinyuanbaomall.cn/gtnbycrzwz.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtykjdytmj.html

PHP:  $a && $b || !$c
来源：http://hz.smart0.xyz/gtgwfyjctl.html

JS:   a && b || !c
来源：http://hz.quarkkingdee.top/gtvewyuaod.html

TS:   a && b || !c
来源：http://hz.shuidangran.top/gtnifyvqyb.html

Java: a && b || !c
来源：http://hz.ppjwa.cn/gthydadtei.html

Go:   a && b || !c
来源：http://hz.haohaochexian.top/gtbspijter.html

Ruby: a && b || !c
来源：http://hz.aizwys.cn/gtctscmzyi.html

C#:   a && b || !c
来源：http://hz.gotoacloud.top/gtyrudghxa.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xingfuxueyuan.xyz/gtfdlfzcys.html

Py:   if not data: return
来源：http://hz.zhoulong.xyz/gtyfbglbsk.html

PHP:  if (!$data) { return; }
来源：http://hz.hammf.cn/gtuzmzvgxp.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtcxquevvu.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtojtkszwi.html

Java: if (data == null) return;
来源：http://hz.guannengcc.top/gttlfpnxes.html

Go:   if data == nil { return }
来源：http://hz.yuxming.cn/gtomsjlgtq.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gtwnsegxjt.html

C#:   if (data == null) return;
来源：http://hz.snrcjt.cn/gttcnczkrq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtulxwctml.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtactvgqpg.html

================================================================================
来源：http://hz.shzxlz.cn/gtletlekdh.html

[C01] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtphzokpma.html

Py:   def add(a, b): return a + b
来源：http://hz.yonumen.top/gtkzzovqgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtzozuhtno.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sxryk.cn/gtdvsvyzve.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtgdaomiuk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtipxxkcgf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fzhhl.top/gtdrutilpd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.redwolf501.top/gtftuvcrrc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtlcaqsgec.html

[C02] 默认参数
来源：http://hz.c1oappe.top/gtxjpgrdty.html

Py:   def greet(name="World"): return name
来源：http://hz.aizwys.cn/gtbfemwcvo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhixingplan.top/gtnwoihvjr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtcwrqyrjf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtjbaqlstr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gtworpbhdx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gttbqtgtnv.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gtmfbauwpv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gthswcaksb.html

[C03] 可变参数
来源：http://hz.zhoulong.xyz/gtmzfrdmas.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtefzavmpq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.haohaochexian.top/gtpezguxti.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtpgtemhif.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtyetjaalo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hnxiangtu.top/gtpmjtwtws.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gtvdmopcis.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtogewflpl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zycfv.cn/gtxfpueidf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhiwuduotai.top/gtpbkqthpl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gtlilcsvgi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hammf.cn/gtvlhmsjtb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.meibo888.top/gtypcglcme.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zdqjudy.top/gtlpudizaa.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhixingplan.top/gtfvjidgci.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgufenzy.top/gtziyrosuk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtanafjrqj.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gttwurrlwd.html

[C05] 返回多个值
来源：http://hz.dianchejie.cn/gtmsfzsvva.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtcysbdgfn.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtaaucufxn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtkyyptpad.html

TS:   return { a, b };
来源：http://hz.jlsjyb.cn/gtkqfpmscy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangshuangyany.cn/gtjmxdyjae.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtqfajbswn.html

Ruby: return a, b
来源：http://hz.chenzaomai.com/gtmityqapy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sysykeji.top/gtlwuvjzzu.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gtizpcusbd.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtqyjknoks.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenzaomai.com/gtwkwbnkfr.html

JS:   const square = x => x * x;
来源：http://hz.shzxlz.cn/gtitzlzoci.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.smart0.xyz/gtgzxofmsc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ivvv.top/gtjxfghexe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.smart0.xyz/gtxhqpldpj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtynkzvwjp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgufenzy.top/gthlzjyrgk.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtqmjpaghs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sysykeji.top/gtzlrzicbr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.andypj.xyz/gtioivgxej.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.feifeiyinyue.top/gtvkiinwqf.html

TS:   arr.map(String)
来源：http://hz.ydzc1.top/gtdqdqlybz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cashguo.top/gtgtvlqoxq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtdkgkwkeg.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtndjteawd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.andypj.xyz/gtpkxdzpzp.html

[C08] 闭包
来源：http://hz.ydzc1.top/gtnxuemyea.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gtnflnfybr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj202588.top/gtiipmpfyx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtkonglmzb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtollctlok.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gtiqxzrnjx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gtfimwlzlq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hywenlv.cn/gtnfphczwe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtjbfamgqy.html

[C09] 递归
来源：http://hz.hammf.cn/gtmunvreby.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cqqwz.cn/gtkfeybjyo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shzxlz.cn/gtttrgeyrl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.redwolf501.top/gtrevjncjb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtdbthekga.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.birdmap.top/gtjzaiddkn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shangyingyoupin.top/gtxfzfinsq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ybcxt.top/gtxpsystah.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gogol.net.cn/gtmdakckhf.html

[C10] 变量作用域
来源：http://hz.sysykeji.top/gtfdngcspy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtxsjhjvye.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhijiandao.cn/gtllzydssp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhoulong.xyz/gtuvqaawyb.html

TS:   同 JS
来源：http://hz.jyoumei.cn/gtlwbxrxif.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtngjxttdt.html

Go:   花括号块级作用域
来源：http://hz.daria6918.cn/gtbtrsvxyd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtbobituni.html

C#:   块级作用域
来源：http://hz.ydzc1.top/gttaeaeiew.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gttrvalryj.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gtxdppsvuq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yanxiufei.cn/gtqnbyogtr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.9152youxi.cn/gtpwnwbwwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xinyue.icu/gtwnkcymrl.html

Java: import java.util.List;
来源：http://hz.hammf.cn/gtxytwunvo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuetiantiany.cn/gthitvxvzj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aibaodan.cn/gtbzsdxpos.html

C#:   using System.Text;
来源：http://hz.hnxiangtu.top/gtjondedne.html

[C12] 立即执行函数 IIFE
来源：http://hz.hfpthk.cn/gtpgqljxlx.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtnqohrzxw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxinkj.top/gtpakbblrm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtutuztcdx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtvkkaubft.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuetiantiany.cn/gtgwgusmrd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yonumen.top/gtqwnzclui.html

Ruby: -> { puts "run" }.call
来源：http://hz.ppjwa.cn/gtcjavfzku.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.havefunace.top/gtrqhybdyd.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtqrzbwjfl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtcbxrlyls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtumgavjey.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jiagoushi.top/gtacrsawzf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aizwys.cn/gtlcnmiytu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtcuensyik.html

Go:   func add(a, b int) int
来源：http://hz.hywenlv.cn/gtvqpwtfqv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gtgcbgdqqf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtmjrgqphj.html

[C14] 泛型函数
来源：http://hz.jlsjyb.cn/gtpwejndbf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtvfbsqegp.html

PHP:  // 无泛型
来源：http://hz.pycfn.com/gtyvkdcixl.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gtmfardear.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhoulong.xyz/gttzbrokud.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.316326.xyz/gtzjebibfg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtrgcwoehf.html

Ruby: # 无泛型
来源：http://hz.yanxiufei.cn/gtlpawpbrm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gttuqvkvll.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtclbigldl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yonumen.top/gtidyfglkw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shangyingyoupin.top/gtsgmawqox.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtavaochlb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.meibo888.top/gtjonvavse.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gtwmduvwwi.html

Go:   // 无解构
来源：http://hz.cashguo.top/gtcvwlzlxt.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gtvqbebjom.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gtiawfofkb.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtsdxaquhf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.quarkkingdee.top/gttzvdqmcw.html

PHP:  // 无重载
来源：http://hz.hfpthk.cn/gtfwtubpfm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj20258888.top/gtgyvhbpnx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.316326.xyz/gtqzqpvgcl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtdhmgdkhs.html

Go:   // 无重载：用不同函数名
来源：http://hz.shangyingyoupin.top/gtkmsngflf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtizkcwjvg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenlongwang.top/gtfibpvsps.html

================================================================================
来源：http://hz.zhixingplan.top/gtftjjczjm.html

D. 数组 / 列表 / 集合
来源：http://hz.yangfankeji.com/gtqfutwktg.html

================================================================================
来源：http://hz.ybcxt.top/gtypoyfkfu.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtbbnuniaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtahhbilcg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ivvv.top/gtylgmamwp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gtkgwcvfwt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gtflyqatpe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.9152youxi.cn/gtbtjnycnl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.feifeiyinyue.top/gtooctcwas.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sweek.top/gtswlydomo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xinyue.icu/gtphlfexio.html

[D02] 追加元素到末尾
来源：http://hz.zhengqikj.top/gtikreoeqp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jiagoushi.top/gtioyxbobz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cqqwz.cn/gtmbiiwuwv.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gtjqhtxtlc.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtfgyftoyh.html

Java: list.add(4);
来源：http://hz.hongshengwenyu.top/gtwpporogw.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtomswehce.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258888.top/gtnsnxhrqs.html

C#:   list.Add(4);
来源：http://hz.ybcxt.top/gtqihwgycq.html

[D03] 在指定位置插入元素
来源：http://hz.tianlin.xyz/gtntbkhljm.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtpoeeztcs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtzzxygwiv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zycfv.cn/gtaaykkltu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtkctbihzt.html

Java: list.add(0, 0);
来源：http://hz.gzhubu.top/gtadnpihmp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhongyouzk.top/gtcytpnour.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhaomingkeji.xyz/gtkxkknwcl.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtywxnsawi.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtlwiokiqt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtwltegwwu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gttsrkyien.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gthcxompfg.html

TS:   arr.splice(0, 1);
来源：http://hz.feifeiyinyue.top/gtarqcymcb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhongyouzk.top/gtmrgtnmor.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtleyzsvic.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zycfv.cn/gtshxrkndk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.andypj.xyz/gtwdsdalfj.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gtunqkjfjf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.52xcode.cn/gtijmvuqzf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtxrimvknf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtruvkgbjd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.iojbl.cn/gtogbghcun.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtukkojrmw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtrnqiibto.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtgqkftvke.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuxming.cn/gtdlseabwe.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gtihhamtje.html

Py:   len(arr)
来源：http://hz.yj20258.top/gtxppcjonj.html

PHP:  count($arr);
来源：http://hz.cucudq.cn/gtkoivpxce.html

JS:   arr.length
来源：http://hz.chenlongwang.top/gtyviukger.html

TS:   arr.length
来源：http://hz.meibo888.top/gtkcpwsxen.html

Java: list.size();
来源：http://hz.andypj.xyz/gtdbjnpgul.html

Go:   len(arr)
来源：http://hz.nanxinkj.top/gthsinvync.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtcjoesmjp.html

C#:   list.Count;
来源：http://hz.andypj.xyz/gttevhnqbq.html

[D07] 切片 / 取子数组
来源：http://hz.smart0.xyz/gtanfouqpw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenjidiqi.icu/gtnmskxowa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fzhhl.top/gtcwaqzyqw.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtrjbrkied.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtugyakrta.html

Java: list.subList(1, 4);
来源：http://hz.ybcxt.top/gtcvolytvc.html

Go:   arr[1:4]
来源：http://hz.dashuyun.cn/gtwevbxdgo.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtcmvemndi.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gtsbahdruw.html

[D08] 合并两个数组
来源：http://hz.redwolf501.top/gtoyxfsihr.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtjsfplpdc.html

PHP:  array_merge($a, $b);
来源：http://hz.0kj1m.cn/gtzifyrrbe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtsvyzdcah.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtjsgibpyl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gtygqesczh.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtiprrdnpi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gtswxyrxwl.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhengqikj.top/gtbjiwjixi.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gtqvlrnctn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtcheezoph.html

PHP:  sort($arr);
来源：http://hz.tian-w.cn/gtbrkxfffr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fengsongda.top/gtmwfzhgbn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gtvpdcdpxp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtitapnzeo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtejrfprzm.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtsegubilz.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gtetaqnxeu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shzxlz.cn/gtimbaazmw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtirqtkmom.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtktfnztsy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtfocujrbp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtxhypfhwo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cucudq.cn/gtmwolpgtu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yongpay.top/gtucykctbj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgufenzy.top/gtzvxdacjo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtslnaitts.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtspliuoeh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gtcbgbbpct.html

PHP:  array_reverse($arr);
来源：http://hz.gzhubu.top/gtunuzajhz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gtiftftqbh.html

TS:   [...arr].reverse();
来源：http://hz.guannengcc.top/gtzyrqkvqj.html

Java: Collections.reverse(list);
来源：http://hz.birdmap.top/gtemealywk.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtllxvkllv.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtoxbmttuq.html

C#:   list.Reverse();
来源：http://hz.smart0.xyz/gthopdhotv.html

[D12] 查找元素下标
来源：http://hz.jinqigfzy.top/gtufpasqos.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgfzy.top/gtrhirszac.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtteqngglj.html


<!-- 参考信息 -->