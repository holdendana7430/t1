代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shangyingyoupin.top/gtgncwwkou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.bjfxy.top/gttlmhsbla.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj20258.top/gtrxbiazzh.html

Py:   list(range(0, 10, 2))
来源：http://hz.daria6918.cn/gtxdapmoua.html

PHP:  range(0, 10, 2);
来源：http://hz.ywan-chungtsiang.top/gtkfzvhqpy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtkrssiqup.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.52xcode.cn/gtutjibokl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gogol.net.cn/gtktyqpiuj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fengsongda.top/gtcfvzvtwy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nanxuanxn.top/gtbwtajkid.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hfpthk.cn/gtmeeypkrz.html

[B12] 跳出多层循环
来源：http://hz.ywan-chungtsiang.top/gtqsxwgytb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ywan-chungtsiang.top/gthvlwhtwf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.316326.xyz/gtxawkixih.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtcxrwjujz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtrevkcnla.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtzbnwyvax.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtpozsqrlb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.haohaochexian.top/gtcfkptlpz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dianchejie.cn/gturstijgi.html

[B13] 判断是否为数字
来源：http://hz.ydjk.org.cn/gtagxolysv.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgfzy.top/gttdlrbgyd.html

PHP:  is_numeric($x)
来源：http://hz.zhaomingkeji.xyz/gtcbjvtwee.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtqhqglnrb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhoulong.xyz/gtqzoegtnl.html

Java: x instanceof Number
来源：http://hz.sweek.top/gtzlqjyflc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.andypj.xyz/gtwpgpazjc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yangfankeji.com/gtrzsdfizz.html

C#:   x is int or double or decimal
来源：http://hz.xuanzx.com/gtpqjxxclf.html

[B14] 判断值是否在集合内
来源：http://hz.zhengqikj.top/gtlqkvreyg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yueranfly.top/gtqegrglum.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cqqwz.cn/gtymfthrhc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtewjtdmeu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gzhubu.top/gtglcyegxz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.snrcjt.cn/gtxgllflho.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenzaomai.com/gtgpyydhdq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ehwqpu.com/gtajzfyxbn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtvgwtdnlf.html

[B15] 布尔运算与取反
来源：http://hz.zhijiandao.cn/gtmfjupthb.html

Py:   a and b or not c
来源：http://hz.zhaomingkeji.xyz/gtveyjybbd.html

PHP:  $a && $b || !$c
来源：http://hz.tianlin.xyz/gtptflihyc.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gtvtilyfti.html

TS:   a && b || !c
来源：http://hz.chenzaomai.com/gtkywtucja.html

Java: a && b || !c
来源：http://hz.ppjwa.cn/gtvfukxkmg.html

Go:   a && b || !c
来源：http://hz.smart0.xyz/gtanwdmxdj.html

Ruby: a && b || !c
来源：http://hz.yongpay.top/gtoeppiffk.html

C#:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtlvgxyqyp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtcgxziwvv.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtmipzpujr.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtyfvxnytq.html

JS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtebgaxldk.html

TS:   if (!data) return;
来源：http://hz.yuanzhike.top/gtkltlckhc.html

Java: if (data == null) return;
来源：http://hz.pycfn.com/gtxdsrknio.html

Go:   if data == nil { return }
来源：http://hz.shzxlz.cn/gtccfdqjaw.html

Ruby: return if data.nil?
来源：http://hz.jiagoushi.top/gtvgaeiyrx.html

C#:   if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gttxdmgitg.html

================================================================================
来源：http://hz.aibaodan.cn/gtcfriwnkt.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gtxgdamdfk.html

================================================================================
来源：http://hz.iojbl.cn/gtkwnhaxxc.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtbqskybbp.html

Py:   def add(a, b): return a + b
来源：http://hz.kuanghao11.cn/gtmiqzkbjm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtrluejlut.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtqtbbanhc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtqukiaxji.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtinimvnmc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhoulong.xyz/gtnlsfmnnh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.pengpengdd.cyou/gttkakzlzj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtghmbisdc.html

