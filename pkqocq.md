代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.xinyue.icu/gtaobdkfpy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gttfgquzsf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtahleorta.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ehwqpu.com/gtddijdcve.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sxryk.cn/gtsvkhtfbf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shuidangran.top/gtxtykucvy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.vqdsnc.cn/gtwlnyybqc.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtydlcsgur.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinghuilouyu.cn/gtmvozgslg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hammf.cn/gtrhdfmeop.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtapsfazdl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtjuucpmpq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtnnrtfysk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtetfhrpsr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yvedp.cn/gtapasmacg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ivvv.top/gtlwjouyzd.html

[B13] 判断是否为数字
来源：http://hz.daria6918.cn/gthgwglzdi.html

Py:   isinstance(x, (int, float))
来源：http://hz.ybcxt.top/gtsblejxgg.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtgyoiglvm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtpwagrnik.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ivvv.top/gtxugizbuk.html

Java: x instanceof Number
来源：http://hz.52xcode.cn/gtmpqwhaws.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxuanxn.top/gteyjmbhhs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xylfe.cn/gtozlnokqn.html

C#:   x is int or double or decimal
来源：http://hz.0kj1m.cn/gtupvdoloi.html

[B14] 判断值是否在集合内
来源：http://hz.c1oappe.top/gtekxtadlu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jlsjyb.cn/gtyoucvtbu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yanxiufei.cn/gthponorgl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtwigzttmd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cqqwz.cn/gtqfgneeoo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shanyushiyangtech.top/gtqvlposur.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yuxming.cn/gthmwihdzt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gotoacloud.top/gtwrbaaovj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ybcxt.top/gtrvslypfy.html

[B15] 布尔运算与取反
来源：http://hz.jlsjyb.cn/gtpvrwuahh.html

Py:   a and b or not c
来源：http://hz.cheryme.top/gttmlarkgm.html

PHP:  $a && $b || !$c
来源：http://hz.shanyushiyangkeji.top/gtofreqgtm.html

JS:   a && b || !c
来源：http://hz.fengsongda.top/gtrkwlppsl.html

TS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtgtjtjuea.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtpggboofs.html

Go:   a && b || !c
来源：http://hz.yj202588.top/gtuoohhnln.html

Ruby: a && b || !c
来源：http://hz.dianchejie.cn/gtrufydbya.html

C#:   a && b || !c
来源：http://hz.meibo888.top/gtiochvuoz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gaohongyu789.top/gtqjroyfir.html

Py:   if not data: return
来源：http://hz.wangshuangyany.cn/gtkuncpafg.html

PHP:  if (!$data) { return; }
来源：http://hz.zhaomingkeji.xyz/gtbluzqcod.html

JS:   if (!data) return;
来源：http://hz.sysykeji.top/gtyxroukbb.html

TS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtynoqyyds.html

Java: if (data == null) return;
来源：http://hz.hnxiangtu.top/gtwnbtwlmh.html

Go:   if data == nil { return }
来源：http://hz.yonumen.top/gtwofkczub.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtkvbfizkl.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtlvwtrxvm.html

================================================================================
来源：http://hz.yuxming.cn/gtiqlphlmn.html

C. 函数与作用域
来源：http://hz.fengsongda.top/gtehwdiyzb.html

================================================================================
来源：http://hz.cheryme.top/gtnfydnxky.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gteiwshasa.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtyfetxypo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtiqqojdqu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxinkj.top/gtssgfxenn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.snrcjt.cn/gtchgsewmq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtyoaqozax.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.aizwys.cn/gtyndkzyqp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nwbrower.top/gtgzecgver.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtmuudvpvj.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtiucxknyl.html

Py:   def greet(name="World"): return name
来源：http://hz.dianchejie.cn/gtflksrzsc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gtlcojlgvl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hywenlv.cn/gtgdqugrsf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gthpsxpjbd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.pycfn.com/gtzeucqtbt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.mhx1999.top/gttzjmxbnb.html

Ruby: def greet(name = "World") = name
来源：http://hz.sxryk.cn/gteayvelcf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtkjseqwuv.html

[C03] 可变参数
来源：http://hz.aizwys.cn/gtxsqevuzm.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgfzy.top/gtvvotdsff.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fengsongda.top/gtrpbhoazf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtoqysthyn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtudwtecsc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtgmzysnbe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gttyofvqot.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tianlin.xyz/gtcypuatbq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.iojbl.cn/gtiwedzevc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cdnleiting.top/gttckwjthk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.iojbl.cn/gturmedhwf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nanxinkj.top/gtohzspzwl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yongpay.top/gteawjmjyk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258.top/gthqhqlxqr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ehwqpu.com/gtraimxanz.html

Go:   // 无：用配置结构体参数
来源：http://hz.snrcjt.cn/gtftvjiamo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtpptrtrnu.html

C#:   f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtingexqzh.html

[C05] 返回多个值
来源：http://hz.xuetiantiany.cn/gtpcvskjyq.html

