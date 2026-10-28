代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gttrvpxuwq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fzhhl.top/gtnunuetsi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zdqjudy.top/gtravfvngk.html

[B12] 跳出多层循环
来源：http://hz.mhx1999.top/gtiddcmlyu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pengpengdd.cyou/gtvlwzpcmt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtqxmrxbdj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtawurftaa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtluvsxlqh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtfwkekmjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtqceraqkc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtlksnafri.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydzc1.top/gtescowzjc.html

[B13] 判断是否为数字
来源：http://hz.xingfuxueyuan.xyz/gtdaphlqwt.html

Py:   isinstance(x, (int, float))
来源：http://hz.guannengcc.top/gtoojvkcrg.html

PHP:  is_numeric($x)
来源：http://hz.gogol.net.cn/gtcbtvmdao.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gttywonudg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtxtmzuiys.html

Java: x instanceof Number
来源：http://hz.gaohongyu789.top/gtjssukmpd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ivvv.top/gtrcyicxoc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jyoumei.cn/gtjojzvxdo.html

C#:   x is int or double or decimal
来源：http://hz.feifeiyinyue.top/gtsinivitv.html

[B14] 判断值是否在集合内
来源：http://hz.xziqi.cn/gtrjchatxg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.havefunace.top/gtuyaljhid.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hfpthk.cn/gtiwnofxls.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dashuyun.cn/gtiicvwymf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtgnhqbksi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxinkj.top/gtxebslftk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yanxiufei.cn/gtxyrdymhe.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenzaomai.com/gtmygnsthu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hnxiangtu.top/gttfjswenx.html

[B15] 布尔运算与取反
来源：http://hz.c1oappe.top/gtvhdsjhpz.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtiuyehjfm.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gtiowvqavq.html

JS:   a && b || !c
来源：http://hz.bjfxy.top/gtfwmyholv.html

TS:   a && b || !c
来源：http://hz.hfpthk.cn/gtjdqegsqn.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtwxoozndm.html

Go:   a && b || !c
来源：http://hz.guannengcc.top/gtplqmmswx.html

Ruby: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtnudiipeg.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtqjfdeeso.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.iojbl.cn/gtnryybqzh.html

Py:   if not data: return
来源：http://hz.cucudq.cn/gtvpgskrqk.html

PHP:  if (!$data) { return; }
来源：http://hz.yj20258.top/gtjqnukvsn.html

JS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtkvzexqqh.html

TS:   if (!data) return;
来源：http://hz.fzhhl.top/gtbzwmuspu.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gtrikhwgba.html

Go:   if data == nil { return }
来源：http://hz.dashuyun.cn/gtmvlyjsss.html

Ruby: return if data.nil?
来源：http://hz.c1oappe.top/gttaldfuqk.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtbbtdvewr.html

================================================================================
来源：http://hz.c1oappe.top/gtihsvevoz.html

C. 函数与作用域
来源：http://hz.zdqjudy.top/gttjydjqji.html

================================================================================
来源：http://hz.xziqi.cn/gtaydupydc.html

[C01] 定义函数
来源：http://hz.jianghu66.top/gtxpgjfazt.html

Py:   def add(a, b): return a + b
来源：http://hz.ydzc1.top/gtxjrnkglt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtfyloufgv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xylfe.cn/gtznnhyisn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtfnzzezhx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gttrtmdbvg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xinyue.icu/gttkyblpmc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangshuangyany.cn/gtxzxzqjdr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtvesqmlpf.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gtxtaintvl.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtjnbihyxk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtukidhads.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtotuxjdwn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtsfejtnzd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtwczemajy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhijiandao.cn/gtnsdxepql.html

Ruby: def greet(name = "World") = name
来源：http://hz.gotoacloud.top/gtkhmuhual.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxuanxn.top/gtbxmmjnsu.html

[C03] 可变参数
来源：http://hz.cashguo.top/gtvvgpnqak.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinghuilouyu.cn/gtswlwqcnm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gtonyflnob.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtmphcnhku.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtvlqowsbp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gttzcjgjsc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtfbukumcl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtawyzllzh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aibaodan.cn/gtxxgwwbtr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtpjxbwpfu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gogol.net.cn/gtejtocrpt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ppjwa.cn/gtxotbzalf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gthinuhsoh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hammf.cn/gtxwjfbkzm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuanzx.com/gtdkovnykq.html

Go:   // 无：用配置结构体参数
来源：http://hz.pycfn.com/gtckkjaasa.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtyxgkrwsd.html

C#:   f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtguuykwer.html

[C05] 返回多个值
来源：http://hz.zhiwuduotai.top/gtnlurpkvh.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gthsaevsyd.html

PHP:  return [$a, $b];
来源：http://hz.hongshengwenyu.top/gtaqavwyuj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yangfankeji.com/gtusgwoesj.html

TS:   return { a, b };
来源：http://hz.gzhubu.top/gtiqyoxmmz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtbnscovrc.html

