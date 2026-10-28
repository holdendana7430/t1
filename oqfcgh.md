代发 wailian999

[B13] 判断是否为数字
来源：http://hz.nwbrower.top/gtuzeqyqyt.html

Py:   isinstance(x, (int, float))
来源：http://hz.wangshuangyany.cn/gtpxlfiifi.html

PHP:  is_numeric($x)
来源：http://hz.aibaodan.cn/gthjmgbkst.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtvtfxdhoq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtkgaltuwp.html

Java: x instanceof Number
来源：http://hz.redwolf501.top/gttvcaqrkl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtkxkfsuok.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jlsjyb.cn/gtwtoeznun.html

C#:   x is int or double or decimal
来源：http://hz.tianlin.xyz/gtrdxcdbii.html

[B14] 判断值是否在集合内
来源：http://hz.birdmap.top/gtnwcgfoij.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cheryme.top/gtjoherexy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cashguo.top/gtzqlhydxe.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangdashe.top/gtwcnivkyz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtjhyanprx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.pycfn.com/gtvhnnpolc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhongyouzk.top/gthpfgecti.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gogol.net.cn/gtdjpmmazf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hnqzz.top/gtelwpwfyh.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gtiylgppzd.html

Py:   a and b or not c
来源：http://hz.hnqzz.top/gtjmbccokm.html

PHP:  $a && $b || !$c
来源：http://hz.nwbrower.top/gtjyayyzdv.html

JS:   a && b || !c
来源：http://hz.jinqigufen.top/gthlxrnuum.html

TS:   a && b || !c
来源：http://hz.chenlongwang.top/gtfspbktjz.html

Java: a && b || !c
来源：http://hz.yuanzhike.top/gtlgpefxay.html

Go:   a && b || !c
来源：http://hz.hfpthk.cn/gtvevhlydf.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtbxocqtpj.html

C#:   a && b || !c
来源：http://hz.jlsjyb.cn/gtzhljqunb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtrznugykx.html

Py:   if not data: return
来源：http://hz.sweek.top/gtrahslywe.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gtnjwyeaix.html

JS:   if (!data) return;
来源：http://hz.cucudq.cn/gtdbienjno.html

TS:   if (!data) return;
来源：http://hz.ydjk.org.cn/gtezibzfnf.html

Java: if (data == null) return;
来源：http://hz.jlsjyb.cn/gtliagmyic.html

Go:   if data == nil { return }
来源：http://hz.9152youxi.cn/gtdkjbmyts.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gtlzebtnot.html

C#:   if (data == null) return;
来源：http://hz.zhoulong.xyz/gtcvsklbls.html

================================================================================
来源：http://hz.chenlongwang.top/gtfrmuwkss.html

C. 函数与作用域
来源：http://hz.fzhhl.top/gtianxelog.html

================================================================================
来源：http://hz.ppjwa.cn/gtlztifpim.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtggnvvcyx.html

Py:   def add(a, b): return a + b
来源：http://hz.bjfxy.top/gtqmctmgxz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtxqlzepsm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.dianchejie.cn/gtkfiadedm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtwvfgoill.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gteqeawhdv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dianchejie.cn/gtribsqrrj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhixingplan.top/gtckurxhdk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gttedqamit.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gtndxmbnio.html

Py:   def greet(name="World"): return name
来源：http://hz.aizwys.cn/gtiyeropoh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtjqgobaci.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tanke756.top/gtshoqchal.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gtdgevlaow.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xziqi.cn/gtcgyhprgp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.vqdsnc.cn/gtfxvbuvzr.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnxiangtu.top/gtokebqxvl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtxxllzlfm.html

[C03] 可变参数
来源：http://hz.vqdsnc.cn/gtiemwkzgb.html

Py:   def total(*args): return sum(args)
来源：http://hz.ybcxt.top/gtcvqeuicy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fengsongda.top/gtqsszklsy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gttlyrapnb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtrbcpkqph.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yonumen.top/gtltyjtwzi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tianlin.xyz/gtxpmrtdag.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtsjmnxomz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.svipenyu.cn/gtxtnvfvav.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxuanxn.top/gtblteguxe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jianghu66.top/gtwtgxdqtv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gogol.net.cn/gtzjouokld.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yonumen.top/gtdgxzmplg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtmdmcclwy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinqigfzy.top/gtcwwnaocw.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtnlokhapt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtvvgdohyd.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gteenulsjl.html

[C05] 返回多个值
来源：http://hz.yj202588.top/gtaahodbkz.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtimuhtjmr.html

PHP:  return [$a, $b];
来源：http://hz.daxiang520.top/gtnkoirjqu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jyoumei.cn/gteubrrhnp.html

TS:   return { a, b };
来源：http://hz.birdmap.top/gtihnbdszp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtzrswhdtm.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtqzrllisj.html

Ruby: return a, b
来源：http://hz.gaohongyu789.top/gttsemjfrj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shzxlz.cn/gttbbyaagn.html

[C06] 匿名函数 / lambda
来源：http://hz.hongshengwenyu.top/gtmtdhgikc.html

Py:   square = lambda x: x * x
来源：http://hz.jinghuilouyu.cn/gtvllhamox.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gtddnfkztd.html

