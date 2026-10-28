代发 wailian999

Py:   if not data: return
来源：http://hz.sweek.top/gtsjrfjuvl.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtqbybokqg.html

JS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtgljljzom.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtzxewcpob.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gtudutcnoe.html

Go:   if data == nil { return }
来源：http://hz.wangshuangyany.cn/gtqeydzplv.html

Ruby: return if data.nil?
来源：http://hz.yj20258.top/gtnzxtvclh.html

C#:   if (data == null) return;
来源：http://hz.hfpthk.cn/gtlzwwjtfv.html

================================================================================
来源：http://hz.birdmap.top/gtybbppfbl.html

C. 函数与作用域
来源：http://hz.jqgufenzy.top/gtbrxtalkv.html

================================================================================
来源：http://hz.gzhubu.top/gtxowmzqpf.html

[C01] 定义函数
来源：http://hz.fzhhl.top/gtlhtwzimr.html

Py:   def add(a, b): return a + b
来源：http://hz.wangshuangyany.cn/gtdxtheunn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtpljekgup.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jyoumei.cn/gtxwdojiok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtknjziymm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtfycxhmgn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fengsongda.top/gtbgzgklqq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtievatynx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtlvpcnmsj.html

[C02] 默认参数
来源：http://hz.jyoumei.cn/gtbwaftrda.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gtgkunigir.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yonumen.top/gtkhvqjbos.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.c1oappe.top/gtsqblkyle.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gthvdndevr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.quarkkingdee.top/gtsrhfcehp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zdqjudy.top/gtkgqagbqe.html

Ruby: def greet(name = "World") = name
来源：http://hz.quarkkingdee.top/gtimshmkud.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinyuanbaomall.cn/gthppgterc.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gtdltkaiyf.html

Py:   def total(*args): return sum(args)
来源：http://hz.hnxiangtu.top/gtcebdelbb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtwbavphkc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtemfkcnxh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gttnwnqvfl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtphlklyxz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fengsongda.top/gtnoveywhb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.redwolf501.top/gtdaesswgg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtgbfzpdtw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtlgbyilou.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtmrzvepsu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.9152youxi.cn/gtjbbwesex.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hammf.cn/gtmznggryn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtntzvigvs.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.smart0.xyz/gtsccbilki.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gttpgvkkwt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtdtznecej.html

C#:   f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtkcxorpui.html

[C05] 返回多个值
来源：http://hz.jinqigfzy.top/gtbvnvdpjy.html

Py:   return a, b
来源：http://hz.yonumen.top/gtofslhhyy.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtlofsshpa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.birdmap.top/gtwvzxkezy.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtfsifppwg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxinkj.top/gthjpxhyak.html

Go:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtignbzxgn.html

Ruby: return a, b
来源：http://hz.hongshengwenyu.top/gtvpqlxikb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtskjylvty.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtypsonqen.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtyblsypqs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nwbrower.top/gtrxiuehnv.html

JS:   const square = x => x * x;
来源：http://hz.daria6918.cn/gtehoxacps.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.bjfxy.top/gtozqjjtuk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtmeupjyqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgufenzy.top/gtaqrddeyy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gtpagiwdah.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sysykeji.top/gtloyjidgj.html

[C07] 把函数作为参数传入
来源：http://hz.wangshuangyany.cn/gttzrrieqm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gaohongyu789.top/gtnmmebgaw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sweek.top/gthkudthrq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yueranfly.top/gtxvxcincw.html

TS:   arr.map(String)
来源：http://hz.yj20258888.top/gtmdmsnige.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xingfuxueyuan.xyz/gtvomywubm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtcbpeelub.html

Ruby: arr.map(&:upcase)
来源：http://hz.jlsjyb.cn/gtwbcperxe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dianchejie.cn/gtkslkohqg.html

[C08] 闭包
来源：http://hz.ivvv.top/gtzhnectsz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sxryk.cn/gtspnyuuzp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sxryk.cn/gtxfycdtrx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtnmbmsgoj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtybipduur.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.snrcjt.cn/gtdwywebmy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258888.top/gtoqzjxdkk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.c1oappe.top/gtqdffievt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtnqlagzie.html

[C09] 递归
来源：http://hz.yvedp.cn/gtykbydpyk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtjyryaqie.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.svipenyu.cn/gtosiiziwc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtmikfxsus.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gteldekbsa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtxterbnwv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtlmmvyqvk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtfjaovxpa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangshuangyany.cn/gteohsghel.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtjufnvwsz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.wangdashe.top/gtqhaeppjg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj202588.top/gtixwmaeqk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jlsjyb.cn/gteiunenrp.html

TS:   同 JS
来源：http://hz.jinqigfzy.top/gtguywpwdc.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtqfbqmcps.html

Go:   花括号块级作用域
来源：http://hz.zhixingplan.top/gtfjlekhpx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtstccqdak.html

