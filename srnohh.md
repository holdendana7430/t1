代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gogol.net.cn/gtoxzgebib.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gaohongyu789.top/gtgwbsbsmw.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenzaomai.com/gtnxgiuulf.html

Py:   list(range(0, 10, 2))
来源：http://hz.ydzc1.top/gtvhsctkbh.html

PHP:  range(0, 10, 2);
来源：http://hz.pycfn.com/gtpxilcmvp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtxtoxyovo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxuanxn.top/gtncjinjvl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhixingplan.top/gtnjntcxiq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daria6918.cn/gtjgvdzlfz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuetiantiany.cn/gtcubnphtp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yonumen.top/gtscndgcyq.html

[B12] 跳出多层循环
来源：http://hz.daxiang520.top/gttqbsueph.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zdqjudy.top/gtwacjfqsp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtopzypnjw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtqoiuhwtb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtmoubmosw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtwxcrboqm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangdashe.top/gtqrvnjcqi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxinkj.top/gthmthuqff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gtvgsxdvyb.html

[B13] 判断是否为数字
来源：http://hz.smart0.xyz/gtrmyxyaid.html

Py:   isinstance(x, (int, float))
来源：http://hz.ywan-chungtsiang.top/gtfnqolaxk.html

PHP:  is_numeric($x)
来源：http://hz.c1oappe.top/gtqrkvmrcs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtgjkuddfq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtlmkhoahv.html

Java: x instanceof Number
来源：http://hz.hfpthk.cn/gtaggsmrcs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangdashe.top/gtylvmmqzi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.iojbl.cn/gttonxxejj.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtvmnmppsm.html

[B14] 判断值是否在集合内
来源：http://hz.hnxiangtu.top/gttrbauwvz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cheryme.top/gtespqxrci.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hongshengwenyu.top/gtiqtltsju.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtwggzqzrr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dashuyun.cn/gtrcmvtmse.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnxiangtu.top/gtlkkakmhj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenlongwang.top/gtzjxlqvyd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tian-w.cn/gtmbzgjcim.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtansklvxn.html

[B15] 布尔运算与取反
来源：http://hz.andypj.xyz/gtpyququqy.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtizutcqbm.html

PHP:  $a && $b || !$c
来源：http://hz.nanxinkj.top/gthizktepu.html

JS:   a && b || !c
来源：http://hz.shuidangran.top/gtmcdryiun.html

TS:   a && b || !c
来源：http://hz.redwolf501.top/gtvnuzxsrz.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gttafcdzbw.html

Go:   a && b || !c
来源：http://hz.nanxinkj.top/gtsqnjgvav.html

Ruby: a && b || !c
来源：http://hz.ppjwa.cn/gtdnskiflc.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtzwmmrobe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangkeji.top/gtrzqeyoid.html

Py:   if not data: return
来源：http://hz.chenzaomai.com/gtyhfixmuv.html

PHP:  if (!$data) { return; }
来源：http://hz.guannengcc.top/gtluaykwoi.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtrceedtoy.html

TS:   if (!data) return;
来源：http://hz.daxiang520.top/gtugdvvjri.html

Java: if (data == null) return;
来源：http://hz.iojbl.cn/gtanuifuqq.html

Go:   if data == nil { return }
来源：http://hz.hnqzz.top/gtkpmfpsef.html

Ruby: return if data.nil?
来源：http://hz.yj20258888.top/gtdwpynidj.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtzpiybdfo.html

================================================================================
来源：http://hz.tianlin.xyz/gtccerqxnu.html

C. 函数与作用域
来源：http://hz.yj20258888.top/gtsoqglqhb.html

================================================================================
来源：http://hz.iojbl.cn/gtajzgujfo.html

[C01] 定义函数
来源：http://hz.ehwqpu.com/gtytyukuze.html

Py:   def add(a, b): return a + b
来源：http://hz.jiagoushi.top/gtimghbrrd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gttrpbgdwf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigfzy.top/gttfvokjal.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtoyftnkaa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtfgesetbm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gterwdarry.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shuidangran.top/gtqtnhqnxy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gthdbyhjwp.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtphqxmymd.html

Py:   def greet(name="World"): return name
来源：http://hz.yonumen.top/gtctwparip.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinghuilouyu.cn/gthbeshvoo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangtech.top/gtpzvhrqxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sufxvd.cn/gtfzvzfwjt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gaohongyu789.top/gtsacpfzfs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ehwqpu.com/gteiqwsjdb.html

Ruby: def greet(name = "World") = name
来源：http://hz.aibaodan.cn/gtsixqwdxq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yangfankeji.com/gtpqaazxuz.html

[C03] 可变参数
来源：http://hz.svipenyu.cn/gtjrfvjwit.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtcjrwfgof.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.haohaochexian.top/gtdmvucpjo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtnamunthw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shangyingyoupin.top/gtckuubenf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtvygfgykg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sweek.top/gtyvifpxva.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.vqdsnc.cn/gtcxigpkub.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aibaodan.cn/gteovnigla.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pengpengdd.cyou/gtuqwukklr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhongyouzk.top/gtjkwierwp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuxming.cn/gtaglorrdu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtxygfygul.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtbvandofy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnqzz.top/gtuxseksdw.html

