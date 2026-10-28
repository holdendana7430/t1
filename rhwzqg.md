代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtrehkdjqc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhijiandao.cn/gttokvfbpt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.smart0.xyz/gtfocuxaqf.html

[B12] 跳出多层循环
来源：http://hz.yuxming.cn/gthfognuuz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sxryk.cn/gtdzdowusn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.andypj.xyz/gtaaoosvdh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtbngnjehq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtqzqwkacm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtksvuqyei.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xziqi.cn/gtuiekxspw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dashuyun.cn/gtdxaunxvh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ivvv.top/gtobqjhcdy.html

[B13] 判断是否为数字
来源：http://hz.sweek.top/gtunbozhqf.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhengqikj.top/gtmsiqbcgm.html

PHP:  is_numeric($x)
来源：http://hz.aizwys.cn/gtujikizqi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtanlkfbnw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gthyucvkzp.html

Java: x instanceof Number
来源：http://hz.jianghu66.top/gtvqledaaa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zdqjudy.top/gtbgiewsyl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.haohaochexian.top/gttqijrwpa.html

C#:   x is int or double or decimal
来源：http://hz.zhoulong.xyz/gtxcromodl.html

[B14] 判断值是否在集合内
来源：http://hz.sufxvd.cn/gtlbhxyzab.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gotoacloud.top/gtjirzqzci.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.meibo888.top/gtimiiqntr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtoafclubq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yangfankeji.com/gtbgthspuk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhengqikj.top/gtptvbeoyr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yongpay.top/gtxcswyakr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.vqdsnc.cn/gtmwdzcczf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtybmwjrus.html

[B15] 布尔运算与取反
来源：http://hz.jinqigufen.top/gtbuukbpat.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gtqtyjikta.html

PHP:  $a && $b || !$c
来源：http://hz.aibaodan.cn/gtqbknhjqw.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtcwodpvnf.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtjkyaqapz.html

Java: a && b || !c
来源：http://hz.snrcjt.cn/gtxcqapikq.html

Go:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtahotfxwe.html

Ruby: a && b || !c
来源：http://hz.316326.xyz/gtwvwjgumu.html

C#:   a && b || !c
来源：http://hz.jyoumei.cn/gtmwkzzrau.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sxryk.cn/gtawefmcbp.html

Py:   if not data: return
来源：http://hz.birdmap.top/gtrvdijrhw.html

PHP:  if (!$data) { return; }
来源：http://hz.shanyushiyangtech.top/gtypgeumth.html

JS:   if (!data) return;
来源：http://hz.daxiang520.top/gtsvidfgjk.html

TS:   if (!data) return;
来源：http://hz.birdmap.top/gtiosxzbfh.html

Java: if (data == null) return;
来源：http://hz.redwolf501.top/gtsqcnhdsp.html

Go:   if data == nil { return }
来源：http://hz.0kj1m.cn/gtnxfiroga.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtkisnyxjr.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtyprjcnry.html

================================================================================
来源：http://hz.tanke756.top/gtmstvrbpw.html

C. 函数与作用域
来源：http://hz.redwolf501.top/gtbjckkayf.html

================================================================================
来源：http://hz.yj20258888.top/gtqabwbaua.html

[C01] 定义函数
来源：http://hz.yueranfly.top/gtlsxvumyp.html

Py:   def add(a, b): return a + b
来源：http://hz.kuanghao11.cn/gtnaqjlypi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gaohongyu789.top/gtyrasrplx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtopvulmeu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtzmjnvree.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtobbeibra.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigfzy.top/gtpoghkyfs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhijiandao.cn/gtrrvrvcrh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gttrfozmib.html

[C02] 默认参数
来源：http://hz.jinyuanbaomall.cn/gtcymvbbbu.html

Py:   def greet(name="World"): return name
来源：http://hz.guowangkeji.top/gtjcwewdev.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtwlizmmwb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtzpclvdjc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtknsmpihl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gogol.net.cn/gthmfjbosl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangkeji.top/gtdlpbwklj.html

Ruby: def greet(name = "World") = name
来源：http://hz.zycfv.cn/gtulohwzkf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jiagoushi.top/gtddgllamq.html

[C03] 可变参数
来源：http://hz.yj20258888.top/gtzdhuwfox.html

Py:   def total(*args): return sum(args)
来源：http://hz.cashguo.top/gtqhhkpsmc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtrrekeciw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtrbzglrmm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuanzx.com/gttxlieopc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aizwys.cn/gtwzeculle.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtzkmudslx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtryxslozl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgfzy.top/gtmqlmyuui.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pycfn.com/gtudfkfdmk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sufxvd.cn/gtzukmhwdb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nanxinkj.top/gtmqhxlpzu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtfjtohxxl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtsgsyqrar.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.kuanghao11.cn/gtffwjzrow.html

Go:   // 无：用配置结构体参数
来源：http://hz.9152youxi.cn/gthjxtvoxj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtgngpkiyq.html

