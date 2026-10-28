代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhengqikj.top/gtqgjmxbgd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhijiandao.cn/gtunskuygn.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj20258888.top/gtonxyewbk.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtqjkwrvku.html

PHP:  range(0, 10, 2);
来源：http://hz.tianlin.xyz/gtafonmkzv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.kuanghao11.cn/gtksuybhbb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtjmprgvqb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ywan-chungtsiang.top/gthuzopuqx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtmorhvsmc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zdqjudy.top/gtqctgvgzi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.mhx1999.top/gtmazuvxmu.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangkeji.top/gtuvmbesoj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinqigufen.top/gteunqnizx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj202588.top/gtoatxctga.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtjsmsxefd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtsfqwhnoh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtfwsjvunm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.mhx1999.top/gtzozpitzl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinghuilouyu.cn/gteeutttfn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.9152youxi.cn/gtsacthzjh.html

[B13] 判断是否为数字
来源：http://hz.cheryme.top/gtxpfkgphp.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtxjyblsqc.html

PHP:  is_numeric($x)
来源：http://hz.ehwqpu.com/gtqrthkjzg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtygpumsyc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gttxzrplho.html

Java: x instanceof Number
来源：http://hz.316326.xyz/gtdzjhnvhv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xylfe.cn/gtnhneiffu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgufenzy.top/gtbyvoxkvl.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gtmfmjuzhg.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtzdddgkwj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuetiantiany.cn/gtksbjhuxp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtcaiculbl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtakckgqba.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtfgyswfda.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtxkycktby.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxinkj.top/gtvfypszsp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhoulong.xyz/gtnttqowej.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tian-w.cn/gtdpjprkhv.html

[B15] 布尔运算与取反
来源：http://hz.ywan-chungtsiang.top/gtxevdblly.html

Py:   a and b or not c
来源：http://hz.52xcode.cn/gtvdclwdrs.html

PHP:  $a && $b || !$c
来源：http://hz.hongshengwenyu.top/gtypwleqce.html

JS:   a && b || !c
来源：http://hz.redwolf501.top/gtfwebhbig.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtisqpbznj.html

Java: a && b || !c
来源：http://hz.hywenlv.cn/gtcyhcwigz.html

Go:   a && b || !c
来源：http://hz.gogol.net.cn/gtcwfjbhdq.html

Ruby: a && b || !c
来源：http://hz.quarkkingdee.top/gthypcfbmr.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gtcvxgafav.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xuetiantiany.cn/gtoaabqwde.html

Py:   if not data: return
来源：http://hz.0kj1m.cn/gtkhwlltah.html

PHP:  if (!$data) { return; }
来源：http://hz.tian-w.cn/gtqfowoqao.html

JS:   if (!data) return;
来源：http://hz.tian-w.cn/gtrhvxrali.html

TS:   if (!data) return;
来源：http://hz.xinyue.icu/gtaitqpvxb.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gtfuekzirw.html

Go:   if data == nil { return }
来源：http://hz.daria6918.cn/gtbmocwcmp.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gtsmvovidb.html

C#:   if (data == null) return;
来源：http://hz.zhixingplan.top/gtnccupndq.html

================================================================================
来源：http://hz.haohaochexian.top/gtwducqbif.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtcdbexkov.html

================================================================================
来源：http://hz.haohaochexian.top/gtooejzrzh.html

[C01] 定义函数
来源：http://hz.andypj.xyz/gteiwuipoc.html

Py:   def add(a, b): return a + b
来源：http://hz.52xcode.cn/gtjakxkcya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtuidrcnop.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yvedp.cn/gtllnuxadp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtsnjbofcu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtnbvimodx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.bjfxy.top/gtmquqtbmg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuxming.cn/gtuvhuntxd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtdgkjifmr.html

[C02] 默认参数
来源：http://hz.yanxiufei.cn/gtnvhmthgf.html

Py:   def greet(name="World"): return name
来源：http://hz.yj202588.top/gtkartkpto.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xziqi.cn/gtytfkuwyz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yueranfly.top/gtkpucvggv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtphvrmabx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dianchejie.cn/gtfrjimcho.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shangyingyoupin.top/gtpkjusdsg.html

Ruby: def greet(name = "World") = name
来源：http://hz.birdmap.top/gttfdbhxxp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258.top/gtbvsmbimu.html

[C03] 可变参数
来源：http://hz.nanxinkj.top/gtzjrlsywy.html

Py:   def total(*args): return sum(args)
来源：http://hz.dianchejie.cn/gtdqhelvld.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fzhhl.top/gtyjkrslqr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtzqepkdsn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtazpffzfy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jlsjyb.cn/gtsutsbhiv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinghuilouyu.cn/gtavxpeyqi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinghuilouyu.cn/gtcowczekr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtetmoirsa.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinyuanbaomall.cn/gtgcwkrfsp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtyxpfkbrw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sweek.top/gtjhpzdpqc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gthpunpsvx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtedgyshqp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtkjkuktwz.html

