代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtajorpbjr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gtolujyoco.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.smart0.xyz/gteloqxytp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gtvkxryydq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gteynzzkjo.html

[B10] 遍历同时拿索引
来源：http://hz.jinghuilouyu.cn/gtgdoihcqx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nwbrower.top/gtmepzermc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtolecgouc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daxiang520.top/gtpwmiqbjz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj202588.top/gtjlcwazkd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ehwqpu.com/gtmvuwwohg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangdashe.top/gtjgzgtpnf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gzhubu.top/gtyrhwtohf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cheryme.top/gtkqqxlmoc.html

[B11] 生成数字序列 / 区间
来源：http://hz.sweek.top/gtvfgvlcsn.html

Py:   list(range(0, 10, 2))
来源：http://hz.cheryme.top/gttnpszauv.html

PHP:  range(0, 10, 2);
来源：http://hz.zhongyouzk.top/gtknerutqq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtxaxjmbxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydjk.org.cn/gtynwxrwia.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj202588.top/gtszixwqfj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hammf.cn/gtvpclrjwt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhijiandao.cn/gtomtftbha.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hongshengwenyu.top/gtwrqgalcj.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtlxghmxnp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.andypj.xyz/gtcbtnsjfw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xuetiantiany.cn/gthkzywkdr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gteigmbwzk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gttvfeuevy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtlpdbjnnu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gaohongyu789.top/gtlxresjde.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fzhhl.top/gtmgjsnelt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pycfn.com/gtnodyxwvq.html

[B13] 判断是否为数字
来源：http://hz.yonumen.top/gtberiswzr.html

Py:   isinstance(x, (int, float))
来源：http://hz.hysaishi.cn/gtvbkeiciz.html

PHP:  is_numeric($x)
来源：http://hz.jinqigufen.top/gtygymqshq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtrggqticx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gtilojkvsy.html

Java: x instanceof Number
来源：http://hz.guannengcc.top/gtqqlmonps.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtjxcomhjn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinqigfzy.top/gtjjprftus.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gtfceuvjew.html

[B14] 判断值是否在集合内
来源：http://hz.zhaomingkeji.xyz/gtabgfphjt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ywan-chungtsiang.top/gtdpgupnfo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sxryk.cn/gtafggdbry.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gttklvcnhk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtyuosuhhy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhijiandao.cn/gtrsyhuewh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxinkj.top/gtvlnbrlja.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangtech.top/gtuxwogoax.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sysykeji.top/gtqsorzare.html

[B15] 布尔运算与取反
来源：http://hz.sysykeji.top/gtlrxumqsw.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtuflryqpz.html

PHP:  $a && $b || !$c
来源：http://hz.hysaishi.cn/gtpudufrtw.html

JS:   a && b || !c
来源：http://hz.ybcxt.top/gtrjrowjgl.html

TS:   a && b || !c
来源：http://hz.cdnleiting.top/gtkormtbjm.html

Java: a && b || !c
来源：http://hz.nanxuanxn.top/gtgwttjhsr.html

Go:   a && b || !c
来源：http://hz.tian-w.cn/gtcghbvjwm.html

Ruby: a && b || !c
来源：http://hz.redwolf501.top/gtqyoaqotb.html

C#:   a && b || !c
来源：http://hz.vqdsnc.cn/gtzyweajzz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtuotecwzy.html

Py:   if not data: return
来源：http://hz.cqqwz.cn/gtfrdngcsi.html

PHP:  if (!$data) { return; }
来源：http://hz.fengsongda.top/gtdorekjru.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtunztnnmb.html

TS:   if (!data) return;
来源：http://hz.cheryme.top/gtnrdytlof.html

Java: if (data == null) return;
来源：http://hz.xinyue.icu/gtxeraqsjl.html

Go:   if data == nil { return }
来源：http://hz.hysaishi.cn/gtlsmjawgp.html

Ruby: return if data.nil?
来源：http://hz.shangyingyoupin.top/gtdipyqfse.html

C#:   if (data == null) return;
来源：http://hz.zdqjudy.top/gtqtwqbrcg.html

================================================================================
来源：http://hz.yvedp.cn/gtywxoalol.html

C. 函数与作用域
来源：http://hz.gogol.net.cn/gtisutplaq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtdakzmtki.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtsdvrygvs.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtqlxugpjx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtmuoatndx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258888.top/gtnwzwwgtz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtkzzcmigf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtkjqguuxp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xziqi.cn/gtysjgbxqs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.meibo888.top/gtzkwagyhu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtauysltsg.html

[C02] 默认参数
来源：http://hz.redwolf501.top/gtjgllrmij.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtmuwbdivm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xziqi.cn/gtmqsutgnp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hfpthk.cn/gtnthhspio.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ehwqpu.com/gtlpnoyjfq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gtqmsyxhjf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhoulong.xyz/gtcsfmpnyc.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtbglkvdsb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigufen.top/gtbkjohrzx.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtmnysbmnl.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhijiandao.cn/gtprqwqdcq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gtaitawzlt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gttqstntnk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtfoqvovhc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtquqtkydm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnqzz.top/gtbciwmsqj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ppjwa.cn/gtdstwzkju.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj20258.top/gtxijiwoam.html