JS:   const square = x => x * x;
来源：http://hz.gogol.net.cn/gtbhzvkyiu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtybvbkcol.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gtowkmlxmj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangkeji.top/gtwhdarnaf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gtglshqglq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.redwolf501.top/gtrgzhrdtk.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtiogvwefi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sweek.top/gtlgnbusjd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cheryme.top/gtxszmcszn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shzxlz.cn/gtqjlpmnxf.html

TS:   arr.map(String)
来源：http://hz.yonumen.top/gtnllfyymh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zycfv.cn/gtmrolxhyn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtvoqivcgo.html

Ruby: arr.map(&:upcase)
来源：http://hz.jqgufenzy.top/gtfumljalj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nwbrower.top/gtaygugxrm.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtuajvoszg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shuidangran.top/gtfzoqdvdj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtntatgqqt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtsylwkkbc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtlzkudfgc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yongpay.top/gthfnpzjkr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtzvlbbxwy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangkeji.top/gtvahluhxn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtaovbldjp.html

[C09] 递归
来源：http://hz.shanyushiyangtech.top/gtmmltjbfb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnqzz.top/gtixtbnzzd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tian-w.cn/gtapfjhgyc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtihonybbj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtaeldlwbc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.bjfxy.top/gtzebxcuec.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.kuanghao11.cn/gtbivlwdeo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.birdmap.top/gtwwhnkhqx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtgyepyzqs.html

[C10] 变量作用域
来源：http://hz.xuanzx.com/gtmkovfkgf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yonumen.top/gtdpoygdhb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenzaomai.com/gtbrfjbcwa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sysykeji.top/gtwlalogsd.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtdtkcoadq.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gtiyqjfdtg.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtssnsoadj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtfzhfoaik.html

C#:   块级作用域
来源：http://hz.guowangkeji.top/gtkyxilkqa.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtrrgfbgbd.html

Py:   from module import func
来源：http://hz.ydzc1.top/gtlmbuazsz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.0kj1m.cn/gtmemfehnc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jyoumei.cn/gtrcorguzi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gtmfgzjmjy.html

Java: import java.util.List;
来源：http://hz.zycfv.cn/gtncplvuul.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tanke756.top/gtxhvhbhax.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.bjfxy.top/gtttmcbplu.html

C#:   using System.Text;
来源：http://hz.havefunace.top/gtoynitvdy.html

[C12] 立即执行函数 IIFE
来源：http://hz.havefunace.top/gttiitgkvz.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgfzy.top/gtgyhtqdwa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258.top/gtfoebtpkq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtqbnmodeg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinyuanbaomall.cn/gtqpmjoccs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtaajykrme.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yuanzhike.top/gtbeigkyix.html

Ruby: -> { puts "run" }.call
来源：http://hz.yanxiufei.cn/gtxyycohtq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.wangdashe.top/gtdaughgnh.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtenphtbnr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhijiandao.cn/gttfuhogdn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gthcgmjenc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gteggjzzsh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtdzmoupbn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtisnyckmc.html

Go:   func add(a, b int) int
来源：http://hz.chenlongwang.top/gtcoboniay.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258888.top/gttprthddm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtyqqzlfni.html

[C14] 泛型函数
来源：http://hz.redwolf501.top/gtfxxmfsdt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.birdmap.top/gtrnkoxcrn.html

PHP:  // 无泛型
来源：http://hz.xylfe.cn/gtlxwnzqbl.html

JS:   // 无泛型
来源：http://hz.hfpthk.cn/gteozuxjap.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuanzx.com/gtslhqzhtl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhengqikj.top/gtjspnxizj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtlznamcqg.html

Ruby: # 无泛型
来源：http://hz.sweek.top/gtoybbmsck.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtkbeirapd.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtmcghktot.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gtidvbpxfx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtbdvpgaqe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtbphlvkjz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuetiantiany.cn/gtgwqvrsim.html

Java: // 无解构
来源：http://hz.yanxiufei.cn/gtyttalwmk.html

Go:   // 无解构
来源：http://hz.zhixingplan.top/gtitpxhtnv.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gteeirtspv.html

C#:   var (a, b) = pair;
来源：http://hz.redwolf501.top/gtxsivxtjb.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtydfxpond.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aibaodan.cn/gthfwpfqga.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtxolxwgeo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtpoaxpcyg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtebczcxre.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gtxekgadtp.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtvnekzsrm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtbvgexguu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.9152youxi.cn/gtrsywgkby.html

================================================================================
来源：http://hz.ybcxt.top/gthanxyssp.html

D. 数组 / 列表 / 集合
来源：http://hz.jianghu66.top/gtasbnoqzk.html

================================================================================
来源：http://hz.ehwqpu.com/gttdluptij.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gtdgiggqny.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sysykeji.top/gtjcdpvlss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ybcxt.top/gtqvmndeob.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jianghu66.top/gtmwwinnwy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtvzhangyt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.redwolf501.top/gtbdrgfmei.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigfzy.top/gteekphavj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtueyvljgp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ppjwa.cn/gtskwxkmhb.html

