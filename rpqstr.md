代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtlmcwdmrj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj202588.top/gtozgljwtk.html

[B11] 生成数字序列 / 区间
来源：http://hz.sweek.top/gteeycjkmp.html

Py:   list(range(0, 10, 2))
来源：http://hz.cashguo.top/gttvydmgry.html

PHP:  range(0, 10, 2);
来源：http://hz.hysaishi.cn/gtrkrwprwz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinyuanbaomall.cn/gtarjuhfqr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtpmecirvp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgfzy.top/gtommahuxq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gtnjvijxyz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinqigufen.top/gtocywkshe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zycfv.cn/gtafmbyokb.html

[B12] 跳出多层循环
来源：http://hz.gogol.net.cn/gtdwwotpps.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxinkj.top/gttroszslg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.smart0.xyz/gttpvxctgx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtrzswgolx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtjryhccbo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtlsqnakns.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.smart0.xyz/gtwjwrwkoa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shanyushiyangtech.top/gticmtdils.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nwbrower.top/gtiwxivbfz.html

[B13] 判断是否为数字
来源：http://hz.yonumen.top/gteujmbxda.html

Py:   isinstance(x, (int, float))
来源：http://hz.c1oappe.top/gtgcppgnhg.html

PHP:  is_numeric($x)
来源：http://hz.yj202588.top/gtbncarxei.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtlwykrxej.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangdashe.top/gtouevrqyi.html

Java: x instanceof Number
来源：http://hz.9152youxi.cn/gtiitunxxz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.birdmap.top/gtdazncgvw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.snrcjt.cn/gtljzhaeop.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gtdeqlwcvj.html

[B14] 判断值是否在集合内
来源：http://hz.sxryk.cn/gtgvibulgq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtitmlyzqm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yongpay.top/gtnacbnhow.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gtvhpbzhaj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jqgufenzy.top/gtajdlamyy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gotoacloud.top/gtebdzhfgj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sxryk.cn/gtghuwrqkl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yangfankeji.com/gtjcqbpdhz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gotoacloud.top/gtlnzwtopj.html

[B15] 布尔运算与取反
来源：http://hz.zhengqikj.top/gtbnqdzkjb.html

Py:   a and b or not c
来源：http://hz.jinqigfzy.top/gttjkqojvb.html

PHP:  $a && $b || !$c
来源：http://hz.fzhhl.top/gtpzkhqqkr.html

JS:   a && b || !c
来源：http://hz.hnqzz.top/gtoozwvowp.html

TS:   a && b || !c
来源：http://hz.gotoacloud.top/gtehksfupa.html

Java: a && b || !c
来源：http://hz.xziqi.cn/gtvbdmujgx.html

Go:   a && b || !c
来源：http://hz.birdmap.top/gtvmsthfpi.html

Ruby: a && b || !c
来源：http://hz.52xcode.cn/gtaguevnnc.html

C#:   a && b || !c
来源：http://hz.chenlongwang.top/gtakvavzer.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.andypj.xyz/gtvbdatinm.html

Py:   if not data: return
来源：http://hz.ydzc1.top/gtrhnuybee.html

PHP:  if (!$data) { return; }
来源：http://hz.pycfn.com/gtmupidluy.html

JS:   if (!data) return;
来源：http://hz.yonumen.top/gtobssunjt.html

TS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtoincxzwh.html

Java: if (data == null) return;
来源：http://hz.zhixingplan.top/gtxuuczrgs.html

Go:   if data == nil { return }
来源：http://hz.tianlin.xyz/gtpelobjtb.html

Ruby: return if data.nil?
来源：http://hz.hnqzz.top/gtkjeaetih.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtcjchmkji.html

================================================================================
来源：http://hz.nanxinkj.top/gtdufbmlsn.html

C. 函数与作用域
来源：http://hz.chenlongwang.top/gthdmnfaqp.html