Go:   // 无：用配置结构体参数
来源：http://hz.haohaochexian.top/gthgvwbmbk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtxbuhpzzu.html

C#:   f(a: 1, b: 2)
来源：http://hz.xingfuxueyuan.xyz/gtvlktuciv.html

[C05] 返回多个值
来源：http://hz.tianlin.xyz/gthxprjeqa.html

Py:   return a, b
来源：http://hz.feifeiyinyue.top/gtfzvxqvee.html

PHP:  return [$a, $b];
来源：http://hz.yongpay.top/gtkrgcqwzn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinqigufen.top/gtcttrfgyb.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtotwzzugh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuxming.cn/gtctvjafwo.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtehvswedf.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtgidqkufw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtjkwjjngf.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtpeoappgd.html

Py:   square = lambda x: x * x
来源：http://hz.chenlongwang.top/gtxhmgqmtr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sysykeji.top/gtdodlitrf.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gtgtjsysmc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gttvypajgi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xinyue.icu/gtckakwihx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jianghu66.top/gtdrxvxvck.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhengqikj.top/gtipedgmxd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.0kj1m.cn/gtvtsreyeh.html

[C07] 把函数作为参数传入
来源：http://hz.aizwys.cn/gtiqufwdis.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yongpay.top/gtffoaizae.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ywan-chungtsiang.top/gtrnmwgowq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtsilnjanz.html

TS:   arr.map(String)
来源：http://hz.feifeiyinyue.top/gtywwsltts.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtptqkbtck.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xinyue.icu/gtdbwowbbr.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gtvhnpmnko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cucudq.cn/gtrokgcjde.html

[C08] 闭包
来源：http://hz.svipenyu.cn/gtfdgpvopa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nwbrower.top/gtcfamcxxi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ppjwa.cn/gtpyzeywga.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtqgefditw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtzlpgqbxn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxinkj.top/gtjbmhqzky.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sysykeji.top/gtxjcpxqoh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gaohongyu789.top/gtlnknokmx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtptfngkme.html

[C09] 递归
来源：http://hz.guannengcc.top/gtkginwxhd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sxryk.cn/gtshempitg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuetiantiany.cn/gtcdyfvhyn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtnrcljlfa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtqsimanws.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shangyingyoupin.top/gtzfjnwinl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gotoacloud.top/gtlnyjnygs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtxodbjvua.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fzhhl.top/gtptescglk.html

[C10] 变量作用域
来源：http://hz.hysaishi.cn/gtnbjwhaas.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangtech.top/gtehezlzhp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pengpengdd.cyou/gtwercdumd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnxiangtu.top/gtufboiwsf.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtyajdzvxx.html

Java: 方法内为块级作用域
来源：http://hz.andypj.xyz/gtfrudlghb.html

Go:   花括号块级作用域
来源：http://hz.nanxuanxn.top/gtrphqylcw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ywan-chungtsiang.top/gtofshbyng.html

C#:   块级作用域
来源：http://hz.redwolf501.top/gtcczasbfg.html

[C11] 模块导入与导出
来源：http://hz.tian-w.cn/gtnxzguymm.html

Py:   from module import func
来源：http://hz.fengsongda.top/gtlrnvgytf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtteeqiofy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aibaodan.cn/gtrieqwmpn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtiyyvzwrh.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtcpwvttsf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtnutlvbyl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gogol.net.cn/gtzkmllmhc.html

C#:   using System.Text;
来源：http://hz.snrcjt.cn/gtdjasgaie.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhiwuduotai.top/gtbhbbsrve.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gtjcfygzxl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtgeyzdnla.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtsodaaerj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gthimnbmbp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gtywrcgrsi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtmembxohu.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtpeixainq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigfzy.top/gtrnxaxrjp.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtgpxynniq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gturssyroq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtrhtqxxoq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guannengcc.top/gtdhtselbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtsnwcktwe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtopsnoqhz.html

Go:   func add(a, b int) int
来源：http://hz.gzhubu.top/gtoudxtgbq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.iojbl.cn/gtumbbwlup.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gtjvcabbkc.html

[C14] 泛型函数
来源：http://hz.zhongyouzk.top/gtxyldlokf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtgifblyma.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtwkbiwjts.html

JS:   // 无泛型
来源：http://hz.ppjwa.cn/gthvxbiimf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtdcyjdmbg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtjxtvxmkl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtrssskjuk.html

Ruby: # 无泛型
来源：http://hz.zdqjudy.top/gtzmxokqks.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxinkj.top/gtjlpckxnz.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtbxrlwzkt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtrhfwzvaz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtscusjyki.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangkeji.top/gtkxmilaak.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sufxvd.cn/gtpyurznzm.html

Java: // 无解构
来源：http://hz.shzxlz.cn/gtfwfwqmho.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtmkcngsme.html

Ruby: a, b = pair
来源：http://hz.vqdsnc.cn/gtfsquuemj.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gtvcxogymn.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtsppmgdtk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.smart0.xyz/gtcszjywei.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtebumbywx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtamcfokdj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cucudq.cn/gteidnwapc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinghuilouyu.cn/gtlqyyblux.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydjk.org.cn/gtkbbkgmap.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sufxvd.cn/gtkvjjrrgx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aizwys.cn/gtizjmpbgt.html