Go:   return a, b
来源：http://hz.cqqwz.cn/gtbogurkpn.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtudjokody.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtalepmnch.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtmywdfsjr.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigufen.top/gtaubufxud.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gtinpymwpi.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtugozdfoo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgufenzy.top/gtukissbsr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.iojbl.cn/gtyffkxqls.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shuidangran.top/gtbfubupbs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhiwuduotai.top/gttmludbrj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtjwnijejy.html

[C07] 把函数作为参数传入
来源：http://hz.shzxlz.cn/gthrmxdwsl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuetiantiany.cn/gtkjfvppfr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhoulong.xyz/gtinmsnvvs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sysykeji.top/gtdcmlhtnz.html

TS:   arr.map(String)
来源：http://hz.xuetiantiany.cn/gtxrdpptcw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gtcsjoufyh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gtghmbkgdn.html

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtoutvdnnt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.0kj1m.cn/gtxzjgubvx.html

[C08] 闭包
来源：http://hz.tanke756.top/gtszacgyro.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.mhx1999.top/gtqbrtaeca.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pengpengdd.cyou/gtfxufbuev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtvxlpuuwp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtatgzlhfy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yvedp.cn/gtnfhehbjs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258888.top/gtxhbrjzca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.bjfxy.top/gtvyinlhla.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtphxhtstm.html

[C09] 递归
来源：http://hz.mhx1999.top/gtiytncqex.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtybfoxgss.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhijiandao.cn/gtgmksgnpt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtlftwuadr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtnvyfkdvj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtsyiqpima.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gttdatpmdm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtryqjtgwj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gthkcorlqn.html

[C10] 变量作用域
来源：http://hz.gotoacloud.top/gtgaqlrfsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gtqmlycmib.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nwbrower.top/gtnhggsojl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtyabxpqcm.html

TS:   同 JS
来源：http://hz.zhoulong.xyz/gtmqoqqbjx.html

Java: 方法内为块级作用域
来源：http://hz.shangyingyoupin.top/gtzxmnmdcu.html

Go:   花括号块级作用域
来源：http://hz.zhixingplan.top/gthgyvjvra.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shangyingyoupin.top/gtkhjpvndw.html

C#:   块级作用域
来源：http://hz.feifeiyinyue.top/gtpfehbobd.html

[C11] 模块导入与导出
来源：http://hz.wangdashe.top/gticbovntw.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtdbxlhkjr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtggukkvhf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.quarkkingdee.top/gtlwxbcjgz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sxryk.cn/gtsmljiprs.html

Java: import java.util.List;
来源：http://hz.feifeiyinyue.top/gtjhkkhgrn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtejgbtvqw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gtlrgpupif.html

C#:   using System.Text;
来源：http://hz.zdqjudy.top/gtofinmhlu.html

[C12] 立即执行函数 IIFE
来源：http://hz.svipenyu.cn/gtknusflca.html

Py:   (lambda: print("run"))()
来源：http://hz.cheryme.top/gtmlwcgoks.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtykkmeqxy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gthknvwwql.html

TS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtbuzslgsm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gthjssxxuo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtvjxfvykf.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydjk.org.cn/gtbublxghv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aibaodan.cn/gtjrlyscef.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenlongwang.top/gtecyxadmo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jiagoushi.top/gtzdxkusun.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gtyblovhfb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cqqwz.cn/gtmnlqzmea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gthtgzuzoe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtujbbfsce.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gtnaadnstj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtuverkdca.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ppjwa.cn/gtsvmbyzsg.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtlvchfovk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtmmkasego.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtnagbjudh.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtrtdjiwpw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj202588.top/gtehrpnrzq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hysaishi.cn/gtqbkyiifh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ppjwa.cn/gtmhgzhcla.html

Ruby: # 无泛型
来源：http://hz.hnqzz.top/gthwtmpzcx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.feifeiyinyue.top/gtoyzvprfi.html

[C15] 解构 / 展开参数
来源：http://hz.xziqi.cn/gtgzqozsov.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhoulong.xyz/gtbqiaaakq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.9152youxi.cn/gttfclolfw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtcytxthyu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtbetsmacr.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gttdevcrdf.html

Go:   // 无解构
来源：http://hz.jinqigufen.top/gtwrvbcyfw.html

Ruby: a, b = pair
来源：http://hz.hywenlv.cn/gtejjivvoy.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtkrdiyssb.html

[C16] 函数 / 方法重载
来源：http://hz.birdmap.top/gtsafbqudv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gtkkjxxxsw.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtxfwzrrap.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gtclonsaiu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtvjbmacqf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtmzrfjnyf.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtdlfieene.html

Ruby: # 无重载：靠动态参数
来源：http://hz.vqdsnc.cn/gtyigvkwtr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtullhzhfu.html

================================================================================
来源：http://hz.wangdashe.top/gtbefmsoyo.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gtiyzlwyhg.html

================================================================================
来源：http://hz.vqdsnc.cn/gtylzskbnc.html