================================================================================
来源：http://hz.zhengqikj.top/gtqgtonkou.html

[C01] 定义函数
来源：http://hz.ivvv.top/gtbscfuysc.html

Py:   def add(a, b): return a + b
来源：http://hz.cashguo.top/gtbmrjmdks.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gthvybamvq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtgnadrknj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gthblrypng.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtwrkzjbcy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtbepqvwpx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ywan-chungtsiang.top/gtjfnunqew.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtqjmjjivr.html

[C02] 默认参数
来源：http://hz.ydjk.org.cn/gtgzumuuhb.html

Py:   def greet(name="World"): return name
来源：http://hz.yanxiufei.cn/gtpsepbnhh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtyrfkvvzp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yonumen.top/gtqbhvwyvx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtainjkbfb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuetiantiany.cn/gtkdsahaqf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cashguo.top/gtqxupksyg.html

Ruby: def greet(name = "World") = name
来源：http://hz.redwolf501.top/gtrrdyvwwj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtikwknbsd.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtvqhsrduw.html

Py:   def total(*args): return sum(args)
来源：http://hz.yueranfly.top/gtvwhuoqpt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtyctbynaf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtgiukrvfd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gtbdiccuur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuxming.cn/gtjilkeqws.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tianlin.xyz/gtnvewohaj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ehwqpu.com/gtxzvtgaqr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtfirmnfvh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtuxmenach.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hongshengwenyu.top/gtunqhvxct.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zdqjudy.top/gtlpylcshy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtezqhqerk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gttrasrvjq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.9152youxi.cn/gtvnoqgqfq.html

Go:   // 无：用配置结构体参数
来源：http://hz.daxiang520.top/gtykmwvnji.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtwlgqsoim.html

C#:   f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtolslxdhj.html

[C05] 返回多个值
来源：http://hz.jinyuanbaomall.cn/gtzvzhrqkj.html

Py:   return a, b
来源：http://hz.birdmap.top/gtogbmzlhu.html

PHP:  return [$a, $b];
来源：http://hz.zhixingplan.top/gthrldqxcs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.c1oappe.top/gtlshqpaiw.html

TS:   return { a, b };
来源：http://hz.zhixingplan.top/gtklbkxqvc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.mhx1999.top/gtokuitaum.html

Go:   return a, b
来源：http://hz.yj202588.top/gtqtgbecfy.html

Ruby: return a, b
来源：http://hz.fengsongda.top/gteselioxl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gthmmjqxwv.html

[C06] 匿名函数 / lambda
来源：http://hz.316326.xyz/gthabwnjfi.html

Py:   square = lambda x: x * x
来源：http://hz.nanxuanxn.top/gtlyipugsn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tianlin.xyz/gtnvlxqhfl.html

JS:   const square = x => x * x;
来源：http://hz.mhx1999.top/gtegmurqfb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hfpthk.cn/gtneaqqvrw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hongshengwenyu.top/gtipwfoypl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuxming.cn/gtcuftgllv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigfzy.top/gtypmgmriz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.meibo888.top/gtigqmwyob.html

[C07] 把函数作为参数传入
来源：http://hz.ybcxt.top/gtegilawsq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gaohongyu789.top/gtvllbdmpz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gogol.net.cn/gttnumabqs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtulckplbj.html

TS:   arr.map(String)
来源：http://hz.birdmap.top/gtidmtljsp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gotoacloud.top/gtithqaebh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pycfn.com/gtpftmegjr.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gthgeumipp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nanxuanxn.top/gtxyvrlrzc.html

[C08] 闭包
来源：http://hz.yj20258.top/gtmfmutggf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtuxlrigjg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhoulong.xyz/gtkziduful.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtshivatmg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtfvonhbih.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.iojbl.cn/gtdwmycmxv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtjrxacyxk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinqigufen.top/gtqtfdclwu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtfxgwshox.html

