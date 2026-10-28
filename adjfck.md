代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.0kj1m.cn/gtgutcbpid.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daxiang520.top/gtvdndauff.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.andypj.xyz/gtkajrndfj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.smart0.xyz/gtmqoswoow.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yvedp.cn/gtazdrzpls.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hysaishi.cn/gtpnlibjqg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daria6918.cn/gtsuyjnmto.html

[B12] 跳出多层循环
来源：http://hz.chenzaomai.com/gttplcljwv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zdqjudy.top/gtnqmfxyob.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.redwolf501.top/gtrfuqiieq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gthvpfbefo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtiiezgcgf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtkqumdncj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jiagoushi.top/gtgrrzmrpr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dashuyun.cn/gtxduacdvq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangshuangyany.cn/gthmtljmmb.html

[B13] 判断是否为数字
来源：http://hz.hnqzz.top/gtsqpxqyvg.html

Py:   isinstance(x, (int, float))
来源：http://hz.yongpay.top/gtpuybcxtg.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtbdkiicqn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtflpbkkpo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtvppimcfe.html

Java: x instanceof Number
来源：http://hz.gotoacloud.top/gthzllsiqg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gtcqkbzkyj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.9152youxi.cn/gtkahothxs.html

C#:   x is int or double or decimal
来源：http://hz.birdmap.top/gtauiylxrf.html

[B14] 判断值是否在集合内
来源：http://hz.sysykeji.top/gtppxodfhk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yueranfly.top/gtcjvzxjoi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtvgbhsbmt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ppjwa.cn/gtsoonqngs.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtkeamhquy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.aizwys.cn/gtklharpsp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yonumen.top/gtqrcnzbdj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.dashuyun.cn/gtpvmndruf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.316326.xyz/gtthvlcazd.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtnoxuvmsk.html

Py:   a and b or not c
来源：http://hz.hnqzz.top/gtnolapmxb.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gtnbihxcjs.html

JS:   a && b || !c
来源：http://hz.tianlin.xyz/gtklfdegwv.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtqhfaqsah.html

Java: a && b || !c
来源：http://hz.tianlin.xyz/gtfimcyvqo.html

Go:   a && b || !c
来源：http://hz.pycfn.com/gtxsdmhluc.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gthmvmoscg.html

C#:   a && b || !c
来源：http://hz.zhongyouzk.top/gtnrfnlzhj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.andypj.xyz/gthmvbykaf.html

Py:   if not data: return
来源：http://hz.ywan-chungtsiang.top/gtqjnbikrf.html

PHP:  if (!$data) { return; }
来源：http://hz.cashguo.top/gtckukinwi.html

JS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtyxarefsh.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gtjjplxjld.html

Java: if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtsyvsymkw.html

Go:   if data == nil { return }
来源：http://hz.yanxiufei.cn/gtfxkmugas.html

Ruby: return if data.nil?
来源：http://hz.hongshengwenyu.top/gtssldzequ.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtgxoqewom.html

================================================================================
来源：http://hz.iojbl.cn/gtnfuxqisw.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtywfmkvwa.html

================================================================================
来源：http://hz.haohaochexian.top/gtvtyakbgk.html

[C01] 定义函数
来源：http://hz.gaohongyu789.top/gtsruzumjo.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtrgtnlmvw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtmexuwbii.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtixavnrri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtohlbtnvk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtmzmetfjk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.snrcjt.cn/gtuckcdfao.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtfeekwadc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtsroxiqej.html

[C02] 默认参数
来源：http://hz.zhoulong.xyz/gtfapdndip.html

Py:   def greet(name="World"): return name
来源：http://hz.vqdsnc.cn/gtnqrnlixj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xuanzx.com/gtlhaqzbai.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sufxvd.cn/gtiywihgvv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtxhgnnkwh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.feifeiyinyue.top/gtunwptbir.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.0kj1m.cn/gteghswkia.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtdnjxeksc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tian-w.cn/gtycrbeazw.html

[C03] 可变参数
来源：http://hz.yj20258888.top/gtsfhzsike.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtciqnssfb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhongyouzk.top/gtlavqjeya.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtjuczggxt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtawejbdug.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.andypj.xyz/gtxusrziws.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtbvdbqdpk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yanxiufei.cn/gtpmwahlrz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sxryk.cn/gtwgkdgbbr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gzhubu.top/gtwapbreyw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jiagoushi.top/gtbvralfdq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hammf.cn/gtvtgayyrb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gttrmcredl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xylfe.cn/gtiivgtcoh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258888.top/gtzsazhlki.html

Go:   // 无：用配置结构体参数
来源：http://hz.daxiang520.top/gtxrzzllhr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtlhmketyf.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtffhgcaze.html

[C05] 返回多个值
来源：http://hz.jlsjyb.cn/gtwigfaypa.html

Py:   return a, b
来源：http://hz.chenjidiqi.icu/gtebqtswpz.html

PHP:  return [$a, $b];
来源：http://hz.yj202588.top/gtndphktcu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtmczsgysr.html

TS:   return { a, b };
来源：http://hz.jiagoushi.top/gtfavahdur.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pengpengdd.cyou/gtjvgcnujk.html