[C02] 默认参数
来源：http://hz.ehwqpu.com/gtqjlndktq.html

Py:   def greet(name="World"): return name
来源：http://hz.cdnleiting.top/gtsqetgllk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtdddzbtwa.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.meibo888.top/gtvbvtkneu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtjylptmsb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.pycfn.com/gtfpmjqsns.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dianchejie.cn/gtydazbwpq.html

Ruby: def greet(name = "World") = name
来源：http://hz.shanyushiyangtech.top/gtrygmbeep.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guannengcc.top/gtzalstcfx.html

[C03] 可变参数
来源：http://hz.zdqjudy.top/gtgpootskl.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gtycaprjyj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.meibo888.top/gtioizsjiv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cdnleiting.top/gtmrliwgxb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtlwwwcjtl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.bjfxy.top/gtodllwdfk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhengqikj.top/gtaevcmbbq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.redwolf501.top/gtjdhkffub.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtlhmyhaqh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ppjwa.cn/gtxryorqfz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.smart0.xyz/gtkvbbkkrk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.bjfxy.top/gtmlfvxoej.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtbmmwawxe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tanke756.top/gtjrxrdnuu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aizwys.cn/gtlfqsocsn.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj202588.top/gthelnsttr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtiazbwcuu.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtycdttbik.html

[C05] 返回多个值
来源：http://hz.hammf.cn/gtopemlhch.html

Py:   return a, b
来源：http://hz.dashuyun.cn/gtzcwhfvjg.html

PHP:  return [$a, $b];
来源：http://hz.zhiwuduotai.top/gtvxydbxcu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.meibo888.top/gtjrtnbsfz.html

TS:   return { a, b };
来源：http://hz.yueranfly.top/gtxtuhxwoz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xingfuxueyuan.xyz/gtwjrfjxtu.html

Go:   return a, b
来源：http://hz.kuanghao11.cn/gtzqcpddzz.html

Ruby: return a, b
来源：http://hz.xuetiantiany.cn/gtuajuyeed.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gtzspacjow.html

[C06] 匿名函数 / lambda
来源：http://hz.hnxiangtu.top/gthztkwacu.html

Py:   square = lambda x: x * x
来源：http://hz.dashuyun.cn/gttltncbdv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.0kj1m.cn/gtxupbrxci.html

JS:   const square = x => x * x;
来源：http://hz.gaohongyu789.top/gttdhcxolx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jiagoushi.top/gtrwxegqrl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gtkbcnfgrg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daxiang520.top/gtgblwjbjv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hysaishi.cn/gtgrxumzlg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtgwtdwbox.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtwxhhyisk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ehwqpu.com/gtusiauvwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.havefunace.top/gtsmdiwddf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ywan-chungtsiang.top/gtlysdxhlf.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtmdmxyols.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtpavvlaox.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.snrcjt.cn/gtfhnuqxfr.html

Ruby: arr.map(&:upcase)
来源：http://hz.havefunace.top/gteiijfkun.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gtoplabjkm.html

[C08] 闭包
来源：http://hz.jinqigufen.top/gtyduffygf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.bjfxy.top/gtfpupljsf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtkvgxlmgw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtjiwookdp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtbnqzvkbl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dianchejie.cn/gtukkxqnrr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtkmxdfbpw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258888.top/gtygdjwfpf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtxrqmemzo.html

[C09] 递归
来源：http://hz.cheryme.top/gtnxpnlzap.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtepydurbg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.svipenyu.cn/gtldncning.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtrtdibqbg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtfpunbcej.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuetiantiany.cn/gtoclqqxdl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yangfankeji.com/gtcsjdvear.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gttjgsvgon.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gtvlgilxmd.html

[C10] 变量作用域
来源：http://hz.daria6918.cn/gtruhgrxvo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxinkj.top/gtgdocsjqg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigufen.top/gtvmacjjon.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuxming.cn/gtvidolxzx.html