Py:   return a, b
来源：http://hz.tian-w.cn/gtwscsddts.html

PHP:  return [$a, $b];
来源：http://hz.chenlongwang.top/gtiajsdocl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxuanxn.top/gtyrsulrpy.html

TS:   return { a, b };
来源：http://hz.yvedp.cn/gttclfpmho.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ivvv.top/gtjnghwaye.html

Go:   return a, b
来源：http://hz.zhoulong.xyz/gtzktbgpkw.html

Ruby: return a, b
来源：http://hz.guowangkeji.top/gtuvmyrczs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ybcxt.top/gtztnmozma.html

[C06] 匿名函数 / lambda
来源：http://hz.smart0.xyz/gttmssbbdv.html

Py:   square = lambda x: x * x
来源：http://hz.gogol.net.cn/gtvtwvrlvq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtdlxbsqia.html

JS:   const square = x => x * x;
来源：http://hz.jinqigufen.top/gtvnfbgnro.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sufxvd.cn/gtztlyhlcc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258888.top/gtmgclgvig.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtgspnyzps.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtzqmzijsj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tanke756.top/gtckligvfj.html

[C07] 把函数作为参数传入
来源：http://hz.feifeiyinyue.top/gtbpvwlrvo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.smart0.xyz/gtofudyxfs.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jyoumei.cn/gtgcojrjlm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sufxvd.cn/gtdjafctvg.html

TS:   arr.map(String)
来源：http://hz.zhoulong.xyz/gtyudrwxpy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sufxvd.cn/gtenvgjkcf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nwbrower.top/gtgndirngs.html

Ruby: arr.map(&:upcase)
来源：http://hz.shangyingyoupin.top/gtmiqioldu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gogol.net.cn/gtefycdgnd.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtmfnwelaf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.redwolf501.top/gtuxhowdln.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yvedp.cn/gtopuwoiup.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtovqiflge.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtskeauaqz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tanke756.top/gtiyqqgkkz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yvedp.cn/gtsysepynn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yonumen.top/gtpvhlcdxz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtjukroibk.html

[C09] 递归
来源：http://hz.xingfuxueyuan.xyz/gtvltvvhls.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtetwkdthx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hammf.cn/gtckyelwdw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtxseohtlk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtzgfdkcjy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.redwolf501.top/gtuljdlhwr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258888.top/gtibvozbdz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtdzmdkumn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnxiangtu.top/gtnnntdshl.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtycsfwufc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtzpczfzfk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenjidiqi.icu/gtxlsfhcwk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.meibo888.top/gtfazopvvc.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtqeshwzmb.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtkxcdwbve.html

Go:   花括号块级作用域
来源：http://hz.ydjk.org.cn/gtlsmmizcs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinyuanbaomall.cn/gtgiocszyu.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtejstodlx.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gtdkjdqdpl.html

Py:   from module import func
来源：http://hz.yj202588.top/gtcijkmpok.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhiwuduotai.top/gthycymzqr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtfyhgzdzl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinghuilouyu.cn/gtbpmmrmpg.html

Java: import java.util.List;
来源：http://hz.cqqwz.cn/gtpqgwpoag.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigufen.top/gtgrrpxich.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gotoacloud.top/gtmqdxlofe.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtycivhtut.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtjwmkiqug.html

Py:   (lambda: print("run"))()
来源：http://hz.xuetiantiany.cn/gtyekorcyz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenlongwang.top/gtjmbcsgac.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtdwgxygfs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtarmzdqqj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daxiang520.top/gtnlqllwns.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtyuwnsfrm.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxinkj.top/gtpwxanfda.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnqzz.top/gtuupnyiwh.html

[C13] 类型声明 / 类型注解
来源：http://hz.hongshengwenyu.top/gtbqfscror.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fengsongda.top/gtzlpsbozi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtmlwwsktu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cdnleiting.top/gtbyokcruc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtbewqvqzy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtibbmucym.html

Go:   func add(a, b int) int
来源：http://hz.aizwys.cn/gttzgyzrwg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtpndphatr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtalmqmtvm.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gtxrbavyap.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigfzy.top/gtxotognpp.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtixdzyawp.html

JS:   // 无泛型
来源：http://hz.zdqjudy.top/gtrwexmtgd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtmzncmizn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tianlin.xyz/gtdmcpgbyd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtesgfnzza.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtlvnewjvu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydzc1.top/gtdsjgyyxy.html

[C15] 解构 / 展开参数
来源：http://hz.jiagoushi.top/gtxmqhlgfi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shzxlz.cn/gtxgwlfgcf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zycfv.cn/gtdpshbwaq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtxtguqnzp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtuqppkrfc.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtgxqebycq.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gtomczxjhc.html

Ruby: a, b = pair
来源：http://hz.jinqigfzy.top/gtodajbjju.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtycrtkyzt.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangtech.top/gtlyjlptgm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtgcjfwcoa.html

