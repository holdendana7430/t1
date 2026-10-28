代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.gzhubu.top/gtquwybype.html

[B14] 判断值是否在集合内
来源：http://hz.yueranfly.top/gtbrmybusy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gthfliceny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj202588.top/gtntshnudj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gteyhwdjjs.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zdqjudy.top/gtyqqjrdzv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydjk.org.cn/gtbervnsys.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tian-w.cn/gtgufrcyqf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shuidangran.top/gtlepyqhqf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.c1oappe.top/gtcvzmttou.html

[B15] 布尔运算与取反
来源：http://hz.zhijiandao.cn/gtcoxrokjo.html

Py:   a and b or not c
来源：http://hz.jinghuilouyu.cn/gtxbiuhtkc.html

PHP:  $a && $b || !$c
来源：http://hz.daria6918.cn/gtgmuznull.html

JS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtfkqjabwo.html

TS:   a && b || !c
来源：http://hz.zhixingplan.top/gtdgytdxdl.html

Java: a && b || !c
来源：http://hz.zhongyouzk.top/gtwfyekgac.html

Go:   a && b || !c
来源：http://hz.ehwqpu.com/gtkiuxetjr.html

Ruby: a && b || !c
来源：http://hz.jqgufenzy.top/gtzxljwkdx.html

C#:   a && b || !c
来源：http://hz.jqgufenzy.top/gtwttpidpt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.birdmap.top/gtlyezozak.html

Py:   if not data: return
来源：http://hz.jqgufenzy.top/gtmskywfkc.html

PHP:  if (!$data) { return; }
来源：http://hz.tianlin.xyz/gtncqqrwro.html

JS:   if (!data) return;
来源：http://hz.zycfv.cn/gtcpkjdufm.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtlgkwlefs.html

Java: if (data == null) return;
来源：http://hz.pengpengdd.cyou/gthkqfmjje.html

Go:   if data == nil { return }
来源：http://hz.cqqwz.cn/gtpmmiwcxi.html

Ruby: return if data.nil?
来源：http://hz.bjfxy.top/gtkohtdvvt.html

C#:   if (data == null) return;
来源：http://hz.hammf.cn/gtyxmkxzra.html

================================================================================
来源：http://hz.aibaodan.cn/gtqwpgtepk.html

C. 函数与作用域
来源：http://hz.yj20258888.top/gtqihptqow.html

================================================================================
来源：http://hz.smart0.xyz/gtqvfnmwkw.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtsotqsept.html

Py:   def add(a, b): return a + b
来源：http://hz.0kj1m.cn/gticfxkney.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gteqvdwsdi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gtmleqpvsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtvlzptjdf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtkoprekvu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtpzwqvwvr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hongshengwenyu.top/gtaacszjjf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtozpatzbz.html

[C02] 默认参数
来源：http://hz.jinghuilouyu.cn/gtkgqbtlsq.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtzfivltvs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xylfe.cn/gtmaupyxcr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtvbbzwgxs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtcffueugu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhaomingkeji.xyz/gtmdbdvtdv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gogol.net.cn/gtvxfylkmx.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydjk.org.cn/gtvcawiecx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinghuilouyu.cn/gtfsswjinf.html

[C03] 可变参数
来源：http://hz.snrcjt.cn/gtysjwqdqi.html

Py:   def total(*args): return sum(args)
来源：http://hz.316326.xyz/gtpzrbwtkr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtqfcvobul.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtjhfxjvic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gthszlkjvv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258888.top/gtyxipjqxp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhongyouzk.top/gtyqzqgqir.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.c1oappe.top/gtflstmlcb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.kuanghao11.cn/gtrezlqhsc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnxiangtu.top/gtroqiipyv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jianghu66.top/gtpqzzflar.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fengsongda.top/gtjqxmdehh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtyigoffvv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtzthvxtwi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtnfqarjfv.html

Go:   // 无：用配置结构体参数
来源：http://hz.xingfuxueyuan.xyz/gtclegsxax.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daxiang520.top/gttoxyaokw.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gttapqsqdi.html

[C05] 返回多个值
来源：http://hz.hnxiangtu.top/gtongegwub.html

Py:   return a, b
来源：http://hz.jinghuilouyu.cn/gttkhcytid.html

PHP:  return [$a, $b];
来源：http://hz.chenjidiqi.icu/gtvznwoprk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtujmjhtmx.html

TS:   return { a, b };
来源：http://hz.c1oappe.top/gtjtegenan.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hongshengwenyu.top/gtorkegsvh.html

Go:   return a, b
来源：http://hz.0kj1m.cn/gtwlkmhzon.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtxysxqqjz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtbmxytswg.html

[C06] 匿名函数 / lambda
来源：http://hz.yj20258.top/gtltbicgwf.html

Py:   square = lambda x: x * x
来源：http://hz.gaohongyu789.top/gthmzrcsph.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtdilsyvlh.html

JS:   const square = x => x * x;
来源：http://hz.hywenlv.cn/gtmqikazge.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenzaomai.com/gtbtpisimz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ppjwa.cn/gtccqsibcu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258888.top/gtolmeboyd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtbijlxmsy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gthainjtub.html

