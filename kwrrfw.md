代发 wailian999

PHP:  $a && $b || !$c
来源：http://hz.yvedp.cn/gtkigcfdtl.html

JS:   a && b || !c
来源：http://hz.sysykeji.top/gtpycndajh.html

TS:   a && b || !c
来源：http://hz.sysykeji.top/gtrjxyxpey.html

Java: a && b || !c
来源：http://hz.guannengcc.top/gtftfrihca.html

Go:   a && b || !c
来源：http://hz.chenzaomai.com/gtrckuqzpp.html

Ruby: a && b || !c
来源：http://hz.guannengcc.top/gtcjgnmllc.html

C#:   a && b || !c
来源：http://hz.shuidangran.top/gtmrgpymje.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gotoacloud.top/gtqtjhvgxi.html

Py:   if not data: return
来源：http://hz.feifeiyinyue.top/gtfdzxulnk.html

PHP:  if (!$data) { return; }
来源：http://hz.c1oappe.top/gtyjdnfkfn.html

JS:   if (!data) return;
来源：http://hz.sxryk.cn/gtgdrlrztj.html

TS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtwmmykeyo.html

Java: if (data == null) return;
来源：http://hz.yuxming.cn/gthecycfys.html

Go:   if data == nil { return }
来源：http://hz.quarkkingdee.top/gtjqjcaknx.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtafnhavtg.html

C#:   if (data == null) return;
来源：http://hz.yongpay.top/gtuoqvnawc.html

================================================================================
来源：http://hz.aizwys.cn/gtlzbrgmwc.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gtdluqwwub.html

================================================================================
来源：http://hz.aibaodan.cn/gtvpiyfkun.html

[C01] 定义函数
来源：http://hz.xuanzx.com/gtjbrtmzwv.html

Py:   def add(a, b): return a + b
来源：http://hz.birdmap.top/gtmaokhdoz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtmrafdhsi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtpodfzsww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtzriydwbo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtzyzknmzt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jiagoushi.top/gtbgddzmdl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangtech.top/gtxboigpxq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtwctkgjsn.html

[C02] 默认参数
来源：http://hz.kuanghao11.cn/gtjlxubtft.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gttawrzkmh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jlsjyb.cn/gtxodlbiwd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtuzvlmcef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gtowzorvzd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtlpvryouu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.haohaochexian.top/gtrcgryxda.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gttkrsctle.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtkzmiechf.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtjhujzroq.html

Py:   def total(*args): return sum(args)
来源：http://hz.sysykeji.top/gtzfecyics.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cdnleiting.top/gtaypmjvrx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtttossrcr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtnnzyoyje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gtwxprqwaj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gzhubu.top/gthrcuxjqx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhiwuduotai.top/gtvbfzhira.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj202588.top/gtkrxartds.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cdnleiting.top/gtzsinzrnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yanxiufei.cn/gtmswsbhyi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xylfe.cn/gtghgcanwo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtkksxoedb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtqppizhks.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258.top/gtbtokqnny.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtxceunwgn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtowzntjyk.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtedbhdvnd.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtdkjuemxy.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtoajibwsq.html

PHP:  return [$a, $b];
来源：http://hz.andypj.xyz/gtxhogjegs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangshuangyany.cn/gtqjjmmdaz.html

TS:   return { a, b };
来源：http://hz.hongshengwenyu.top/gtmzadnavj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jyoumei.cn/gtpxzbybqb.html

Go:   return a, b
来源：http://hz.tianlin.xyz/gtzemnurle.html

Ruby: return a, b
来源：http://hz.cashguo.top/gttghtvmmn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gtxbrujbkq.html

[C06] 匿名函数 / lambda
来源：http://hz.hammf.cn/gtnuqtrhmg.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtznmpsguw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.9152youxi.cn/gtnnxggqzt.html