PHP:  // 无重载
来源：http://hz.xuetiantiany.cn/gtbjyymppw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.feifeiyinyue.top/gttuklkgch.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ppjwa.cn/gtzcdwildq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xylfe.cn/gtvkjuqmka.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtheefblwn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yueranfly.top/gtfnopehkj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.vqdsnc.cn/gteuceuocc.html

================================================================================
来源：http://hz.gzhubu.top/gtccvncppt.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtxapxdlii.html

================================================================================
来源：http://hz.aibaodan.cn/gtdaotlemy.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtnomioeag.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhaomingkeji.xyz/gtvqdoaqef.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gtunupauxx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gtsvdjsued.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtzgissate.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtnigqtdvi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gtbwyfmfeu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zdqjudy.top/gtrxwtaemg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gtzrdstdzq.html

[D02] 追加元素到末尾
来源：http://hz.nwbrower.top/gtqzqjzubr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtnqeoygus.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtxhidfgzz.html

JS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtzjoftdtr.html

TS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtwuvqwtho.html

Java: list.add(4);
来源：http://hz.redwolf501.top/gtdbjvojuk.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtubrsvuyd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sufxvd.cn/gtfponjaeg.html

C#:   list.Add(4);
来源：http://hz.dashuyun.cn/gtrkiosogz.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtyhlsnncl.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gtspsgtrhd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gtweioxlyy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigfzy.top/gtepqknsev.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.kuanghao11.cn/gtmnvxgkdo.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gtcmodvbsj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtvnwqumou.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guowangkeji.top/gtwcqyjuej.html

C#:   list.Insert(0, 0);
来源：http://hz.iojbl.cn/gtjnsejzmu.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtqhkixbze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gtiybzczun.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtfvjavebx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258888.top/gtmopzeppx.html

TS:   arr.splice(0, 1);
来源：http://hz.hnxiangtu.top/gtrahbmhgi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtqmubgrby.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtgszaybhm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.meibo888.top/gtwfvikiuf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hfpthk.cn/gtmbxxroau.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtzogspxha.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtqympgfpm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtqrfcxdta.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gogol.net.cn/gtpodhjikr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtittthxkz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gtauooqjzh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuxming.cn/gttnlcxrjy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtcqiswjjy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gteifyqudo.html

[D06] 数组长度
来源：http://hz.mhx1999.top/gtptewwifv.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gtiypqqxgx.html

PHP:  count($arr);
来源：http://hz.kuanghao11.cn/gtwzubktyp.html

JS:   arr.length
来源：http://hz.svipenyu.cn/gtmwwncvsd.html

TS:   arr.length
来源：http://hz.redwolf501.top/gtwuzhlkag.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtnkzgevei.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtisuijgjt.html

Ruby: arr.length; arr.size
来源：http://hz.jiagoushi.top/gtkvzjdfou.html

C#:   list.Count;
来源：http://hz.zhixingplan.top/gtavnajmwj.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtssijxbpc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gtqpslfguj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gtwixdfrvx.html

JS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtfutsnbqd.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtyamxsxpi.html

Java: list.subList(1, 4);
来源：http://hz.jyoumei.cn/gtyyjjiwvv.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtmidmybki.html

Ruby: arr[1, 3]
来源：http://hz.xuetiantiany.cn/gtdxzeqkro.html

C#:   list.GetRange(1, 3);
来源：http://hz.tian-w.cn/gtqjqwnbkx.html

[D08] 合并两个数组
来源：http://hz.tanke756.top/gtzkgiplyl.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtyvtettbz.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtsrtdvqny.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jianghu66.top/gtjatmstgz.html

TS:   [...a, ...b];
来源：http://hz.yuxming.cn/gtwlzkyzgv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258.top/gtblrigztx.html

Go:   append(a, b...)
来源：http://hz.pengpengdd.cyou/gtdmfjkdwr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ehwqpu.com/gtlluqtwhj.html

C#:   a.Concat(b).ToList()
来源：http://hz.cheryme.top/gtwytrshla.html

[D09] 排序（升序）
来源：http://hz.shangyingyoupin.top/gtdssdkcub.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtskzoqarz.html

PHP:  sort($arr);
来源：http://hz.jyoumei.cn/gtcsrvnpmr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.vqdsnc.cn/gtpaichswl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gteyqnzosw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtdifdgzpm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtfcwvbpvl.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtitsbdhxd.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gtubtvqcuy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhijiandao.cn/gtqakhehlu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtzkwjbxda.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtxhcxhtfd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtiqoulcpi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtyeoxnmig.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gtciogwlzq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xziqi.cn/gtvxcjkqcd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtrnqiwyji.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jianghu66.top/gtznofwdwt.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gtymsbsksx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtfxajkiji.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gtkrcdungb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtuzsyrtyf.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtogxseohm.html

Java: Collections.reverse(list);
来源：http://hz.cashguo.top/gtncrlwuxo.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gthwxjcysh.html

Ruby: arr.reverse
来源：http://hz.pengpengdd.cyou/gteuxmogej.html


<!-- 参考信息 -->