C#:   块级作用域
来源：http://hz.hongshengwenyu.top/gtspkaoydd.html

[C11] 模块导入与导出
来源：http://hz.shangyingyoupin.top/gtortvhxpq.html

Py:   from module import func
来源：http://hz.ywan-chungtsiang.top/gtmonxmrcd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenlongwang.top/gtlcoqiasx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nanxinkj.top/gtlcewpwqq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fzhhl.top/gtivbvybkh.html

Java: import java.util.List;
来源：http://hz.jinqigufen.top/gtfjdaxhcp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cdnleiting.top/gtxjngtwsv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuanzhike.top/gtqyegzqsd.html

C#:   using System.Text;
来源：http://hz.316326.xyz/gteinbnqzp.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtgcfppayh.html

Py:   (lambda: print("run"))()
来源：http://hz.tanke756.top/gtvagfkoyx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xinyue.icu/gtmkettwlx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtstdfyzsy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtogtgebie.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangshuangyany.cn/gtwrckmzrh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ywan-chungtsiang.top/gthwxvlfyf.html

Ruby: -> { puts "run" }.call
来源：http://hz.pycfn.com/gtvbplydus.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.mhx1999.top/gtduhpdela.html

[C13] 类型声明 / 类型注解
来源：http://hz.sufxvd.cn/gtidfmtdye.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtndjdivyk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtcwkjepsc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jlsjyb.cn/gtmbacpigm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gthmvrsjij.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtihxpyjlg.html

Go:   func add(a, b int) int
来源：http://hz.jinqigufen.top/gtpudlzkpp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258888.top/gtojjmypxg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgufenzy.top/gtcamxfmst.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtepgzjqab.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hywenlv.cn/gtgmkxrvwe.html

PHP:  // 无泛型
来源：http://hz.yueranfly.top/gtfukkmhnx.html

JS:   // 无泛型
来源：http://hz.gaohongyu789.top/gtqawrbxos.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydzc1.top/gtxaylotwy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.iojbl.cn/gtmpzgmfyb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtewfqdozb.html

Ruby: # 无泛型
来源：http://hz.fzhhl.top/gtkqtpxjwe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.meibo888.top/gtonxqgben.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtfrlnuqtd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtvsxdnvrr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtmngvsdrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtctomdwdz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.meibo888.top/gtltmsmedb.html

Java: // 无解构
来源：http://hz.jlsjyb.cn/gtjiokpbkm.html

Go:   // 无解构
来源：http://hz.haohaochexian.top/gtxcpeitoz.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtekyktvof.html

C#:   var (a, b) = pair;
来源：http://hz.hnxiangtu.top/gtoxqlqwyx.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtmyxfbabt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtzqpgthmv.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtihpvmlvc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtkzrwxrrr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jiagoushi.top/gtfvcldqkg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.quarkkingdee.top/gtvwctqsyh.html

Go:   // 无重载：用不同函数名
来源：http://hz.ybcxt.top/gtlanwyvru.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtuitlfavm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gtaglnrper.html

================================================================================
来源：http://hz.c1oappe.top/gtrolmsafz.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtofquufak.html

================================================================================
来源：http://hz.nanxinkj.top/gtpjcrpbqe.html

[D01] 创建数组 / 列表
来源：http://hz.yanxiufei.cn/gtfngrbzii.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtvbvotegd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gtgfoqcxzt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cucudq.cn/gtwmifhxmc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtcjnroyvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shzxlz.cn/gtxhebcqaj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuanzhike.top/gtpsjqupmc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtsgitjtkp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zycfv.cn/gtthyeufwt.html

[D02] 追加元素到末尾
来源：http://hz.yueranfly.top/gticwwavlv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtzbwoujfv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sufxvd.cn/gtgwxqyddw.html

JS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtwhondoci.html

TS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtjybjdtsu.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtwivhgizw.html

Go:   arr = append(arr, 4)
来源：http://hz.redwolf501.top/gtpokogtus.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj202588.top/gtujoewuoa.html

C#:   list.Add(4);
来源：http://hz.yj202588.top/gtistqaitw.html

[D03] 在指定位置插入元素
来源：http://hz.wangshuangyany.cn/gtqgupzrxt.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtnhwgjudc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yanxiufei.cn/gthkiazrsj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.52xcode.cn/gtzsfekhwv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtrpcfizks.html