[C04] 命名参数 / 关键字参数
来源：http://hz.daria6918.cn/gtuibinhjw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhiwuduotai.top/gtpuffgfil.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dianchejie.cn/gttbkwvuyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtbhfhmnkk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtqvxymhdq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtwevvwwlm.html

Go:   // 无：用配置结构体参数
来源：http://hz.shuidangran.top/gtvpbcskqd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gttzxqadkd.html

C#:   f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtzughrire.html

[C05] 返回多个值
来源：http://hz.hfpthk.cn/gtvrdqgncq.html

Py:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtqfmctrfd.html

PHP:  return [$a, $b];
来源：http://hz.xuanzx.com/gtwmfyfaim.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yueranfly.top/gtnsgyilhq.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtviahllsb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangdashe.top/gtcfhzkvjw.html

Go:   return a, b
来源：http://hz.jinyuanbaomall.cn/gttpirfzcz.html

Ruby: return a, b
来源：http://hz.jianghu66.top/gtevqvjipq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gthgeavgcb.html

[C06] 匿名函数 / lambda
来源：http://hz.daxiang520.top/gtegeddlkd.html

Py:   square = lambda x: x * x
来源：http://hz.fengsongda.top/gtbqqvjciz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gtksrxonlx.html

JS:   const square = x => x * x;
来源：http://hz.bjfxy.top/gtsodjgtse.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yueranfly.top/gthkshjkah.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gttomnliim.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xziqi.cn/gtfiwptwbc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnxiangtu.top/gtdneeeheu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtdttotkjg.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gthazyvzar.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jiagoushi.top/gtiqpdjmdv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aizwys.cn/gtkoewunmm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtbxkxhrkg.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtfgxqebco.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gogol.net.cn/gtxnfnyult.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.quarkkingdee.top/gtyrghekbu.html

Ruby: arr.map(&:upcase)
来源：http://hz.c1oappe.top/gtsdjidgaz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258888.top/gttkfeznqt.html

[C08] 闭包
来源：http://hz.zdqjudy.top/gtuuymcxkd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pengpengdd.cyou/gtmzymdwyq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhaomingkeji.xyz/gttfceborc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtvwjaxnkx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gthqnjdkxs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuxming.cn/gtaonrrcwz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangtech.top/gtkqdkgwkv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhiwuduotai.top/gtadivvbje.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtbfpxomkc.html

[C09] 递归
来源：http://hz.yonumen.top/gtdqwlrbsx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cqqwz.cn/gthdhcajka.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.9152youxi.cn/gtubezjhhp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtriwitwsf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtmhrtkjnc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtvvubduor.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gtvzcypoky.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hfpthk.cn/gthdmvkkrg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yanxiufei.cn/gtgnsqrgxa.html

[C10] 变量作用域
来源：http://hz.dianchejie.cn/gtlvchfefi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenlongwang.top/gtppnlowik.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtrdkqocnl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tian-w.cn/gtfgmzsrwk.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtbtntnihs.html

Java: 方法内为块级作用域
来源：http://hz.tanke756.top/gtdizdvsrp.html

Go:   花括号块级作用域
来源：http://hz.smart0.xyz/gtkcvsaskb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hfpthk.cn/gtkftrkiik.html

C#:   块级作用域
来源：http://hz.ydzc1.top/gttyyxvrvv.html

[C11] 模块导入与导出
来源：http://hz.zhixingplan.top/gtoklpmfcm.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtpwrvluhq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtzjuzdxpe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cucudq.cn/gtbvomelas.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cashguo.top/gtajjzzheu.html

Java: import java.util.List;
来源：http://hz.mhx1999.top/gtqjfzmwdq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yvedp.cn/gtpzsjqwbr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cucudq.cn/gtplwdhlgo.html

C#:   using System.Text;
来源：http://hz.ehwqpu.com/gtqzlfndzk.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gtrycrowwm.html

Py:   (lambda: print("run"))()
来源：http://hz.cheryme.top/gtmatuvgti.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daria6918.cn/gtzppnqqzc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtliezcyuu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtkgcokfoh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.andypj.xyz/gtugnqtpbp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sysykeji.top/gtjllxeltg.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtrqznowba.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtrucjmjnt.html

[C13] 类型声明 / 类型注解
来源：http://hz.sufxvd.cn/gtljymbdjz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gotoacloud.top/gttviuwool.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtwgeucybu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtgzyjsakx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtvzjsigjy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtsvdzxdxd.html

Go:   func add(a, b int) int
来源：http://hz.hnqzz.top/gtpnauuzxs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtzycvdagi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtkrrvolcd.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtvemtrbsa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ivvv.top/gtgydcjjfm.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gttnfjklue.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtqiqdivye.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xziqi.cn/gtxolahgne.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hammf.cn/gtjonpdnxk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtgkehugzr.html

Ruby: # 无泛型
来源：http://hz.xuanzx.com/gtcltpidof.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtldiacapt.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gthngqyeip.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtdaivhtgb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gtmrniczrr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.havefunace.top/gtrgzabsqg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.birdmap.top/gtqyavslll.html