[C09] 递归
来源：http://hz.jianghu66.top/gtcsinekbo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.birdmap.top/gthwsldqlm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gttxxpfskw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtzubtzrrm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtvquxmngt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gtuaxctriw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sxryk.cn/gtmiykqclw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtirxovrpt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zycfv.cn/gtymdtbycf.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtbrtkrapn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yonumen.top/gtvvsvuvwq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gzhubu.top/gtbmhdzait.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtzwwnumsx.html

TS:   同 JS
来源：http://hz.redwolf501.top/gtuzcseagi.html

Java: 方法内为块级作用域
来源：http://hz.zhongyouzk.top/gtxpuzkwfh.html

Go:   花括号块级作用域
来源：http://hz.zycfv.cn/gtuhyjhaxu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.snrcjt.cn/gtjgvwvqms.html

C#:   块级作用域
来源：http://hz.ybcxt.top/gtyyyglalk.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtgwuywcwu.html

Py:   from module import func
来源：http://hz.guowangkeji.top/gtwgxlfuxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtrnyvmyae.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtkvbzlmxw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jianghu66.top/gtacusicdb.html

Java: import java.util.List;
来源：http://hz.ybcxt.top/gtrpvkzajo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xingfuxueyuan.xyz/gtyvdjngcp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gteuemnhiq.html

C#:   using System.Text;
来源：http://hz.yj202588.top/gtefiqpvpo.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenlongwang.top/gtztzldehz.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gtgfwagnjx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.bjfxy.top/gtibpzudaj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtxblvnlsp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtnkkmmmcb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ybcxt.top/gtkcclvaai.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gteqlijcuj.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxinkj.top/gtqhxrowvi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.quarkkingdee.top/gtvpfgmhlw.html

[C13] 类型声明 / 类型注解
来源：http://hz.snrcjt.cn/gtlazicvno.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtgizfhozr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtocvkijav.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtejmtggex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtjktuhupl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtxxrvijrm.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtstnnhvkp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtyrawjyxx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtxqvwmdtc.html

[C14] 泛型函数
来源：http://hz.ivvv.top/gtcgakqtac.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtkpixxvkx.html

PHP:  // 无泛型
来源：http://hz.guannengcc.top/gtaadviqvc.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtfhylwngi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgufenzy.top/gtbbwpvbyc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ywan-chungtsiang.top/gtntylqmgm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtckuyqjom.html

Ruby: # 无泛型
来源：http://hz.xylfe.cn/gtybufkfrs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cdnleiting.top/gtnzvujzad.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtsolsvphj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gtvdlqedlm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gttpmgronb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gttlrjsvub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtchvztnem.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtpmhywizc.html

Go:   // 无解构
来源：http://hz.zhaomingkeji.xyz/gtyirthpuo.html

Ruby: a, b = pair
来源：http://hz.0kj1m.cn/gtsuikloqw.html

C#:   var (a, b) = pair;
来源：http://hz.cheryme.top/gtjtkbtmtx.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtdgsnonuw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtlxebrcuc.html

PHP:  // 无重载
来源：http://hz.havefunace.top/gtsbbkwqty.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuetiantiany.cn/gtupmabhzl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cheryme.top/gtvwsitcbs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtsuwosgae.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhoulong.xyz/gtrqkuhtqw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fzhhl.top/gtoqqztjmg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtmnxusuvv.html

================================================================================
来源：http://hz.cdnleiting.top/gtuvqbcxwd.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtnlikvdyn.html

================================================================================
来源：http://hz.ppjwa.cn/gtmguspiwu.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtbumbzzgw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gogol.net.cn/gtpuzqbapo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gtgjkmiipz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtguenfqrd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtrxqqbzgi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aibaodan.cn/gtnshpljsf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtdoxaaxhv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtmrvrmvrk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zycfv.cn/gtveyonrel.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtsxrhgaqq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtuflueizb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuetiantiany.cn/gtclfmzzso.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtlqadksyw.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtzqprbqmn.html