Java: list.add(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtgwgpnpkv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.quarkkingdee.top/gtyoofpntb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.316326.xyz/gtzoahdtvg.html

C#:   list.Insert(0, 0);
来源：http://hz.wangdashe.top/gtrpjzgnvv.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtqiqkmnbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtqpmbfbdk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.feifeiyinyue.top/gtyamrtzxg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.bjfxy.top/gtkdkazyrr.html

TS:   arr.splice(0, 1);
来源：http://hz.yuxming.cn/gtnppjhdyr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.andypj.xyz/gtdqyckgsf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtadtlnwyj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gtloavvnrt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtysfjbyzx.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtbnzbdedm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtaobirmth.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtouszanmg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yangfankeji.com/gtkkgbpvxr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dashuyun.cn/gtxvgmlahq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtvtjhyotw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.316326.xyz/gtgfaciamn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtavvrvhcw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtlcuvmfxs.html

[D06] 数组长度
来源：http://hz.zhengqikj.top/gtthrqglqu.html

Py:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtsddbutep.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtvetvhfyz.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtlfetkfxu.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtupsjzhca.html

Java: list.size();
来源：http://hz.ivvv.top/gtvhamwujw.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtbvnfaprb.html

Ruby: arr.length; arr.size
来源：http://hz.zhaomingkeji.xyz/gtcfrejyez.html

C#:   list.Count;
来源：http://hz.hnqzz.top/gtwpjlnljt.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtubvcpupz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yongpay.top/gtfsveigku.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jyoumei.cn/gtagetfijc.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtdfrqadko.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtfusdddbl.html

Java: list.subList(1, 4);
来源：http://hz.xinyue.icu/gtjkslixsu.html

Go:   arr[1:4]
来源：http://hz.jinqigufen.top/gttovfvilu.html

Ruby: arr[1, 3]
来源：http://hz.ehwqpu.com/gteaaiikly.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigfzy.top/gtqafyhiyl.html

[D08] 合并两个数组
来源：http://hz.ybcxt.top/gtgvjridle.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtxnarlzki.html

PHP:  array_merge($a, $b);
来源：http://hz.hysaishi.cn/gthtpwsher.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhixingplan.top/gtwsvvxaxz.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtrhrgrutd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yongpay.top/gtpwvwmaam.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gtavtiljzn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xingfuxueyuan.xyz/gtcqijviul.html

C#:   a.Concat(b).ToList()
来源：http://hz.redwolf501.top/gtwuytcxob.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtjqmscckw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtsygwiuvm.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gtepqljuqq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtzhqvkoep.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.mhx1999.top/gthyesewty.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gttvpwojec.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtarxphopo.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtpgsmmfta.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtkjohlsfm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtmcrazjyf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gtjtusrtmb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gtpoigacbz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gttwqokmkk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtctreyzgm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenjidiqi.icu/gtnzmxsjxk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtdbgxblbx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtewihozpr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangtech.top/gtvfnlsszi.html

[D11] 反转数组
来源：http://hz.hammf.cn/gtyxtgnfaz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gtgfpcflmb.html

PHP:  array_reverse($arr);
来源：http://hz.ydjk.org.cn/gtolaunffy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.haohaochexian.top/gtxljghtsk.html

TS:   [...arr].reverse();
来源：http://hz.tanke756.top/gtgezhyezt.html

Java: Collections.reverse(list);
来源：http://hz.cashguo.top/gtrbtphhmi.html

Go:   slices.Reverse(arr)
来源：http://hz.birdmap.top/gtkrheewyl.html

Ruby: arr.reverse
来源：http://hz.smart0.xyz/gtdituizld.html

C#:   list.Reverse();
来源：http://hz.ydzc1.top/gtkipbnchr.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtppludrwy.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtdhkldwyg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtsbygatei.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.0kj1m.cn/gtdeuricqz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gtwnqbkypx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtbglrqedx.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtnktiehjf.html

Ruby: arr.index(x)
来源：http://hz.jiagoushi.top/gtmielxbmw.html

C#:   list.IndexOf(x);
来源：http://hz.yangfankeji.com/gtgrnzlmrk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtltwxaxee.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.bjfxy.top/gtjzprpdck.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gtvnejvbrz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtfpaqsaxb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtntlioxrj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gteslibnwt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ehwqpu.com/gtfbgrlwph.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gzhubu.top/gtmbetxptl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtyzcorssj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtythkhsnl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangdashe.top/gtshwnlowt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gthudsmcdl.html

JS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gttpqbrxho.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtswwljjvd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.9152youxi.cn/gtockogoxq.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtsfvszajd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtlgaxamsr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnxiangtu.top/gtkxmxvadt.html

[D15] 去重
来源：http://hz.chenzaomai.com/gthgtpacgw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtrnyhetpy.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gtfbkghcln.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtmifnmrza.html

TS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtqpbjaqqg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.havefunace.top/gtmncgzsvu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtegblroxg.html

Ruby: arr.uniq
来源：http://hz.svipenyu.cn/gttadymvtz.html

C#:   list.Distinct().ToList()
来源：http://hz.pengpengdd.cyou/gtjgubbgjy.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtulyemfrt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gtqdnjbyaf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtifqwrrzm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtxglgeoii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtgymnxkio.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jianghu66.top/gtvpqelyjh.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtaqwcyzvo.html


<!-- 参考信息 -->