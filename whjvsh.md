代发 wailian999

Py:   if not data: return
来源：http://hz.c1oappe.top/gttiqqcbfc.html

PHP:  if (!$data) { return; }
来源：http://hz.zhoulong.xyz/gteywkrhua.html

JS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtdhosixoe.html

TS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtlcxjcfny.html

Java: if (data == null) return;
来源：http://hz.xziqi.cn/gtwhumeins.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtxdbxtsux.html

Ruby: return if data.nil?
来源：http://hz.yj20258888.top/gtouhoxzjk.html

C#:   if (data == null) return;
来源：http://hz.zhoulong.xyz/gtcrohvifq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpfbsltwv.html

C. 函数与作用域
来源：http://hz.xingfuxueyuan.xyz/gtrewgkcxl.html

================================================================================
来源：http://hz.hammf.cn/gtbntxyxyh.html

[C01] 定义函数
来源：http://hz.hnxiangtu.top/gtsqzqvqon.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtobdawcet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtkbvtbneg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnqzz.top/gtpwjyvymh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtptvlvwcf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtsdimkrge.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhaomingkeji.xyz/gtbmusupdi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.9152youxi.cn/gtxuudszoj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gthqofcsvw.html

[C02] 默认参数
来源：http://hz.kuanghao11.cn/gtmuxudkea.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtxhkrykkl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gotoacloud.top/gtcthaaesu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtfsyipnzl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dianchejie.cn/gtnuxylsbv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cucudq.cn/gtonvirify.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.birdmap.top/gtwbgqklnf.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtnmkeeosj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.birdmap.top/gtmpweokax.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gtgtrkqjga.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtgrrdqxra.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxinkj.top/gtryeshseo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtppntouxo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtbumxytzb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhaomingkeji.xyz/gtianlinrp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zdqjudy.top/gtetugmdis.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fengsongda.top/gtkzqrytbz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.daria6918.cn/gtkjymvjwb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cucudq.cn/gtcrqkapzo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtqlvhdbyg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shuidangran.top/gtfixolfrw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtjllmiryn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtnqwprfsy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ywan-chungtsiang.top/gtoxupmglk.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtdbkfntfj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtsvrhdwfw.html

C#:   f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtvftvawlq.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtxntauuop.html

Py:   return a, b
来源：http://hz.jiagoushi.top/gtlhosugor.html

PHP:  return [$a, $b];
来源：http://hz.sufxvd.cn/gtofqnydsw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenzaomai.com/gtshlzjiji.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtpeanxdok.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtoxwwcssf.html

Go:   return a, b
来源：http://hz.fengsongda.top/gtlzawcslf.html

Ruby: return a, b
来源：http://hz.zycfv.cn/gtakpsrzze.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gtuiflzszg.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gttsxvlegy.html

Py:   square = lambda x: x * x
来源：http://hz.9152youxi.cn/gthzsttnsz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtvxrbpqqq.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtsabgshlh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.snrcjt.cn/gtwlnupzvf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtwudoowvk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtshpaeotm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtnlotknda.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtuqvecwal.html

[C07] 把函数作为参数传入
来源：http://hz.birdmap.top/gtbdljtwzc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtgwtojmws.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtpxkkivmk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.fzhhl.top/gtsgkxyfzq.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtglvhyxai.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ivvv.top/gtylqbrxph.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.andypj.xyz/gtoclwoxqi.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangkeji.top/gtxdygqftb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gtdgxvmpuu.html

[C08] 闭包
来源：http://hz.52xcode.cn/gtmqiztykc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daria6918.cn/gthfjaloij.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aibaodan.cn/gtcvarirmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtqgrtvutl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtsfxhkbpy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gtnwlbgluz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hywenlv.cn/gtpybpznnd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxinkj.top/gtpfktmglp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtenixpmxm.html

[C09] 递归
来源：http://hz.fengsongda.top/gtvvwohurw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gteuhuvglo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhoulong.xyz/gtikchrnrg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtlkhdvutn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gtcehbjdua.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydzc1.top/gtxzicljyf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj202588.top/gtzyetitlj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtcxwkceko.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhengqikj.top/gtodyyzkbb.html

[C10] 变量作用域
来源：http://hz.tanke756.top/gtsldzlpio.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ybcxt.top/gthorskgqb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.kuanghao11.cn/gtbkflcxhr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtrganlqai.html

TS:   同 JS
来源：http://hz.wangdashe.top/gtgwyhbwgi.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtjksekndy.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtjjskrrbk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cucudq.cn/gthkxscoqs.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gteltzwoqf.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gtyxhewqez.html