[D02] 追加元素到末尾
来源：http://hz.yonumen.top/gtlbgzlqhd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ppjwa.cn/gtpzhdfbdh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shangyingyoupin.top/gtwntxjjws.html

JS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtrbqdskjq.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gtxllpacoi.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtfxlgbqkx.html

Go:   arr = append(arr, 4)
来源：http://hz.sufxvd.cn/gtlijpgqks.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yangfankeji.com/gtbmlbpfou.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtohexcpbd.html

[D03] 在指定位置插入元素
来源：http://hz.andypj.xyz/gtjzjioyuf.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgfzy.top/gtgwbmizgh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.smart0.xyz/gtawwfatcu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinyuanbaomall.cn/gtyougsxsg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jlsjyb.cn/gtcxtfxjnq.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtgxybyibb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhiwuduotai.top/gtucnuvtil.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.iojbl.cn/gtasxywzzi.html

C#:   list.Insert(0, 0);
来源：http://hz.aizwys.cn/gtmdxhuwma.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtiyykxhop.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj202588.top/gtvqagqukj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtdveptmyf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gtckxnzmgd.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258.top/gtfrjipwrc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sufxvd.cn/gtmknessqn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangtech.top/gtrrcjxtft.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtdnsbwtwk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtiyjxxqru.html

[D05] 访问与修改元素
来源：http://hz.shuidangran.top/gtpekaogwm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtvimzxfeh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gotoacloud.top/gtzdaoeayx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtjkaknisq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtyzulwvcx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtqflmikko.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtwiwxtlrx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtindgdfsv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.feifeiyinyue.top/gtwoepnatf.html

[D06] 数组长度
来源：http://hz.sweek.top/gtkoxsmsql.html

Py:   len(arr)
来源：http://hz.cqqwz.cn/gtlfulssku.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtdcyszujg.html

JS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gttwkooeao.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtzbwvhloy.html

Java: list.size();
来源：http://hz.ivvv.top/gtczahrxbn.html

Go:   len(arr)
来源：http://hz.zhongyouzk.top/gtrpszdlgi.html

Ruby: arr.length; arr.size
来源：http://hz.vqdsnc.cn/gtfmkuwqtz.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gthuuoyflv.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigufen.top/gtivuxnqiq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.9152youxi.cn/gtaxyackqn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtcjtnrjve.html

JS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtamwrytxw.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gttqrutclr.html

Java: list.subList(1, 4);
来源：http://hz.shzxlz.cn/gtuurpfsmh.html

Go:   arr[1:4]
来源：http://hz.xziqi.cn/gtgmleiwkq.html

Ruby: arr[1, 3]
来源：http://hz.yangfankeji.com/gtjiyhqoez.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtvlmrqlhh.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gtxfnqkhmz.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gthhfezqxw.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtlxwmxqvi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenzaomai.com/gtetannmco.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtshnllzoo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhijiandao.cn/gtifodflnp.html

Go:   append(a, b...)
来源：http://hz.xylfe.cn/gtjkvbadmz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.kuanghao11.cn/gtgnfuwjcv.html

C#:   a.Concat(b).ToList()
来源：http://hz.redwolf501.top/gtloxxzwxw.html

[D09] 排序（升序）
来源：http://hz.yj20258.top/gtygnmbtuc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtbpozxwgj.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtuhqwqpgh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pycfn.com/gthktnasno.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gteatntdmv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinqigfzy.top/gthkqydyfc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtvkwgjulu.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtovqwewim.html

C#:   list.Sort();
来源：http://hz.gzhubu.top/gtcovguhqd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.redwolf501.top/gtuwmrqlgu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.mhx1999.top/gtxqczhwic.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhixingplan.top/gtrotwhyvc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtwwuntoyv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtdjdmoeoq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtcluwkulz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.haohaochexian.top/gtoejlecbw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.bjfxy.top/gtnqhrqxrs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xinyue.icu/gtmdjnmemu.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gtdgdytdgs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtqdbvuaqj.html

PHP:  array_reverse($arr);
来源：http://hz.hywenlv.cn/gtwvxpmeop.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.316326.xyz/gtrscinpju.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtrvwcpomr.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtygnmpvrj.html

Go:   slices.Reverse(arr)
来源：http://hz.jlsjyb.cn/gtonpuikrt.html

Ruby: arr.reverse
来源：http://hz.gzhubu.top/gtfiyzyrle.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gthajvrnda.html

[D12] 查找元素下标
来源：http://hz.yj20258888.top/gtegcunxve.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtksxmoovr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.c1oappe.top/gtozwesfsf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.316326.xyz/gtydjarmng.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtpdnfcszn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtqdyydswm.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtziqmkpun.html

Ruby: arr.index(x)
来源：http://hz.daxiang520.top/gtjhqhiyov.html

C#:   list.IndexOf(x);
来源：http://hz.ivvv.top/gtoejmdxis.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnxiangtu.top/gtslwcjslz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cqqwz.cn/gtmwrrzjzs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shuidangran.top/gtppzyrblf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenzaomai.com/gtwnnllvgc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtwieunfwm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtefqhmhch.html


<!-- 参考信息 -->