JS:   const square = x => x * x;
来源：http://hz.andypj.xyz/gtcrhldiso.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhengqikj.top/gtwgwtuoru.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.iojbl.cn/gtwwinyamj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yangfankeji.com/gtxjkzpxjl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.9152youxi.cn/gtsnbqnejd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.9152youxi.cn/gtphjkecym.html

[C07] 把函数作为参数传入
来源：http://hz.kuanghao11.cn/gtyftoldmm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtlxkwoikm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cdnleiting.top/gthbbhyaju.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.kuanghao11.cn/gtsjwhuhiq.html

TS:   arr.map(String)
来源：http://hz.hywenlv.cn/gtiouyywzn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guannengcc.top/gtavywcvjl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nwbrower.top/gttnrlzlxw.html

Ruby: arr.map(&:upcase)
来源：http://hz.svipenyu.cn/gtbaqgrwjy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xylfe.cn/gteluiitdq.html

[C08] 闭包
来源：http://hz.pycfn.com/gthdciydkq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangdashe.top/gtuwjnaflz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhixingplan.top/gthhmmqydr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtoqmikfxk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtvckbdzzn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtqiqcxhls.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gtcvletfql.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtbaywzocd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtjtyrtsrv.html

[C09] 递归
来源：http://hz.yuxming.cn/gtihrtymel.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cashguo.top/gtqpagwopi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258888.top/gtfqxvgwcl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtsvnbubie.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtaafkvbcq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nwbrower.top/gtvsbgubji.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gttxcaawso.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtjpftzhjs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sweek.top/gtuhffqwna.html

[C10] 变量作用域
来源：http://hz.gzhubu.top/gtdbgriqjh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gtjbckagbw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shuidangran.top/gtmhcvycdg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtaerwgwdy.html

TS:   同 JS
来源：http://hz.sysykeji.top/gtbzlgjuzo.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtmylcuilc.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtujnbwile.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigfzy.top/gtfwuowqzo.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtoolnwcjd.html

[C11] 模块导入与导出
来源：http://hz.fzhhl.top/gtuqzgnjxs.html

Py:   from module import func
来源：http://hz.yonumen.top/gtachieqrh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangdashe.top/gtevfcabhy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aibaodan.cn/gtjydovpqk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ehwqpu.com/gtdigsqaff.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gtdamxkyrd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj202588.top/gtervirewo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtevgdihhx.html

C#:   using System.Text;
来源：http://hz.shzxlz.cn/gtrvstlwsx.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtiecjykkd.html

Py:   (lambda: print("run"))()
来源：http://hz.chenlongwang.top/gtxtiiegro.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fengsongda.top/gtzeysygir.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtsnmyhmpd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtemkxauok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yongpay.top/gtfzvlneex.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnxiangtu.top/gtqjrnycqc.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtqtpsdagp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ybcxt.top/gtfbfkbvlb.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtcimpmyti.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.9152youxi.cn/gthsbtiqug.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtuowogsrf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gttbbnseij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gthpmjjabw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtpxwvlnhz.html

Go:   func add(a, b int) int
来源：http://hz.zdqjudy.top/gtdjtmouzr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ywan-chungtsiang.top/gtddjfozdo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zycfv.cn/gtzzogxlkz.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtmgkaybdo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtpwhpoetr.html

PHP:  // 无泛型
来源：http://hz.dashuyun.cn/gtxmwhkbzz.html

JS:   // 无泛型
来源：http://hz.zhengqikj.top/gtexqxmdwj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.bjfxy.top/gtlnzxuhgj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fzhhl.top/gtnpawyqkf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yongpay.top/gtaegryogk.html

Ruby: # 无泛型
来源：http://hz.52xcode.cn/gttmodvbxc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.quarkkingdee.top/gtxbuwzhru.html

[C15] 解构 / 展开参数
来源：http://hz.hnqzz.top/gtbifervqv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtlctuqsdu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenzaomai.com/gtiqibrqfw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtbtbvvobe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ywan-chungtsiang.top/gtnqvormbz.html