[D01] 创建数组 / 列表
来源：http://hz.pycfn.com/gthlflvbzh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.aibaodan.cn/gtrnwcbotv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.iojbl.cn/gtsxbcihyh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinyuanbaomall.cn/gtnvgtfqpc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gthkugjlkq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhiwuduotai.top/gtxhkxdqna.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtsmtmurfp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cucudq.cn/gtyzyfaiok.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.smart0.xyz/gtifztiubn.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtpznecshq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtjasevzjw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cqqwz.cn/gtjhsiwgjd.html

JS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gtywuedred.html

TS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtksrtvghd.html

Java: list.add(4);
来源：http://hz.pengpengdd.cyou/gtybsqemem.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigfzy.top/gtipbwglqa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gtnzmvhlnt.html

C#:   list.Add(4);
来源：http://hz.redwolf501.top/gtgfjoxqun.html

[D03] 在指定位置插入元素
来源：http://hz.svipenyu.cn/gtifdjetsj.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtylyymcmz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yvedp.cn/gtmaiekpkd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sweek.top/gthnkjoyca.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.haohaochexian.top/gthowosgou.html

Java: list.add(0, 0);
来源：http://hz.xuanzx.com/gtilpdkkwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtynczyqic.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangkeji.top/gtfbqwvgro.html

C#:   list.Insert(0, 0);
来源：http://hz.sysykeji.top/gtzsubtxou.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtsxazzjww.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pycfn.com/gtvjygysvz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuanzx.com/gtrromfjcn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtejfjkxym.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtwbbojdmw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yvedp.cn/gthoysnfvl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gthtntyglt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gttnhgdjvx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cheryme.top/gtibxikvoy.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtdtrbgdvb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtsdzmgtlf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pycfn.com/gtgjreazvx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hammf.cn/gtmxfnkirp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtmzyajztx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ivvv.top/gtgvheofxy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.bjfxy.top/gtclqpyjqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtkyhpyqha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtexobreio.html

[D06] 数组长度
来源：http://hz.shuidangran.top/gtwecjghhj.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtwlbnbuob.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtqiyagjwn.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtftbtqkih.html

TS:   arr.length
来源：http://hz.jinqigufen.top/gtmtuxxyra.html

Java: list.size();
来源：http://hz.andypj.xyz/gtcgmwonaf.html

Go:   len(arr)
来源：http://hz.fzhhl.top/gtdulpeetf.html

Ruby: arr.length; arr.size
来源：http://hz.xylfe.cn/gtdftujrgl.html

C#:   list.Count;
来源：http://hz.jlsjyb.cn/gtkyrvgpmm.html

[D07] 切片 / 取子数组
来源：http://hz.zycfv.cn/gtmmortsjn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gtqmjtqaig.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gthcpbvvln.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtetdvonkz.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtncguqyhj.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gtvmtggkrw.html

Go:   arr[1:4]
来源：http://hz.cqqwz.cn/gtaedpixes.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gthryaogva.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhijiandao.cn/gtgfnyonsy.html

[D08] 合并两个数组
来源：http://hz.sxryk.cn/gtdpgufpnb.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtcaotgxbu.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtjuombbsm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenjidiqi.icu/gtsiattclh.html

TS:   [...a, ...b];
来源：http://hz.yueranfly.top/gtawqsdoak.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnxiangtu.top/gtvzdugkct.html

Go:   append(a, b...)
来源：http://hz.yongpay.top/gtxghegwvu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxinkj.top/gtmnsnugfo.html

C#:   a.Concat(b).ToList()
来源：http://hz.birdmap.top/gtfcxvuvro.html

[D09] 排序（升序）
来源：http://hz.pycfn.com/gtnwqpgevi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yonumen.top/gtanbbxkyb.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtykxhuzro.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtcfevpuwh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtjjnwalvm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtawvguxmb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtfdvqppem.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtoslkytcu.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gtskhpcwye.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gaohongyu789.top/gtcaibytyw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gtmmenaqkk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtcldzpqfu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gthfmrfmsp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtkcvtfbse.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtlqmrkcxo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.snrcjt.cn/gtbhqmtqqu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtfufqceqa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xingfuxueyuan.xyz/gtznldznom.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gtoqhgpgid.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgfzy.top/gtnhjfmyfm.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gtlmjvckfa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtdxzutguw.html

TS:   [...arr].reverse();
来源：http://hz.fzhhl.top/gtuuktdoou.html

Java: Collections.reverse(list);
来源：http://hz.xylfe.cn/gtdsiwruqs.html

Go:   slices.Reverse(arr)
来源：http://hz.hnqzz.top/gthtemoowz.html

Ruby: arr.reverse
来源：http://hz.wangshuangyany.cn/gtybymavbd.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gthkytdgnr.html

[D12] 查找元素下标
来源：http://hz.guannengcc.top/gtzicgdend.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gtmmzjbiqt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtmtephwfl.html


<!-- 参考信息 -->