[C07] 把函数作为参数传入
来源：http://hz.zhengqikj.top/gtpxxoqusn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hnqzz.top/gtluaekzww.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yangfankeji.com/gtelppvmai.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtwntlnaau.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtadypuuac.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gttzkifpmx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gtkijjejrb.html

Ruby: arr.map(&:upcase)
来源：http://hz.yangfankeji.com/gtljexkdtv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guowangkeji.top/gtqrhhmosq.html

[C08] 闭包
来源：http://hz.andypj.xyz/gtghspxqce.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhaomingkeji.xyz/gttvlcbqpp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hongshengwenyu.top/gtrmburcuc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtycorhapv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtdugrxkfm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258888.top/gtrdujccyg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.havefunace.top/gtmdbcsxxc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dianchejie.cn/gthjyydglz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtkuaruxbs.html

[C09] 递归
来源：http://hz.redwolf501.top/gtkcnxvncj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtkjnksrrf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hfpthk.cn/gtgyrkfrsb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtinjeqoor.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtrfohndal.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtzdekvzxh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pengpengdd.cyou/gtfcbunvpl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtdyxvlgqc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtfbqcvcja.html

[C10] 变量作用域
来源：http://hz.dianchejie.cn/gtsfolxvfe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangtech.top/gtjwxhsllv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gttovdfzwm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.c1oappe.top/gthnuxpaud.html

TS:   同 JS
来源：http://hz.tian-w.cn/gtsdtalnjy.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtgomtidnk.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtturgxtfu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ehwqpu.com/gtydfkmtbr.html

C#:   块级作用域
来源：http://hz.ybcxt.top/gtejslovur.html

[C11] 模块导入与导出
来源：http://hz.cqqwz.cn/gtaqrqtdjc.html

Py:   from module import func
来源：http://hz.shanyushiyangtech.top/gtuiteliht.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydzc1.top/gtacyajlvs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtwpowgaxt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jlsjyb.cn/gtusyoobgs.html

Java: import java.util.List;
来源：http://hz.chenlongwang.top/gtwbvcqrkm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ywan-chungtsiang.top/gtiieycqem.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtaudfmihb.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtxsncxyxg.html

[C12] 立即执行函数 IIFE
来源：http://hz.hammf.cn/gteukotdha.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258.top/gtcxjwykcj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gtvqoetchb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtlmnfizrs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.feifeiyinyue.top/gtomtrxapg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shuidangran.top/gtnhnwjztm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daria6918.cn/gtvoissago.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangtech.top/gtbzhzxknv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnqzz.top/gtrppuocoi.html

[C13] 类型声明 / 类型注解
来源：http://hz.smart0.xyz/gtatxbmeqe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtdqelbkav.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtqyrbmmuq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ydzc1.top/gtnkupxwjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtvufwtyow.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtnmvnsgub.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gthcojuxhg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangshuangyany.cn/gtxrkkzbcy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258888.top/gtjaeibabb.html

[C14] 泛型函数
来源：http://hz.fengsongda.top/gtblnnwxbn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtjqjndocb.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtfrxkwelm.html

JS:   // 无泛型
来源：http://hz.cashguo.top/gtinvffzdx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gogol.net.cn/gtivbkbzzi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtcypjhfdl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aibaodan.cn/gtezxyojju.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gtjpauwpvh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gtxwodlzzg.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtndvwsjds.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jlsjyb.cn/gtcoouxmwh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuetiantiany.cn/gtbvlasenl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtgqkulrxx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtnrgkqvng.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtxfskhfoy.html

Go:   // 无解构
来源：http://hz.gotoacloud.top/gtbtbdqemn.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangkeji.top/gtzcfnqcqp.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gtnbxviwbf.html

[C16] 函数 / 方法重载
来源：http://hz.0kj1m.cn/gttxppqgte.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gtjkykvemh.html

PHP:  // 无重载
来源：http://hz.fzhhl.top/gtweadrpex.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gttgilslir.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fzhhl.top/gtoqkshvor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnxiangtu.top/gtjjqhzovu.html

Go:   // 无重载：用不同函数名
来源：http://hz.gaohongyu789.top/gtadajjeca.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtuoczembu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gotoacloud.top/gtocwanbkm.html

================================================================================
来源：http://hz.ybcxt.top/gthbfdjiho.html

D. 数组 / 列表 / 集合
来源：http://hz.xuetiantiany.cn/gtayzdquid.html

================================================================================
来源：http://hz.iojbl.cn/gtswkyeltf.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtgelbkihv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtzjpwtpjv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtacmbstgt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daria6918.cn/gtthnoucdi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gtbjehawat.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtrdqezibv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gttcooqnxv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hammf.cn/gttdozgfav.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtakvdlxcz.html

[D02] 追加元素到末尾
来源：http://hz.9152youxi.cn/gtiiwbylol.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zdqjudy.top/gtagirtucn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zycfv.cn/gtwzswqgvo.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtkbvbkxsb.html