Java: list.add(4);
来源：http://hz.zycfv.cn/gtsgjdjfue.html

Go:   arr = append(arr, 4)
来源：http://hz.tanke756.top/gteunwsqef.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtirmyprto.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtoylnzvmm.html

[D03] 在指定位置插入元素
来源：http://hz.sweek.top/gtslfepskm.html

Py:   arr.insert(0, 0)
来源：http://hz.c1oappe.top/gtotucleyb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gthlhkhllo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gthvualjau.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtciwvzdem.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtebpphjou.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xziqi.cn/gtetrnlcmi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.meibo888.top/gtkdammwyp.html

C#:   list.Insert(0, 0);
来源：http://hz.jyoumei.cn/gtzmvaddkl.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gttoxqeygk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhaomingkeji.xyz/gtgccxhgcp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtfabnhgcn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.c1oappe.top/gtxqjmvxzs.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtawqrmprz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hfpthk.cn/gtzsupuzfj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.bjfxy.top/gtvnvfmgmv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guowangkeji.top/gtjnxnwmrt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtnqyzdfjj.html

[D05] 访问与修改元素
来源：http://hz.jyoumei.cn/gtrkhxfxca.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtlmyajuul.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangdashe.top/gtiwblrrvq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtamnkmhqd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.vqdsnc.cn/gtrvadypyo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtpeymfule.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtyqgruslx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gttawgfpvv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cdnleiting.top/gtatmyoppf.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtdoykuzwi.html

Py:   len(arr)
来源：http://hz.ehwqpu.com/gtfzyddtqs.html

PHP:  count($arr);
来源：http://hz.tian-w.cn/gtrkaistqg.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtijdvkrij.html

TS:   arr.length
来源：http://hz.gotoacloud.top/gtcnndtpiy.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gttemdstad.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gtksctyjtg.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gthdbyuara.html

C#:   list.Count;
来源：http://hz.feifeiyinyue.top/gtrmivlpft.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtygzefdxy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gthrppczhn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guannengcc.top/gtttrbyyyu.html

JS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtsbdpdnar.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtmwizfqud.html

Java: list.subList(1, 4);
来源：http://hz.kuanghao11.cn/gtzesvoebf.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtlohexjyo.html

Ruby: arr[1, 3]
来源：http://hz.smart0.xyz/gtuddjeghy.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinyuanbaomall.cn/gtcmxtzhql.html

[D08] 合并两个数组
来源：http://hz.shuidangran.top/gtrrwcduvi.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtdpkgvikh.html

PHP:  array_merge($a, $b);
来源：http://hz.ppjwa.cn/gteaermglv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtiadqioah.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gtsquqwovn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtilgsezxb.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtjbymbkjz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fengsongda.top/gtflepstep.html

C#:   a.Concat(b).ToList()
来源：http://hz.sweek.top/gtlwnahbjd.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gthcwfdfax.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtgopqxpzz.html

PHP:  sort($arr);
来源：http://hz.jinqigufen.top/gtowlukvmt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daxiang520.top/gtogwobhvu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtqoftteie.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtyboxssvj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtfeqsslyb.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gthxjwdqcq.html

C#:   list.Sort();
来源：http://hz.sufxvd.cn/gtmhviyvjy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gtthbkbire.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ywan-chungtsiang.top/gtuhexfclw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtghwumwes.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtjctyscsg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtbefdsnll.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gtrmeofcbg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shzxlz.cn/gtewnktaqk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtvkwpgqoc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtrvekqphr.html

[D11] 反转数组
来源：http://hz.ydjk.org.cn/gtrguvqyem.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sweek.top/gtnzksllkd.html

PHP:  array_reverse($arr);
来源：http://hz.ydzc1.top/gtxjuevtrj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yongpay.top/gtkpwgltwt.html


<!-- 参考信息 -->