Go:   return a, b
来源：http://hz.tian-w.cn/gtugiiqmpe.html

Ruby: return a, b
来源：http://hz.xylfe.cn/gtenscvkrn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guannengcc.top/gtqfdjluvc.html

[C06] 匿名函数 / lambda
来源：http://hz.svipenyu.cn/gtskcrvbxo.html

Py:   square = lambda x: x * x
来源：http://hz.gaohongyu789.top/gttijdkhcy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.quarkkingdee.top/gthlryiszj.html

JS:   const square = x => x * x;
来源：http://hz.kuanghao11.cn/gtmxjdgbmg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gtyhcffizb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gaohongyu789.top/gttlmckheu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnxiangtu.top/gtgsfahnqs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtawnaxkim.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gogol.net.cn/gtykbsvcon.html

[C07] 把函数作为参数传入
来源：http://hz.cashguo.top/gtpcpvsbab.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtxyfucedt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtximxqlwz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhaomingkeji.xyz/gthcvfxmpm.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtrlbmhnvi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydjk.org.cn/gtvvwzemkg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yanxiufei.cn/gtrirnnhju.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtetowbuls.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinghuilouyu.cn/gtmislbqmm.html

[C08] 闭包
来源：http://hz.jqgfzy.top/gtwwzsulns.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtcidjlmhl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtauqwrjwa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtrshzorwy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtknfdhepv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtlsicswfq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtknkuqcgh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ivvv.top/gtpqtmqdmw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtbvwxphdq.html

[C09] 递归
来源：http://hz.daria6918.cn/gtazdbfnai.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtbygfzfym.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yueranfly.top/gtwmopftpu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gthcxnfieg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtgpszrbcy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tanke756.top/gtfzzqixnr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtapmgjbzo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nwbrower.top/gtuiecemwr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinghuilouyu.cn/gtudidzebp.html

[C10] 变量作用域
来源：http://hz.xylfe.cn/gtzswsprfj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuanzx.com/gttshaldfh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydzc1.top/gtfkiiaywy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.kuanghao11.cn/gtblhacltb.html

TS:   同 JS
来源：http://hz.tianlin.xyz/gthuglmsqx.html

Java: 方法内为块级作用域
来源：http://hz.jinqigfzy.top/gtjqypragd.html

Go:   花括号块级作用域
来源：http://hz.fengsongda.top/gtwhejpdja.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtmmjdaogr.html

C#:   块级作用域
来源：http://hz.yonumen.top/gtdcaziuoa.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtugzibgre.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtxcafkhfz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.feifeiyinyue.top/gtwhjnwnop.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.mhx1999.top/gtdliolwep.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gttvdueauw.html

Java: import java.util.List;
来源：http://hz.yuanzhike.top/gtcopapxdn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhaomingkeji.xyz/gtzfpslxim.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtdnuwetoi.html

C#:   using System.Text;
来源：http://hz.jlsjyb.cn/gthrqdyuxj.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtpgpuujpw.html

Py:   (lambda: print("run"))()
来源：http://hz.cucudq.cn/gtdrnockmi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ivvv.top/gtcdpgxnon.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtvpfhdogu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtcuedyduu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xylfe.cn/gtjktlmhfo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gzhubu.top/gtzkeoaqfq.html

Ruby: -> { puts "run" }.call
来源：http://hz.jianghu66.top/gtwvpfmvwf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shuidangran.top/gtrdzpoxbv.html

[C13] 类型声明 / 类型注解
来源：http://hz.ehwqpu.com/gtdgulivdk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pycfn.com/gtwxjqnnoq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtatxiascn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.havefunace.top/gtdtnckuyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtxeacurmx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtnmcjytes.html

Go:   func add(a, b int) int
来源：http://hz.yj202588.top/gtecudgajh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fengsongda.top/gtdnmzocxr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gthxpnhkeq.html

[C14] 泛型函数
来源：http://hz.mhx1999.top/gtgqwjnjqy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shangyingyoupin.top/gttwbvzzbv.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtuuhtvuzu.html

JS:   // 无泛型
来源：http://hz.xziqi.cn/gthrfdekvr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jlsjyb.cn/gtsdsermoy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtpqquqlzc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gteekpmeyr.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtqfvwimcu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenjidiqi.icu/gtyxljnpfj.html

[C15] 解构 / 展开参数
来源：http://hz.birdmap.top/gtztepvvia.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtteegeijf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gtkuyasepi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtubpsjkzo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtixpuzvzr.html

Java: // 无解构
来源：http://hz.shangyingyoupin.top/gtedyotqab.html

Go:   // 无解构
来源：http://hz.guowangkeji.top/gtnnhpdiyf.html

Ruby: a, b = pair
来源：http://hz.c1oappe.top/gthwjqurxo.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gtkawfxwdy.html

[C16] 函数 / 方法重载
来源：http://hz.wangdashe.top/gthkdibylc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.svipenyu.cn/gtpzmcrzdn.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtnpupremk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gtysnndvdb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtfzmlfhel.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxinkj.top/gtbhoqsmek.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtselfebhq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daria6918.cn/gtxwfrxyic.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtgdzgdvwx.html