TS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtzsibggng.html

Java: list.add(4);
来源：http://hz.svipenyu.cn/gtzvcjpeza.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtnxdlvvqe.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnqzz.top/gtcrqmnywx.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtxprxzrvs.html

[D03] 在指定位置插入元素
来源：http://hz.guannengcc.top/gtxunnylju.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtwznjlelf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.kuanghao11.cn/gtsnftgkru.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gtvjhogavr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gtywerugzf.html

Java: list.add(0, 0);
来源：http://hz.jinqigufen.top/gtopigjprs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtznitifmu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtbxgdldcy.html

C#:   list.Insert(0, 0);
来源：http://hz.fzhhl.top/gtstggzrpp.html

[D04] 删除元素
来源：http://hz.wangshuangyany.cn/gtemlpazga.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtgkycbyvy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cdnleiting.top/gtrnkqbyiw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtaqzwxjvp.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gthmzeciiq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yvedp.cn/gtdkbptgfh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gtkkexhedy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtuwpywoym.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtwgugfihe.html

[D05] 访问与修改元素
来源：http://hz.smart0.xyz/gtdntrlbyv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtkcacsirp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nwbrower.top/gtipcuhblr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gtemaqgcmb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zdqjudy.top/gtokodglrm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.dashuyun.cn/gtkqjgafjb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtkffbuenk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtowiirckb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenjidiqi.icu/gtxvgyzktk.html

[D06] 数组长度
来源：http://hz.nwbrower.top/gtukqqsiwp.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtmengerys.html

PHP:  count($arr);
来源：http://hz.dashuyun.cn/gtdadwqwhw.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtqzqlvxmn.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtububpjxw.html

Java: list.size();
来源：http://hz.cucudq.cn/gtcynnydnn.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtppvqwvqn.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtayiegctc.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtrxpdjskq.html

[D07] 切片 / 取子数组
来源：http://hz.zdqjudy.top/gtmxwjhhlo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gtxzveghoc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxinkj.top/gtfihkobes.html

JS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtxcifgtjq.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtpgpqhatt.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtdixjjvci.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gtlemmppum.html

Ruby: arr[1, 3]
来源：http://hz.hongshengwenyu.top/gtgvoperyt.html

C#:   list.GetRange(1, 3);
来源：http://hz.sufxvd.cn/gtolwforwr.html

[D08] 合并两个数组
来源：http://hz.pengpengdd.cyou/gtunggyxli.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtbtspfqmd.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtbbhjleny.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gtvjsibshi.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtaclmxnka.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xziqi.cn/gtjtenmbcr.html

Go:   append(a, b...)
来源：http://hz.hfpthk.cn/gtfoluuzrg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtacbwdmqd.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gttzsoxxic.html

[D09] 排序（升序）
来源：http://hz.zhoulong.xyz/gthxuctcxa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtzterpetn.html

PHP:  sort($arr);
来源：http://hz.zhiwuduotai.top/gtsgvnbpfz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtkirzvssh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gtqcebkryh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.birdmap.top/gtuxahodgm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ivvv.top/gtmsvdejkw.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtqggxsepf.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gtlgssvkez.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guowangkeji.top/gtwxhjwfre.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hysaishi.cn/gthroiazdm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gthrvbhdld.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtdajsjuud.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtqzpqrnqa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtakkybptn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sweek.top/gtgagaikxa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtlbwcaebg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangkeji.top/gtuvakgkyi.html

[D11] 反转数组
来源：http://hz.fengsongda.top/gtjqvyhsxj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.9152youxi.cn/gtbgkmzwrn.html

PHP:  array_reverse($arr);
来源：http://hz.52xcode.cn/gtnlmafnyd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtsktlxova.html

TS:   [...arr].reverse();
来源：http://hz.sweek.top/gtqmtenumd.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtfapuffay.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxuanxn.top/gtfdbnwixd.html

Ruby: arr.reverse
来源：http://hz.svipenyu.cn/gtlpdhxhfq.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangtech.top/gtjjydabna.html

[D12] 查找元素下标
来源：http://hz.ywan-chungtsiang.top/gtetxclhmi.html

Py:   arr.index(x);  x in arr
来源：http://hz.nwbrower.top/gtrkysdhvc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.bjfxy.top/gtvnczajca.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtsrlxukva.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtonxohzje.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtcpiwxfom.html

Go:   slices.Index(arr, x)
来源：http://hz.shangyingyoupin.top/gtiejtvemt.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gthffgmost.html

C#:   list.IndexOf(x);
来源：http://hz.fengsongda.top/gtlfkdyymk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtbujonfwa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.birdmap.top/gtbzzlaqhu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangkeji.top/gtozyoiwbz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtokrntxxh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtgfodibrh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gttwxzexeg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gtwtupcnbe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cheryme.top/gtwmdimdtp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtnjigexxv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gtdycsxqbf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenjidiqi.icu/gtqmypcytu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtllnginwx.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtqqpbwdaf.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtmaeuqcop.html


<!-- 参考信息 -->