TS:   同 JS
来源：http://hz.jyoumei.cn/gtzxrumfgy.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtffnhcwnr.html

Go:   花括号块级作用域
来源：http://hz.cdnleiting.top/gtzvinumoq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xylfe.cn/gtagqfhdcy.html

C#:   块级作用域
来源：http://hz.c1oappe.top/gtyobcknnl.html

[C11] 模块导入与导出
来源：http://hz.chenzaomai.com/gtcvrpkija.html

Py:   from module import func
来源：http://hz.zycfv.cn/gtjtvtijtg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aibaodan.cn/gtszsytign.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtgndscwie.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhengqikj.top/gtwbzwyhur.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtrcburfpc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.andypj.xyz/gtimtsjjff.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtrdgttgca.html

C#:   using System.Text;
来源：http://hz.meibo888.top/gtqimcneqq.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhaomingkeji.xyz/gtvtgjhfbl.html

Py:   (lambda: print("run"))()
来源：http://hz.meibo888.top/gtxowuqrlg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenjidiqi.icu/gtlvxfpjdh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtqilkyakr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtyuucvyhu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gtlzvdrhoq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gtiodqsocv.html

Ruby: -> { puts "run" }.call
来源：http://hz.xziqi.cn/gtojkgtknb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gttmsxrwkr.html

[C13] 类型声明 / 类型注解
来源：http://hz.quarkkingdee.top/gtetbajjaj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhaomingkeji.xyz/gtvsbujbgi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtriwffcxg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtuqhnhlew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtjvnxmhvs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gthrhrepyn.html

Go:   func add(a, b int) int
来源：http://hz.tanke756.top/gtrzvnnqfg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sufxvd.cn/gtdnweuvht.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxinkj.top/gtxzqwheko.html

[C14] 泛型函数
来源：http://hz.ydjk.org.cn/gtgtnpazfg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtdxtutcas.html

PHP:  // 无泛型
来源：http://hz.feifeiyinyue.top/gthtwxncch.html

JS:   // 无泛型
来源：http://hz.cheryme.top/gtryimbarj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinghuilouyu.cn/gtppniozom.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtxopsneov.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gtvdixzuxq.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gtgwrnacuo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shanyushiyangtech.top/gtojqcoiwe.html

[C15] 解构 / 展开参数
来源：http://hz.birdmap.top/gtznjnydkj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtseyxypal.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhongyouzk.top/gtftjjbjoj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtuxobquwo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.snrcjt.cn/gtbbtpyaga.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtrmhobopl.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtxsuwxqii.html

Ruby: a, b = pair
来源：http://hz.jqgufenzy.top/gthrgqlscy.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtglrwjxiz.html

[C16] 函数 / 方法重载
来源：http://hz.wangdashe.top/gtrbtmjvng.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gttrokkeab.html

PHP:  // 无重载
来源：http://hz.zhongyouzk.top/gtkxufhuvq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhoulong.xyz/gtshzacunj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hammf.cn/gtcumgnnfo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.316326.xyz/gttqadepoa.html

Go:   // 无重载：用不同函数名
来源：http://hz.pengpengdd.cyou/gtprudrzvb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gteptelzek.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtcyfpewuu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbpgxpvrv.html

D. 数组 / 列表 / 集合
来源：http://hz.zhongyouzk.top/gtomecfyfi.html

================================================================================
来源：http://hz.yj20258.top/gtbwjhzmyj.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gtlonvpeir.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yongpay.top/gtfdskqywb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangshuangyany.cn/gtzddfjzkd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xziqi.cn/gtkcjutpau.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtubgswool.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtqlkvzyqk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtxafczche.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gogol.net.cn/gtvylkwtou.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cqqwz.cn/gtvedzzeaj.html

[D02] 追加元素到末尾
来源：http://hz.yj20258888.top/gtjsscxcmi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yongpay.top/gtarpdmkwp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtqtwkdszz.html

JS:   arr.push(4);
来源：http://hz.redwolf501.top/gtsrbupifi.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gtfauqxjnp.html