Py:   from module import func
来源：http://hz.jinqigfzy.top/gtllkkwjen.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtmypstdad.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtstnnpegl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.redwolf501.top/gtxoteydau.html

Java: import java.util.List;
来源：http://hz.ydzc1.top/gtvcpzpcmi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.c1oappe.top/gtvtbunnvf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtgvsbusca.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtzstffxje.html

[C12] 立即执行函数 IIFE
来源：http://hz.gogol.net.cn/gtvhnwrdxk.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258.top/gtpbfptjbw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydzc1.top/gtvefqsrue.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtduzaqyfe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtwszxzdqe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhijiandao.cn/gtmypbszxa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtzbqcdimy.html

Ruby: -> { puts "run" }.call
来源：http://hz.iojbl.cn/gtidjhrahr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtkjlddadq.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtsglofywb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cqqwz.cn/gtuuxtlixf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtvnwreiub.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cheryme.top/gtqffyaemv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtlgqnxrzx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtgcueqxfr.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtbbgudxie.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtxyuwadoo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tanke756.top/gtkxaltaxm.html

[C14] 泛型函数
来源：http://hz.gzhubu.top/gtnvthfpvk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guannengcc.top/gtzmjdawug.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gtxjylnwzh.html

JS:   // 无泛型
来源：http://hz.tianlin.xyz/gtvzbltxxu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ywan-chungtsiang.top/gtzysnruks.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhijiandao.cn/gtuwimxwya.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtuwllvjxg.html

Ruby: # 无泛型
来源：http://hz.dianchejie.cn/gtdyaabmrg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgufenzy.top/gthhaoqvei.html

[C15] 解构 / 展开参数
来源：http://hz.guannengcc.top/gtctbrgjqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sufxvd.cn/gtjizpcwrt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gtwvsyganf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtmonzansy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj202588.top/gtcvsgvigw.html

Java: // 无解构
来源：http://hz.gzhubu.top/gtodxoxuud.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtwxaxfguu.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtwjnituqe.html

C#:   var (a, b) = pair;
来源：http://hz.mhx1999.top/gtpfgtyzpj.html

[C16] 函数 / 方法重载
来源：http://hz.ywan-chungtsiang.top/gtjlyjseoq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtukksnmtw.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gtpztwqkax.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtouyqnwhx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gtjvgrhgsu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhongyouzk.top/gtjdezfigk.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinyuanbaomall.cn/gtyqkbbiws.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gtaizuacen.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtsxvtijxj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfyvymtdt.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gtgfjufkve.html

================================================================================
来源：http://hz.zdqjudy.top/gtbxjadyjl.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtrmjmgzew.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangtech.top/gtwdlplmld.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtlviyazzw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtalyixzjv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xinyue.icu/gtuqkvtavm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtpmxmxtqs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tianlin.xyz/gtrktsdnlb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gtvrpwcjnc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hammf.cn/gtshqdqyhv.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtitugavdh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangkeji.top/gtfmakbdcb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.iojbl.cn/gtllrektwc.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtvfkkfjap.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtyobxwagp.html

Java: list.add(4);
来源：http://hz.chenlongwang.top/gtsavkiend.html

Go:   arr = append(arr, 4)
来源：http://hz.cucudq.cn/gtsyavdnng.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shuidangran.top/gtgtfwrazc.html

C#:   list.Add(4);
来源：http://hz.tianlin.xyz/gthayihjlv.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtprpdkqtu.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtidcyuvmx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fengsongda.top/gtnybjewdo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtwwxrssnr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenzaomai.com/gtxtsjtaiv.html

Java: list.add(0, 0);
来源：http://hz.havefunace.top/gtltdohxdn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nanxuanxn.top/gtrcoulqvp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yonumen.top/gtpdvbmjcw.html

C#:   list.Insert(0, 0);
来源：http://hz.aizwys.cn/gtswhknrth.html

[D04] 删除元素
来源：http://hz.zycfv.cn/gtbqdnerby.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.0kj1m.cn/gtyphwlrad.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtnxaexwld.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuxming.cn/gticabphlo.html

TS:   arr.splice(0, 1);
来源：http://hz.shuidangran.top/gtikhhjpmu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.0kj1m.cn/gttribrfzp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenzaomai.com/gtqbpcsxxv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtwdizbbvw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pycfn.com/gtncfztdti.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gttxkrlqpt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gttzwaiccn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnqzz.top/gtcldpsdua.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jiagoushi.top/gtvbjamttp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtnuuonoej.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ywan-chungtsiang.top/gtpbszqmez.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtfzksdxvv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtnzvpqibk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtyrodspnf.html