Java: // 无解构
来源：http://hz.xuetiantiany.cn/gtyuqsmzxz.html

Go:   // 无解构
来源：http://hz.yj20258.top/gtytpwtvpq.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gtbnmmvtve.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gtjrguqkcr.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtgnogonzq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuanzhike.top/gtzpsmsvfb.html

PHP:  // 无重载
来源：http://hz.shzxlz.cn/gtxccuklhh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangkeji.top/gtzdnciwax.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hfpthk.cn/gtdgodajiq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj202588.top/gttwhxxkvj.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxinkj.top/gtgiwnkgzu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aibaodan.cn/gthlihxhnv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hfpthk.cn/gtnoxohwyg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtagedmlvj.html

D. 数组 / 列表 / 集合
来源：http://hz.zhiwuduotai.top/gtcrjkzbnr.html

================================================================================
来源：http://hz.wangdashe.top/gtlelztasi.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtltrkytgh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yvedp.cn/gtfimlmjue.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtzslvdoqf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.vqdsnc.cn/gthrzknheh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuanzhike.top/gtkqptwoxh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtvknttcqn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtafocacts.html

Ruby: arr = [1, 2, 3]
来源：http://hz.mhx1999.top/gtnrsedbyn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtmaeoltzw.html

[D02] 追加元素到末尾
来源：http://hz.ppjwa.cn/gtazslqqmm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.haohaochexian.top/gtzyosrbfn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.0kj1m.cn/gtjrxftfuc.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtodhwjuon.html

TS:   arr.push(4);
来源：http://hz.guowangkeji.top/gtgifgjugs.html

Java: list.add(4);
来源：http://hz.xziqi.cn/gtellighyn.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gtfykirnyx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtstisontk.html

C#:   list.Add(4);
来源：http://hz.chenzaomai.com/gtuhnobtlt.html

[D03] 在指定位置插入元素
来源：http://hz.zhongyouzk.top/gtubyvtbmm.html

Py:   arr.insert(0, 0)
来源：http://hz.pycfn.com/gtrjkmspfi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.redwolf501.top/gtpztxwuis.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xingfuxueyuan.xyz/gtbfzngadv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhiwuduotai.top/gtqzmmffwy.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gttprxvmgf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtqchlbuub.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtaprtrqrx.html

C#:   list.Insert(0, 0);
来源：http://hz.aizwys.cn/gtnildqlao.html

[D04] 删除元素
来源：http://hz.hfpthk.cn/gtyvtcmzqe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtgwyuvivu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhoulong.xyz/gticajycdu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.redwolf501.top/gtxezjcafm.html

TS:   arr.splice(0, 1);
来源：http://hz.cucudq.cn/gtkdwwqyaz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gtbkkgddwe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtmscklpoc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtpzmfskjz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xinyue.icu/gthcqukaqk.html

[D05] 访问与修改元素
来源：http://hz.birdmap.top/gtivsiwcoc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtvxctbjso.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtqralmssr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtaszfqgsz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtqfudoiaf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtskveacmu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtmjmwvojf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtgkttvdtg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gtxtzgvnwz.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtdrgtriyx.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gtsnmqbhiy.html

PHP:  count($arr);
来源：http://hz.birdmap.top/gtsdhbkcmo.html

JS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtiptluhnr.html

TS:   arr.length
来源：http://hz.ehwqpu.com/gthvskfmrz.html

Java: list.size();
来源：http://hz.yj20258.top/gtvzdebmgl.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtycsbfolw.html

Ruby: arr.length; arr.size
来源：http://hz.birdmap.top/gtngdemdln.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtnnzekvfa.html

[D07] 切片 / 取子数组
来源：http://hz.zhiwuduotai.top/gtpgmkrmjq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dianchejie.cn/gtkpoqpsso.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtolhijein.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtqwtnvwuw.html

TS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gteknmotrr.html

Java: list.subList(1, 4);
来源：http://hz.sweek.top/gtkvwwwbku.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtograapiw.html

Ruby: arr[1, 3]
来源：http://hz.nwbrower.top/gtntptkhwu.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gteavcprrm.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtvcfaiqpe.html

Py:   a + b;  a.extend(b)
来源：http://hz.shuidangran.top/gtpwjflews.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtqnmonole.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnqzz.top/gtaanlvkng.html

TS:   [...a, ...b];
来源：http://hz.chenjidiqi.icu/gtzhvslxqv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.smart0.xyz/gtsumbtmsb.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtiuutxnag.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtcqyotpkl.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuanzhike.top/gtvtsezxsr.html

[D09] 排序（升序）
来源：http://hz.mhx1999.top/gtboswwguw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuxming.cn/gtgybjvnth.html

PHP:  sort($arr);
来源：http://hz.hnqzz.top/gttwnpstyu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtnzjdydux.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtaqdirbdv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtgsxrlxee.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gtiidnfrog.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtcctlrnyq.html

C#:   list.Sort();
来源：http://hz.jqgufenzy.top/gtdiuhcdup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hfpthk.cn/gtmuedexpm.html


<!-- 参考信息 -->