Java: // 无解构
来源：http://hz.tian-w.cn/gtznxvnjzs.html

Go:   // 无解构
来源：http://hz.316326.xyz/gtxfpojxlq.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gtzyofpisu.html

C#:   var (a, b) = pair;
来源：http://hz.guowangkeji.top/gtnxrbrhep.html

[C16] 函数 / 方法重载
来源：http://hz.wangdashe.top/gtjiisbxty.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtgetxivxo.html

PHP:  // 无重载
来源：http://hz.gogol.net.cn/gtioshzgxb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.quarkkingdee.top/gtnawxwmyd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gtdhdqeczn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxinkj.top/gtdcmgjaoc.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxinkj.top/gtwentszjw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhongyouzk.top/gtjldgslen.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtmwxksgyz.html

================================================================================
来源：http://hz.yuanzhike.top/gtfbmjkzxy.html

D. 数组 / 列表 / 集合
来源：http://hz.yj202588.top/gtfsafervt.html

================================================================================
来源：http://hz.shuidangran.top/gtpghmyjfn.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gtfsclrxea.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tanke756.top/gtfgmezilf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtnalukmky.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.mhx1999.top/gtaermuynx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtokeqkslf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cqqwz.cn/gtrrfaoxky.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gtccwinwwo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jiagoushi.top/gtmifrmrht.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtrwxgtnlt.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtcjfutwoi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtdohxjyfg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ydzc1.top/gtjghuzngn.html

JS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtexlgoufi.html

TS:   arr.push(4);
来源：http://hz.tian-w.cn/gtepaupdzb.html

Java: list.add(4);
来源：http://hz.mhx1999.top/gtbrriicsc.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtekfituau.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yonumen.top/gtszgsmnmw.html

C#:   list.Add(4);
来源：http://hz.andypj.xyz/gtyxionrbh.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtbifsqrzs.html

Py:   arr.insert(0, 0)
来源：http://hz.jianghu66.top/gtquhyjujd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fzhhl.top/gtijlbbobs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtitpststx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtlssrqxmp.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtaxukjsrt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtvhjqegig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xinyue.icu/gtokfvuojw.html

C#:   list.Insert(0, 0);
来源：http://hz.zdqjudy.top/gttdcxmacr.html

[D04] 删除元素
来源：http://hz.redwolf501.top/gtvbdwtpom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gotoacloud.top/gttbqwehly.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cashguo.top/gtgohzufnw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daxiang520.top/gtqynsmpkr.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtwhmgtejc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtkrdxgviq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ybcxt.top/gtmpnxwsth.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtkqgpgoby.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxuanxn.top/gtlzjvhnbr.html

[D05] 访问与修改元素
来源：http://hz.9152youxi.cn/gtxauposce.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtgusqxbif.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtygywwthc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtbrpmzanw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gzhubu.top/gtsrkeqvcl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hongshengwenyu.top/gtlkmwxshq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtxwnyxosd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtyiskziae.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daxiang520.top/gttwhommxd.html

[D06] 数组长度
来源：http://hz.jinqigfzy.top/gtlhougnkm.html

Py:   len(arr)
来源：http://hz.aizwys.cn/gtojmsghek.html

PHP:  count($arr);
来源：http://hz.sufxvd.cn/gtfcxffqis.html

JS:   arr.length
来源：http://hz.nwbrower.top/gtutmdlxyf.html

TS:   arr.length
来源：http://hz.chenlongwang.top/gtdedvuojn.html

Java: list.size();
来源：http://hz.guannengcc.top/gtyccqjvoh.html

Go:   len(arr)
来源：http://hz.cqqwz.cn/gtftylsdyr.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtusyeypbk.html

C#:   list.Count;
来源：http://hz.c1oappe.top/gttiwxzhxp.html