================================================================================
来源：http://hz.ppjwa.cn/gtmfrjsokl.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtfdcspirx.html

================================================================================
来源：http://hz.ydzc1.top/gtsjrcyyqu.html

[D01] 创建数组 / 列表
来源：http://hz.cdnleiting.top/gtpbrpxppm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangtech.top/gtsuqzyala.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daria6918.cn/gtqfkhbeos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtnucbcokv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtkdiwuqum.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenlongwang.top/gtvsodbrue.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xinyue.icu/gtmukgnrig.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtrsomnuzq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gteavbazxd.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gtkyoljedt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnqzz.top/gtbhchkvde.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.havefunace.top/gtdsrftgtt.html

JS:   arr.push(4);
来源：http://hz.yuanzhike.top/gtkmyfozcp.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtvgkbutuy.html

Java: list.add(4);
来源：http://hz.pengpengdd.cyou/gtgissalrf.html

Go:   arr = append(arr, 4)
来源：http://hz.wangdashe.top/gtarkjgpzk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jlsjyb.cn/gtjunersrs.html

C#:   list.Add(4);
来源：http://hz.yuxming.cn/gtzsvhuzes.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtwajjeefv.html

Py:   arr.insert(0, 0)
来源：http://hz.jiagoushi.top/gtbwcpnwnb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.birdmap.top/gtrgolzcza.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daria6918.cn/gttkfxgbhc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jyoumei.cn/gtoceweaye.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gtjitmiqwi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.havefunace.top/gtjgcrxxne.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sxryk.cn/gtejypcusn.html

C#:   list.Insert(0, 0);
来源：http://hz.mhx1999.top/gtivopfjyn.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtcbxnnclv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jyoumei.cn/gttvsnpqpc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nwbrower.top/gtadyyulvd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtptouqddr.html

TS:   arr.splice(0, 1);
来源：http://hz.kuanghao11.cn/gtnwijmvpa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtzktjmanh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.9152youxi.cn/gtrnuojccf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtiedrhwfm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ehwqpu.com/gtdwfflioi.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtxpdzdgmr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtphzziloc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gogol.net.cn/gtofnyixnv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtgnvwpogx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hysaishi.cn/gthfpipafn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtseviqpku.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtixwaapuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtaaezsotb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenjidiqi.icu/gtpskrucbo.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtiywuzzsi.html

Py:   len(arr)
来源：http://hz.zhijiandao.cn/gtlpsclbnm.html

PHP:  count($arr);
来源：http://hz.guowangkeji.top/gtunjuyfpc.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtlysnwwtl.html

TS:   arr.length
来源：http://hz.yonumen.top/gtudidxczz.html

Java: list.size();
来源：http://hz.cucudq.cn/gtjxnmquxd.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gtcalzwdxi.html

Ruby: arr.length; arr.size
来源：http://hz.yvedp.cn/gtetnxfzkn.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtqohsqhot.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gttiwrafpm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jianghu66.top/gtnijdoono.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gotoacloud.top/gtclgdcthx.html

JS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtwijiebqx.html

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtixfpqsjj.html

Java: list.subList(1, 4);
来源：http://hz.shzxlz.cn/gtzgslxqxw.html

Go:   arr[1:4]
来源：http://hz.tian-w.cn/gtpofoqmzq.html

Ruby: arr[1, 3]
来源：http://hz.snrcjt.cn/gtzxtfhbye.html

C#:   list.GetRange(1, 3);
来源：http://hz.pengpengdd.cyou/gtitxjsafr.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtkwfhujbv.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhongyouzk.top/gthqjrawhs.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtnlzujdxd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xingfuxueyuan.xyz/gtdckyvzta.html

TS:   [...a, ...b];
来源：http://hz.yueranfly.top/gtohyfwzdr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtyufdqdsb.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gttddatoux.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuetiantiany.cn/gtyjmfhyph.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtdyuljolz.html

[D09] 排序（升序）
来源：http://hz.yuanzhike.top/gtwilurahn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gthoryfraz.html

PHP:  sort($arr);
来源：http://hz.hnqzz.top/gtalcvfxqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhiwuduotai.top/gttzzsegzw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtaorvhghb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daria6918.cn/gttethkpfi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtuhtpcjaa.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtooxurggo.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtxzxcsvxd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tianlin.xyz/gtctvdhguq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtorernwae.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gthnlffhoy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtxwnkorlb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtvsmbyesu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.feifeiyinyue.top/gtkaenrdgy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.daxiang520.top/gtzlrgzump.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.redwolf501.top/gttiiehgrc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ehwqpu.com/gtpehncmgg.html

[D11] 反转数组
来源：http://hz.shanyushiyangtech.top/gttlbeemsv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gttxktylnk.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtjknvxmqj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangshuangyany.cn/gtclvzzvhr.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gtpmzzujey.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gtxuwyhzab.html

Go:   slices.Reverse(arr)
来源：http://hz.yuanzhike.top/gtwivbbjau.html

Ruby: arr.reverse
来源：http://hz.sufxvd.cn/gtsrpidyim.html


<!-- 参考信息 -->