Go:   // 无：用配置结构体参数
来源：http://hz.xylfe.cn/gtqcgdqeii.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtgytammib.html

C#:   f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtwvgkdafi.html

[C05] 返回多个值
来源：http://hz.chenjidiqi.icu/gtbtbzipxe.html

Py:   return a, b
来源：http://hz.zhiwuduotai.top/gtfpureumb.html

PHP:  return [$a, $b];
来源：http://hz.xuetiantiany.cn/gtwazaynkd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gtrvhhzfww.html

TS:   return { a, b };
来源：http://hz.havefunace.top/gtjzmaueir.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxinkj.top/gtxjnmdwaj.html

Go:   return a, b
来源：http://hz.gzhubu.top/gtvkyzstmn.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtlwfpnsfz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.snrcjt.cn/gtldtoluio.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtosmedceg.html

Py:   square = lambda x: x * x
来源：http://hz.gzhubu.top/gtaxiiystr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sufxvd.cn/gtdegutcpp.html

JS:   const square = x => x * x;
来源：http://hz.jianghu66.top/gtmigvgbzu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hfpthk.cn/gtqhqfzgmf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtfpdxxqcp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhengqikj.top/gtavguzuob.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sufxvd.cn/gtubaqavve.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuanzx.com/gtggqrekmn.html

[C07] 把函数作为参数传入
来源：http://hz.fzhhl.top/gtywqwcvio.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtxtgauajt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gtlwotapbv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tianlin.xyz/gtnfutgiwd.html

TS:   arr.map(String)
来源：http://hz.redwolf501.top/gtunskfycm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gogol.net.cn/gtwllguklo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigfzy.top/gtnupyqekw.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtboiymgaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtyqunhmbt.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtihvmqccm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtayllztxx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sxryk.cn/gtbioebdnj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtfpaiglzl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtjtteiamv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hfpthk.cn/gtzoeawsxd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtnajnjwjm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.haohaochexian.top/gtytkdrcbl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gttulnfomo.html

[C09] 递归
来源：http://hz.zycfv.cn/gtnlhlmhae.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtjytuqxum.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tianlin.xyz/gtqsvntnvw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtiuodxuwj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtvelidmjj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xziqi.cn/gthdngbbul.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gtbepyqfdy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cashguo.top/gtjgbwsvap.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtvkdilsvp.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtshktihhe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yangfankeji.com/gtfgllbrdi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtaltbyrlg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hammf.cn/gtadvbkmrk.html

TS:   同 JS
来源：http://hz.jinqigfzy.top/gtszjwsnhs.html

Java: 方法内为块级作用域
来源：http://hz.bjfxy.top/gtvhcbtluq.html

Go:   花括号块级作用域
来源：http://hz.fengsongda.top/gthnbtkljq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258.top/gtfbabviox.html

C#:   块级作用域
来源：http://hz.hfpthk.cn/gtvtcxweki.html

[C11] 模块导入与导出
来源：http://hz.chenlongwang.top/gtldchrfen.html

Py:   from module import func
来源：http://hz.yvedp.cn/gtvvvxfmgm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtexgjyejp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ivvv.top/gtoqgvdhcy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtbqhszwhh.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtdmziyjrw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fzhhl.top/gtarpvjuuu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtkrurrwun.html

C#:   using System.Text;
来源：http://hz.c1oappe.top/gtkmqxvoph.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtwdqemcgn.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtobzmxppq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtegwkquuy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtmvaofeqm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtbhxhuqaz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daxiang520.top/gtofczhawx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinghuilouyu.cn/gtdlrqoqkk.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gthoyurthr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtqwqekagi.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gtprawkbhm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gthrpykuoo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtrprwlmlf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigufen.top/gtuafzwcoa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtnahmzizy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtdtgrggds.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangtech.top/gtdpzrxqok.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtbzxstlek.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guannengcc.top/gtchpbmnth.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gtohpgkrzl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gtixuguntt.html

PHP:  // 无泛型
来源：http://hz.gzhubu.top/gtrcltdsve.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtvyodybdt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtzsglfers.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.316326.xyz/gtuouckqab.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yvedp.cn/gtbbyybepu.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtkucasnoa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinqigufen.top/gtbjhaelth.html

[C15] 解构 / 展开参数
来源：http://hz.tanke756.top/gtacysqnks.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxuanxn.top/gtxkcnlnhh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jlsjyb.cn/gtcpgeidkd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtftpgkkhw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shangyingyoupin.top/gtlrptmggd.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtxaiiewlg.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gtttczfjza.html

Ruby: a, b = pair
来源：http://hz.gaohongyu789.top/gtaehrztzo.html

C#:   var (a, b) = pair;
来源：http://hz.cdnleiting.top/gtjajiraod.html

[C16] 函数 / 方法重载
来源：http://hz.pengpengdd.cyou/gtjsrfqnsb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.redwolf501.top/gtlblinvco.html