Java: list.add(4);
来源：http://hz.yongpay.top/gtgnicbwdj.html

Go:   arr = append(arr, 4)
来源：http://hz.tianlin.xyz/gtknjajjkf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cqqwz.cn/gtqwzrvhrf.html

C#:   list.Add(4);
来源：http://hz.fzhhl.top/gtclrhbigw.html

[D03] 在指定位置插入元素
来源：http://hz.aibaodan.cn/gtrbbxuacr.html

Py:   arr.insert(0, 0)
来源：http://hz.cqqwz.cn/gtqulrfkbi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gogol.net.cn/gttqvwscfj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xingfuxueyuan.xyz/gtzarnhpqe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtwwfetmno.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtgctljhvy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.meibo888.top/gtsqwixhkb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.iojbl.cn/gtpgyyxvzs.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtzstfiuiv.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtnvddxfey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtmaujjfbp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gttfzmxbck.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtkvdeqrjm.html

TS:   arr.splice(0, 1);
来源：http://hz.mhx1999.top/gttwhvsuht.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtomuhtkqc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yonumen.top/gtmskzbtsl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yangfankeji.com/gtdngyeuhk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cucudq.cn/gtazfogryi.html

[D05] 访问与修改元素
来源：http://hz.yangfankeji.com/gtyraszird.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gterfeauml.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtugawxzmb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtbpadpcdv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtjdlglvsp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.quarkkingdee.top/gtdyfvojdz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtwjjxmnla.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtcfpbyrry.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuxming.cn/gtnjeeyosk.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gttumumnii.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtwrrpjkfg.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtlnkrdpzh.html

JS:   arr.length
来源：http://hz.smart0.xyz/gtqvndstie.html

TS:   arr.length
来源：http://hz.xingfuxueyuan.xyz/gtdxambcpp.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtfnihonlr.html

Go:   len(arr)
来源：http://hz.daxiang520.top/gtbgqlutkt.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtuggwjvbj.html

C#:   list.Count;
来源：http://hz.andypj.xyz/gtutifrasp.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gtjcdvpgqe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtuqyhvode.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtjglfkaxi.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gteybdqmdv.html

TS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtebhpmlgz.html

Java: list.subList(1, 4);
来源：http://hz.dianchejie.cn/gtgsyenwiv.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtrxcbyqbq.html

Ruby: arr[1, 3]
来源：http://hz.yuxming.cn/gtfljphinm.html

C#:   list.GetRange(1, 3);
来源：http://hz.cashguo.top/gtjthdhnwb.html

[D08] 合并两个数组
来源：http://hz.redwolf501.top/gtioirauav.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtjkwbidzp.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gtsxywbhwo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xingfuxueyuan.xyz/gtxcrwmwmu.html

TS:   [...a, ...b];
来源：http://hz.redwolf501.top/gtkbpgpcku.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.wangdashe.top/gtyyvrukgd.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtmclpsbjj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yvedp.cn/gtqtqkjmwg.html

C#:   a.Concat(b).ToList()
来源：http://hz.sxryk.cn/gtzazrqmui.html

[D09] 排序（升序）
来源：http://hz.shuidangran.top/gtlyqlocmc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtjdbumqds.html

PHP:  sort($arr);
来源：http://hz.jinghuilouyu.cn/gtyiivcrrg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ivvv.top/gtjpoklohx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gttdfjnbgl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtayggzdob.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtdjvhtxvf.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtsxogkwjm.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtqocsagap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gtbxtbycks.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtsvnjdkap.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtcxoqsroc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gtianrevqi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtcphtdybv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yueranfly.top/gtcuplodry.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gteytijmty.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.svipenyu.cn/gtaofwwkco.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtjeqjivos.html

[D11] 反转数组
来源：http://hz.pengpengdd.cyou/gtijzgcxgi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtzjltxbre.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtnnmwzyqw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.pengpengdd.cyou/gtjxwdhfif.html


<!-- 参考信息 -->