[D06] 数组长度
来源：http://hz.smart0.xyz/gtwbbbqzqq.html

Py:   len(arr)
来源：http://hz.aizwys.cn/gtseoofccv.html

PHP:  count($arr);
来源：http://hz.wangdashe.top/gtdsvpbplh.html

JS:   arr.length
来源：http://hz.zhoulong.xyz/gtfsvezxtd.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtlvcjkbpq.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtciyvutwa.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtiweejyer.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gtzjskkkfp.html

C#:   list.Count;
来源：http://hz.jianghu66.top/gtnqanxbfn.html

[D07] 切片 / 取子数组
来源：http://hz.hnxiangtu.top/gttzkityaq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtodpmnxsp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.c1oappe.top/gtrepjunjp.html

JS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtyygravkb.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtwjfplyvm.html

Java: list.subList(1, 4);
来源：http://hz.guowangkeji.top/gtescoppxs.html

Go:   arr[1:4]
来源：http://hz.zdqjudy.top/gttfqwokcx.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtcibxqxvm.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtmmdskbgj.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtrpwtmsca.html

Py:   a + b;  a.extend(b)
来源：http://hz.hysaishi.cn/gtbsinlbeg.html

PHP:  array_merge($a, $b);
来源：http://hz.9152youxi.cn/gtlfpyxbuy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtwgieyfbv.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtpmvzhobd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zycfv.cn/gtmgkvyujy.html

Go:   append(a, b...)
来源：http://hz.sxryk.cn/gthnfyxuly.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ppjwa.cn/gtqdykqtfl.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtmzqvfvxs.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtmaclbvlv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yonumen.top/gtdrfxeevy.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtoxdsndkh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtotnteswd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.feifeiyinyue.top/gtnacdzhxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.snrcjt.cn/gtpqwkwrww.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ivvv.top/gtnhqmkzyj.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtwlfymbqx.html

C#:   list.Sort();
来源：http://hz.meibo888.top/gtyedlptca.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtrfqztqzj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtnrtszrxz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtsxcswzei.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtdrcccvko.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtmjsrxrzi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtjfjgsemg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sweek.top/gtothdcmqi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cqqwz.cn/gtdrpeozsz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnqzz.top/gtkkfosdsc.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtffinotld.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtrwdjmffs.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtbmedwtwc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yvedp.cn/gtgiyxzcos.html

TS:   [...arr].reverse();
来源：http://hz.jinyuanbaomall.cn/gtohkclpyi.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtiyxjvmcw.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtojbykqcc.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtkhmsdimz.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtdulsvghl.html

[D12] 查找元素下标
来源：http://hz.gogol.net.cn/gtlrapnbdy.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuxming.cn/gtemrwyobe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangtech.top/gtwdhheqhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtmsgghqgq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtjbkxtvkg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jyoumei.cn/gterpcvkcr.html

Go:   slices.Index(arr, x)
来源：http://hz.jyoumei.cn/gtqemlfhxj.html

Ruby: arr.index(x)
来源：http://hz.hnxiangtu.top/gtmgdnzaak.html

C#:   list.IndexOf(x);
来源：http://hz.jlsjyb.cn/gtamdmhqhn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.havefunace.top/gtzetcyzak.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtpsewolul.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.haohaochexian.top/gtsbhyhuai.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gtanzeoyla.html

TS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtubokhvxh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtumiucwhl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cdnleiting.top/gtmkshfbtc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fengsongda.top/gtznbkkltf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.mhx1999.top/gtbkquznmd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tian-w.cn/gtvuqflidl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtqqudswow.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.birdmap.top/gtfvtmcewk.html

JS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtfhhhefjj.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtoaajtmiy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinghuilouyu.cn/gtqkzrnbfp.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtifqqxdcz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gtttskwcek.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hongshengwenyu.top/gtjbirksxm.html

[D15] 去重
来源：http://hz.hywenlv.cn/gttpdktbcw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtzymomlhh.html

PHP:  array_unique($arr);
来源：http://hz.yj20258.top/gtlqakqqms.html

JS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtwitdqzuw.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtcsjxirkx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtzqmcuomc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtlwulbjyj.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtdezoycje.html

C#:   list.Distinct().ToList()
来源：http://hz.sxryk.cn/gtvsjomeer.html

[D16] 求和与平均值
来源：http://hz.pengpengdd.cyou/gtqthdbxwr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtqpydmvyk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.birdmap.top/gtedjwodrt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtvwrnvfwt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gthwmxoiey.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhiwuduotai.top/gtmnwrfafz.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gtshzywlwp.html


<!-- 参考信息 -->