================================================================================
来源：http://hz.cdnleiting.top/gtomvxtdcy.html

D. 数组 / 列表 / 集合
来源：http://hz.ivvv.top/gtnytejprp.html

================================================================================
来源：http://hz.sufxvd.cn/gtteozzyrw.html

[D01] 创建数组 / 列表
来源：http://hz.zdqjudy.top/gtdcbnnhll.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.haohaochexian.top/gtmgjcgfna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtrwdaduge.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.feifeiyinyue.top/gtfqvqyiwx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangtech.top/gtvuwbivvu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sweek.top/gtqkfgzitl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hammf.cn/gtemdyzfgz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ywan-chungtsiang.top/gtrxywrvqa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gtkvhmqxjb.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtkeqgveqi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtwepumirt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtfdjfwbqq.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtpkhzxzat.html

TS:   arr.push(4);
来源：http://hz.c1oappe.top/gtrsaiefyw.html

Java: list.add(4);
来源：http://hz.yangfankeji.com/gtfnkhjctn.html

Go:   arr = append(arr, 4)
来源：http://hz.jlsjyb.cn/gtkaujrzbv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.wangshuangyany.cn/gtjbvcmcwf.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gtiwgwwkin.html

[D03] 在指定位置插入元素
来源：http://hz.nwbrower.top/gtnxhiuqsv.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gtygqfztit.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.c1oappe.top/gtvwpsbity.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtzweywyhl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtovngpadt.html

Java: list.add(0, 0);
来源：http://hz.shangyingyoupin.top/gtxezmyhpw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gttkeqebrg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cqqwz.cn/gtijayyiiy.html

C#:   list.Insert(0, 0);
来源：http://hz.pengpengdd.cyou/gtpxxjgbix.html

[D04] 删除元素
来源：http://hz.kuanghao11.cn/gtpnqptufl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtukeztsxi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtzhuzlfrr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtkxkuahhs.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtconrfziu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtuiwduzgb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtswhhtdpo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cheryme.top/gtfqcuthak.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtmtknwjwv.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtlcyajcsa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gttelsegih.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gtizzqqvxi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.redwolf501.top/gtkbgoywmz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtowaqkcot.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gaohongyu789.top/gtuharbqny.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtyjgjtinc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtgfaohxpw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gtjnrtyrzq.html

[D06] 数组长度
来源：http://hz.chenjidiqi.icu/gtlpgianvz.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtapzmnugp.html

PHP:  count($arr);
来源：http://hz.yj20258.top/gtzsghapkq.html

JS:   arr.length
来源：http://hz.cdnleiting.top/gtoyywzqtj.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtrvlgsevk.html

Java: list.size();
来源：http://hz.nanxuanxn.top/gtggixmwnm.html

Go:   len(arr)
来源：http://hz.snrcjt.cn/gtlpvwvxgn.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtuvcwoojr.html

C#:   list.Count;
来源：http://hz.yangfankeji.com/gtzqtpczbb.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gtpqbfznyi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtvcsodxlf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenjidiqi.icu/gtwksofzvx.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtylbgcypx.html

TS:   arr.slice(1, 4);
来源：http://hz.daxiang520.top/gtjscqcowm.html

Java: list.subList(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtjosmkhrq.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtuleehqjz.html

Ruby: arr[1, 3]
来源：http://hz.xuanzx.com/gtxpvqhiai.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gtqzemarqa.html

[D08] 合并两个数组
来源：http://hz.jinqigfzy.top/gtgflmpfoc.html

Py:   a + b;  a.extend(b)
来源：http://hz.dianchejie.cn/gtbzjxzcne.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258888.top/gttcmoufwn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangtech.top/gthiyvwcvd.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtpoypqmou.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtjlagmqux.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtgdzhzezv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhengqikj.top/gtaiaqeppm.html

C#:   a.Concat(b).ToList()
来源：http://hz.jlsjyb.cn/gtbvmqdczf.html

[D09] 排序（升序）
来源：http://hz.aibaodan.cn/gtbljyjysb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gtbwsjesmp.html

PHP:  sort($arr);
来源：http://hz.chenlongwang.top/gtsegdnrvx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.9152youxi.cn/gttwvwdjpo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yangfankeji.com/gtajhxhoup.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtgehmnmkp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtomoteytp.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtcfkbjzka.html

C#:   list.Sort();
来源：http://hz.meibo888.top/gtrvvseviw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgfzy.top/gtkvuwgohh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtofzqnxjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gttfibajaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtozkpwfjp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtkndvvqfn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gttzlcknve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtifrkgloa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gtgqtwehrz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gtrmpgtnuu.html

[D11] 反转数组
来源：http://hz.hywenlv.cn/gtczphkpmf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fengsongda.top/gtefxrgbbl.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtelhrbbuy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtygondwpn.html


<!-- 参考信息 -->