C#:   f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtvpttudrd.html

[C05] 返回多个值
来源：http://hz.fzhhl.top/gtqniyvozj.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtstuegfir.html

PHP:  return [$a, $b];
来源：http://hz.yj20258.top/gtvjbjnxxj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxinkj.top/gtitgncrxm.html

TS:   return { a, b };
来源：http://hz.ydjk.org.cn/gtuihglbus.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jqgfzy.top/gtbbaosopp.html

Go:   return a, b
来源：http://hz.jiagoushi.top/gtpcdsitio.html

Ruby: return a, b
来源：http://hz.ywan-chungtsiang.top/gtkbmdaccn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gtcukxhohv.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtmlbctgkm.html

Py:   square = lambda x: x * x
来源：http://hz.tanke756.top/gtypojoahn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhengqikj.top/gtckovcrnp.html

JS:   const square = x => x * x;
来源：http://hz.ybcxt.top/gtetqqpgti.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhoulong.xyz/gtrzcrnkzc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yuanzhike.top/gtlfgqtywg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtzwcuojty.html

Ruby: square = ->(x) { x * x }
来源：http://hz.0kj1m.cn/gtnivgfffn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnxiangtu.top/gtauugssab.html

[C07] 把函数作为参数传入
来源：http://hz.sxryk.cn/gtsnykzrzy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tanke756.top/gtjewucthu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yueranfly.top/gtpzdqqsoy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ybcxt.top/gtgbhrqxwe.html

TS:   arr.map(String)
来源：http://hz.feifeiyinyue.top/gtpskoirds.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtfbdpurhi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhongyouzk.top/gtoxwntzum.html

Ruby: arr.map(&:upcase)
来源：http://hz.jyoumei.cn/gtoelkwzci.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtkcuilfra.html

[C08] 闭包
来源：http://hz.hysaishi.cn/gttgufdpie.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtbchaawqw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zdqjudy.top/gtfagnwmfl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtdfxxugaf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtwekgskhn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aibaodan.cn/gtnarviwsp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gtyemrpfrx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gtgwmyteco.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtndguafml.html

[C09] 递归
来源：http://hz.daria6918.cn/gtrgotacdy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtrdpelicz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtsauhfxqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtvpmkgfin.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtamxxdsgw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtlcdmxjyp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shuidangran.top/gtyceuithi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtttsldlwy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yanxiufei.cn/gtxjimnspr.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gtqftppici.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gtzssdxxeg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtolgtuicy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258.top/gtstotwybz.html

TS:   同 JS
来源：http://hz.andypj.xyz/gtyzcudknj.html

Java: 方法内为块级作用域
来源：http://hz.svipenyu.cn/gtkwjrodfk.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtemhmowyf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigufen.top/gtvmeivoog.html

C#:   块级作用域
来源：http://hz.guannengcc.top/gtjsrcjwqn.html

[C11] 模块导入与导出
来源：http://hz.ivvv.top/gtgsnnvcyn.html

Py:   from module import func
来源：http://hz.zhoulong.xyz/gtvfitysqq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtaifkglcl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenlongwang.top/gtwutzqxem.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.birdmap.top/gtbqgvmjuo.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gtrtjcmkvr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtdvbmvtag.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.vqdsnc.cn/gtbaonaqul.html

C#:   using System.Text;
来源：http://hz.gzhubu.top/gtbzyjovqh.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtamvfbsap.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtukwvbpgq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtpgnmsuaj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gthvqlhuik.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtsgxfzmil.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pycfn.com/gtblgopeor.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtfpzhtmky.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtcsnaivou.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenzaomai.com/gtddzvskfp.html

[C13] 类型声明 / 类型注解
来源：http://hz.aibaodan.cn/gtcsmkyknf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jiagoushi.top/gtcgcztepp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtucfjetms.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtzyyugxje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtigchoyqx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtfjolngfm.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtmbvfgswc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangshuangyany.cn/gtimplcqvv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yanxiufei.cn/gtmnxqouyj.html

[C14] 泛型函数
来源：http://hz.guannengcc.top/gtxubyrkqh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shuidangran.top/gtlyxneodi.html

PHP:  // 无泛型
来源：http://hz.redwolf501.top/gtxvuvnsvp.html

JS:   // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtpsolejsu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zycfv.cn/gtabsebzij.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtfudegqkj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yanxiufei.cn/gtmdleeoaf.html

Ruby: # 无泛型
来源：http://hz.jinghuilouyu.cn/gttseedhpe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.iojbl.cn/gtazytluxy.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtdjkjhzgx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shuidangran.top/gtlwzpcbzl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gturprewrl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.birdmap.top/gtzjnzwmqn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtikopdjap.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtgmpzfgnu.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gttlfrjlxe.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtbppsilav.html

C#:   var (a, b) = pair;
来源：http://hz.yj202588.top/gtmuimxcyg.html

[C16] 函数 / 方法重载
来源：http://hz.c1oappe.top/gtspmjdpox.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.iojbl.cn/gtslvwlogs.html