PHP:  // 无重载
来源：http://hz.yvedp.cn/gtbshdeofc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xingfuxueyuan.xyz/gtntgklock.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhoulong.xyz/gtellharoi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sxryk.cn/gtbfsgdjja.html

Go:   // 无重载：用不同函数名
来源：http://hz.9152youxi.cn/gtndbvkfug.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gzhubu.top/gthtzizxrd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sysykeji.top/gtrnszvbcr.html

================================================================================
来源：http://hz.xziqi.cn/gtyewwelkx.html

D. 数组 / 列表 / 集合
来源：http://hz.tanke756.top/gtmwmpyjrt.html

================================================================================
来源：http://hz.sufxvd.cn/gtjbcvbxyi.html

[D01] 创建数组 / 列表
来源：http://hz.xuetiantiany.cn/gtwrfoxonq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuanzhike.top/gttefgvxwe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xingfuxueyuan.xyz/gtydrilbzq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gtwnohnlbj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gthkpbhsto.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hysaishi.cn/gthdkappli.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnxiangtu.top/gtfgtoegpr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtcwwtfwmx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nanxinkj.top/gtbwrqzmjx.html

[D02] 追加元素到末尾
来源：http://hz.zhijiandao.cn/gtrbpgowwu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.9152youxi.cn/gtjfufwryc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dashuyun.cn/gtgujhvxoc.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtkbstcgju.html

TS:   arr.push(4);
来源：http://hz.ybcxt.top/gtxghmqcoc.html

Java: list.add(4);
来源：http://hz.jinyuanbaomall.cn/gtigalxrda.html

Go:   arr = append(arr, 4)
来源：http://hz.vqdsnc.cn/gtettzomob.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtzdqzwavr.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtxfboykkm.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtfoqdoavi.html

Py:   arr.insert(0, 0)
来源：http://hz.jianghu66.top/gtlykmfers.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtkqebxhua.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtivhlilfc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nanxinkj.top/gtjwrrxrxd.html

Java: list.add(0, 0);
来源：http://hz.nanxuanxn.top/gtqleoasfr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnqzz.top/gtfrfsjkrg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gthvbrdgxf.html

C#:   list.Insert(0, 0);
来源：http://hz.tanke756.top/gthnkbcwss.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtubfgcvpu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtujvxxwem.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.mhx1999.top/gtlszazydv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gtalktxkii.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtugkkomud.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenzaomai.com/gtusfhimld.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jyoumei.cn/gtftmqgghm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtlqmhzhhd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tanke756.top/gtrtnnmkml.html

[D05] 访问与修改元素
来源：http://hz.gaohongyu789.top/gtgsmpyjoh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtfxaxvukv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtpfgehfmx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dashuyun.cn/gtnasmmcji.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258.top/gttoznimgw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtzeplnkpr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtmhgazhnv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtiqberlii.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhengqikj.top/gtdcbbmjpl.html

[D06] 数组长度
来源：http://hz.gogol.net.cn/gtxotitcqi.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtzjyauypa.html

PHP:  count($arr);
来源：http://hz.smart0.xyz/gtowfusjbj.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtgsmyixus.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtlmbhixrf.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtwznvltwc.html

Go:   len(arr)
来源：http://hz.gotoacloud.top/gtwaznxbjo.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtjqdnbhnz.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtfdrfchzj.html

[D07] 切片 / 取子数组
来源：http://hz.quarkkingdee.top/gtxnvivagv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtlgxsnkoi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gtygcoalql.html

JS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtzookdcgh.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gteawqrsla.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtatbyewzd.html

Go:   arr[1:4]
来源：http://hz.jlsjyb.cn/gtgpkdjdmc.html

Ruby: arr[1, 3]
来源：http://hz.gzhubu.top/gtbeiqcmij.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtivtktimn.html

[D08] 合并两个数组
来源：http://hz.52xcode.cn/gtoqappbsq.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigufen.top/gtdkbcgthl.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtueotyubw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guowangkeji.top/gtrzidwowt.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtmueivyyj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gthbaltlqd.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gtucczycqk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jianghu66.top/gtsalcthvq.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhaomingkeji.xyz/gtpvbmdpsg.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtfkpuxcab.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtxpzymwnp.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtqswnksst.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtbkuhyrfh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gtvevbfslv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ivvv.top/gtpnfpnlpw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtzpbxsiqb.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtdobpszfb.html

C#:   list.Sort();
来源：http://hz.yj20258888.top/gtermaspqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenjidiqi.icu/gtwgagxvhm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtzoaqnova.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtoxgjbgwe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtzevkztbh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtsqbdhlok.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhoulong.xyz/gtuzckbvsg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhijiandao.cn/gtbfixtfwj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.feifeiyinyue.top/gtjkuwqiyc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gterprichc.html

[D11] 反转数组
来源：http://hz.jiagoushi.top/gtyihhngkb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gttrmniavs.html

PHP:  array_reverse($arr);
来源：http://hz.zycfv.cn/gtnpoydchh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtzkpwephl.html


<!-- 参考信息 -->