[D07] 切片 / 取子数组
来源：http://hz.yueranfly.top/gtshatfxso.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gtzlzeqxuk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtzvizsnxg.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtgzbhoumv.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtcurswzdd.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gtolhlawoo.html

Go:   arr[1:4]
来源：http://hz.nanxuanxn.top/gtnuijbqnn.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gthasykhiy.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtstpwssld.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtgovdxlsa.html

Py:   a + b;  a.extend(b)
来源：http://hz.svipenyu.cn/gtcihqiyzk.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gtpggnoyne.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.vqdsnc.cn/gtrsmsltml.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gtqlpvilfw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtpqmoypyu.html

Go:   append(a, b...)
来源：http://hz.jlsjyb.cn/gtwjnekmik.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangdashe.top/gtaejjkmmc.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydjk.org.cn/gtczfynbrj.html

[D09] 排序（升序）
来源：http://hz.hammf.cn/gttcvzdzoo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtneoloftc.html

PHP:  sort($arr);
来源：http://hz.wangdashe.top/gtmjviviwo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtywhpdbnz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xziqi.cn/gteiqjbbot.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yueranfly.top/gtzulfburl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtelmlhhys.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtdzjiyiiy.html

C#:   list.Sort();
来源：http://hz.cashguo.top/gttbqnimsw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cucudq.cn/gtopglngfg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gogol.net.cn/gtlqhfaybe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtrjkbqwml.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtazokcwpu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtjbkhrrnd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtswjdjloc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtrepqqzyo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangshuangyany.cn/gtwyimdgmf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.iojbl.cn/gtrlhvqbgr.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtjaawjxiy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cucudq.cn/gtngnpelgb.html

PHP:  array_reverse($arr);
来源：http://hz.hammf.cn/gttuzzsyvp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jqgufenzy.top/gtkxrisveq.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtiybxnsct.html

Java: Collections.reverse(list);
来源：http://hz.meibo888.top/gtrajkkybw.html

Go:   slices.Reverse(arr)
来源：http://hz.sxryk.cn/gtrmbnfyux.html

Ruby: arr.reverse
来源：http://hz.sweek.top/gtvrfvnjkw.html

C#:   list.Reverse();
来源：http://hz.yuanzhike.top/gtophbgmye.html

[D12] 查找元素下标
来源：http://hz.0kj1m.cn/gtlpveaicj.html

Py:   arr.index(x);  x in arr
来源：http://hz.shuidangran.top/gtwpaotrtv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zycfv.cn/gtpeuuewyq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtstrxucgy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtvejmuzlx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtlhyecmml.html

Go:   slices.Index(arr, x)
来源：http://hz.jiagoushi.top/gtzkgjcost.html

Ruby: arr.index(x)
来源：http://hz.hnxiangtu.top/gtxczbmjek.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gtxrbdwody.html

[D13] 过滤（保留满足条件的）
来源：http://hz.mhx1999.top/gtotarjkmn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gtxvsixsez.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydzc1.top/gtowlgdycx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtcraxtbom.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtydxcbaaf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gtaqhgvbrd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cdnleiting.top/gtzzxwiuxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtdzvdqbut.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gthhcypxgg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtiojbacom.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtfmvvdyxe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sufxvd.cn/gtohpnyess.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtaldxxomc.html

TS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtyhowmuhj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtaxmesggr.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtjaarpxor.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.iojbl.cn/gtwfuerkdi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtktqrjrqe.html

[D15] 去重
来源：http://hz.jiagoushi.top/gtyviyntrv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtospmjsyi.html

PHP:  array_unique($arr);
来源：http://hz.birdmap.top/gtnkvexmln.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtguvrdwju.html

TS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtxogzzklv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangshuangyany.cn/gtndnrxvfg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtnzkrvuuq.html

Ruby: arr.uniq
来源：http://hz.gotoacloud.top/gteqlvferi.html


<!-- 参考信息 -->