PHP:  // 无重载
来源：http://hz.jinqigfzy.top/gtwvwuautj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gtseiwqrzv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtnuowpkow.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gotoacloud.top/gtorcvujog.html

Go:   // 无重载：用不同函数名
来源：http://hz.vqdsnc.cn/gtsfkbzhsd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtcfszgacw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ppjwa.cn/gtddgqnuew.html

================================================================================
来源：http://hz.yvedp.cn/gtbozqzfnb.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtwxltoknj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtdkaolhox.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtomaajigr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenjidiqi.icu/gtywwgxids.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.haohaochexian.top/gtmggaelae.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtawsyavgq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtltusslhs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.vqdsnc.cn/gtsgenadag.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gteylkhuot.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtvahtetge.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.feifeiyinyue.top/gtjzsbjwke.html

[D02] 追加元素到末尾
来源：http://hz.yj20258888.top/gtevjcsqvo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxuanxn.top/gtcbrxgsmi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangkeji.top/gtndssfqis.html

JS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtsrmwyoau.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtgpkahnzs.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtnptepbas.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtxhrclije.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenjidiqi.icu/gtitozxjvm.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gtlrtfgvfe.html

[D03] 在指定位置插入元素
来源：http://hz.yangfankeji.com/gthorfsdoy.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtksipikgo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinyuanbaomall.cn/gthshshzwi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gttsthkhil.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtzxnfehga.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gteiuivunb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gthgqzmjld.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtkscggwrf.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gtrhtyggjp.html

[D04] 删除元素
来源：http://hz.nwbrower.top/gtlfeiirgm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtpoqnmbzk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sxryk.cn/gtchfdnnuf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj202588.top/gtjmjcgiqk.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtnknkqksi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yongpay.top/gtfkutlssr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuanzx.com/gtupvjuecf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hfpthk.cn/gtuzzlskft.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtnpubszfw.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gtbcdqxicb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtbjpvooac.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtuxillazl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sweek.top/gtjowgusmt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtwidzbcin.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtaepinydm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtquftkfjv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtcqmdtnyv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydzc1.top/gtdthuvenm.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtlnejvuvj.html

Py:   len(arr)
来源：http://hz.havefunace.top/gtratbzdmz.html

PHP:  count($arr);
来源：http://hz.zhaomingkeji.xyz/gtoefzbgup.html

JS:   arr.length
来源：http://hz.cheryme.top/gtxhdajhzw.html

TS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtmgurlnwo.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtdfawsvgj.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtjfotdbwk.html

Ruby: arr.length; arr.size
来源：http://hz.xuetiantiany.cn/gtuyfbeetm.html

C#:   list.Count;
来源：http://hz.wangshuangyany.cn/gtsnmfoppj.html

[D07] 切片 / 取子数组
来源：http://hz.jinyuanbaomall.cn/gtarzpgjmp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.iojbl.cn/gtkfyydehr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gteghecmne.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtjlnzlwsr.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtdcfgkxei.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gttlyqsmqn.html

Go:   arr[1:4]
来源：http://hz.zhixingplan.top/gtcifhlxqa.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtbwnqemtp.html

C#:   list.GetRange(1, 3);
来源：http://hz.fzhhl.top/gtxwdywoce.html

[D08] 合并两个数组
来源：http://hz.jianghu66.top/gtbakutgyi.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtaozpwqmc.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gtgxkzljgs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtpmyupuuq.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gtytzomzgk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtgbsdtlwa.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtzsupymvl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cheryme.top/gtrztjshom.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtuidvrllw.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtynebkrpj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtxtvuppid.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtyyzxyjfk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dashuyun.cn/gtwvinwyqd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtrlluiqzt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtyqwvxuco.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zycfv.cn/gtklnylwlw.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtrfegylia.html

C#:   list.Sort();
来源：http://hz.yuxming.cn/gtlcgpxzmw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gtfakoobpy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gteuzuusdg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtuveicksf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtysahjcbv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtdppcovhh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtnecybvsc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnqzz.top/gtjsqxlxjc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtlqwudhqi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gtgtcseplh.html

[D11] 反转数组
来源：http://hz.shuidangran.top/gtybrdpxed.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtlcqggpgk.html

PHP:  array_reverse($arr);
来源：http://hz.zycfv.cn/gtdlxjwida.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtxqmjuahp.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gttipuczzg.html

Java: Collections.reverse(list);
来源：http://hz.zhixingplan.top/gtbjdbtqje.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtrojmezkk.html

Ruby: arr.reverse
来源：http://hz.sxryk.cn/gtwfymqnss.html

C#:   list.Reverse();
来源：http://hz.hfpthk.cn/gtwmkmsxrs.html

[D12] 查找元素下标
来源：http://hz.zhongyouzk.top/gtfojovgwj.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gttfwvwwjd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenjidiqi.icu/gtneysppkp.html


<!-- 参考信息 -->