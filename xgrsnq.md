代发 wailian999

Java: if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtbciulrxi.html

Go:   if data == nil { return }
来源：http://hz.gzhubu.top/gtcqepywsm.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtmrajetnj.html

C#:   if (data == null) return;
来源：http://hz.fengsongda.top/gtjjkufzgp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtibczsxgm.html

C. 函数与作用域
来源：http://hz.yj20258.top/gtovgtkgev.html

================================================================================
来源：http://hz.aizwys.cn/gtkqfgqzfd.html

[C01] 定义函数
来源：http://hz.xuetiantiany.cn/gtgwuxvihg.html

Py:   def add(a, b): return a + b
来源：http://hz.mhx1999.top/gtbifcjcjk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtrgpxiqky.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jianghu66.top/gtrmtonvqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtirwqhypd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtfgvcxyma.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gzhubu.top/gtfkctiupn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zycfv.cn/gtkffyddum.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtztrdsgxo.html

[C02] 默认参数
来源：http://hz.shanyushiyangkeji.top/gtohpoedfb.html

Py:   def greet(name="World"): return name
来源：http://hz.jinyuanbaomall.cn/gtbvocpshq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxinkj.top/gtztquuilm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtkankdsaa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dianchejie.cn/gtniqekdrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.kuanghao11.cn/gtkviexgsi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daria6918.cn/gtodydvptj.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtjfcsghxd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtgztvxshu.html

[C03] 可变参数
来源：http://hz.haohaochexian.top/gtdwfwrmmj.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gtrvbfrrtb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtjlyaerqq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gttrpbervl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxinkj.top/gtyebqkmzd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jianghu66.top/gtcqqejczr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gttjtjxvfo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aizwys.cn/gthuovnubc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinghuilouyu.cn/gtkzjujdwi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gzhubu.top/gtmzfelybg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xingfuxueyuan.xyz/gtycsoehlt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dashuyun.cn/gtmqfddzhi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.316326.xyz/gtzavsnkgb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ivvv.top/gtolosgjqw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tianlin.xyz/gtjjgzalxy.html

Go:   // 无：用配置结构体参数
来源：http://hz.hysaishi.cn/gtdexiqmkc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtpzfaneoq.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtneubrawr.html

[C05] 返回多个值
来源：http://hz.gzhubu.top/gtxywnvtzy.html

Py:   return a, b
来源：http://hz.0kj1m.cn/gtxbhcrueo.html

PHP:  return [$a, $b];
来源：http://hz.smart0.xyz/gtixzuqumr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hammf.cn/gtlaxfzvfc.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtmrybvbys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuanzx.com/gtmlrnszee.html

Go:   return a, b
来源：http://hz.jinqigfzy.top/gtunzxuhev.html

Ruby: return a, b
来源：http://hz.9152youxi.cn/gtxqhluboi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.bjfxy.top/gttcecnfhe.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtfqxmqlsu.html

Py:   square = lambda x: x * x
来源：http://hz.dianchejie.cn/gtrpsobvlb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtxsobjovf.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtpqnjurlh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtujyfewny.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtzxifmkmi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtpzlvflbf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zdqjudy.top/gtqzsrljhd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dianchejie.cn/gtpabbcxwe.html

[C07] 把函数作为参数传入
来源：http://hz.jinyuanbaomall.cn/gtytslujtl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.svipenyu.cn/gtaihxlrob.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jiagoushi.top/gtbuopdblo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gtsqmqoahw.html

TS:   arr.map(String)
来源：http://hz.zhijiandao.cn/gtuoslcdwt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.mhx1999.top/gtbbokcqaq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtpquzbwyn.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhaomingkeji.xyz/gthyvbvbom.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gtafoillyk.html

[C08] 闭包
来源：http://hz.ydjk.org.cn/gteehowowv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.mhx1999.top/gtrrihhzxk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gotoacloud.top/gtjyordwhv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtqvtgnjgq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtjzyxlygp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.52xcode.cn/gtalubgwoc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydzc1.top/gtqjtplvbz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.feifeiyinyue.top/gtpsfgeidk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtawwnvina.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtkvnlhmmi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gtngwxicmi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gtkoefdlyy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtikycpvev.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gthgjxbtqx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnqzz.top/gtgraklwnu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtqgusqswo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtxkalsvkp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yangfankeji.com/gtmvnmfqbw.html

[C10] 变量作用域
来源：http://hz.yj202588.top/gttkmvqyxm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gtvvsowdhx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xziqi.cn/gtdqxdyvsk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gtbzkwryft.html

TS:   同 JS
来源：http://hz.yuxming.cn/gtnbqfeuho.html

Java: 方法内为块级作用域
来源：http://hz.hysaishi.cn/gtbmycpbbc.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtwawxavij.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtsfwbgdqs.html

C#:   块级作用域
来源：http://hz.mhx1999.top/gtpklsplgo.html

[C11] 模块导入与导出
来源：http://hz.hysaishi.cn/gtegjkigsi.html

Py:   from module import func
来源：http://hz.cdnleiting.top/gtnipdwuvi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtkowpjeoh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtanhorcgc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gzhubu.top/gtyfxndqmf.html

Java: import java.util.List;
来源：http://hz.9152youxi.cn/gtspzdrogs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydzc1.top/gtniychkcy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jiagoushi.top/gtyrurtwtx.html

C#:   using System.Text;
来源：http://hz.jianghu66.top/gtpxfrebjf.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxinkj.top/gtffjjxqeo.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtvygmexoj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenjidiqi.icu/gtwcjmejrw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtakxrvjry.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtajlxhbht.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuanzhike.top/gtbtilbrbm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zycfv.cn/gtzjyqigei.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtoobzyvbi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.dashuyun.cn/gtptzswsom.html

[C13] 类型声明 / 类型注解
来源：http://hz.xylfe.cn/gtcfqhphww.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgfzy.top/gtkdxfekev.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gthjrlojye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtpdtpzcff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtdmrsunbf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtjfwfgbud.html

Go:   func add(a, b int) int
来源：http://hz.dashuyun.cn/gtwnlwnllv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.birdmap.top/gtejpnvbir.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tanke756.top/gtqyjiffoa.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtxjoptxkm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtyltzovhq.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtuiijrxyx.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtqhrduzdn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gtudecbrza.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.9152youxi.cn/gtrdanrbkc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtzmhbpaft.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtfzzjockj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shuidangran.top/gtnywyqkjj.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangkeji.top/gtgildfrnz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gtjnirkjgx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtanturlpk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtrpadrbad.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtvrzmdlsa.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gtablteypa.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtjvxfokbf.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtamakgcnw.html

C#:   var (a, b) = pair;
来源：http://hz.xingfuxueyuan.xyz/gtquqlupmd.html

[C16] 函数 / 方法重载
来源：http://hz.jlsjyb.cn/gtnhsvyxxf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenlongwang.top/gtvmpbfzzc.html

PHP:  // 无重载
来源：http://hz.birdmap.top/gtfzlwqamn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtvvakmgfo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cashguo.top/gtzerzdqpy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pycfn.com/gtlwgtxsuv.html

Go:   // 无重载：用不同函数名
来源：http://hz.feifeiyinyue.top/gtteabstfi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtkbuilaqo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gttelrdhqr.html

================================================================================
来源：http://hz.c1oappe.top/gtvnbudgao.html

D. 数组 / 列表 / 集合
来源：http://hz.aibaodan.cn/gtapqxhwof.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvgjmnnhs.html

[D01] 创建数组 / 列表
来源：http://hz.zhongyouzk.top/gtigjsrgpl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtspvhopvz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtinjnubjq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jyoumei.cn/gtbyptlkvt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtkhphxpqh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnqzz.top/gtwdykzqif.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ybcxt.top/gtlrwtrhem.html

Ruby: arr = [1, 2, 3]
来源：http://hz.haohaochexian.top/gtpyxilrmb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shuidangran.top/gtizjsrmxv.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gtdasvuzrs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtmxdqwpbm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sweek.top/gtcmblykks.html

JS:   arr.push(4);
来源：http://hz.guannengcc.top/gtjbbugtby.html

TS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtcjijmgdp.html

Java: list.add(4);
来源：http://hz.nwbrower.top/gtvdqruozy.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gticzzipod.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.wangdashe.top/gtmjvgxxlp.html

C#:   list.Add(4);
来源：http://hz.iojbl.cn/gtqezqllht.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtzovwudti.html

Py:   arr.insert(0, 0)
来源：http://hz.gotoacloud.top/gtrfnmxktg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gtqpyooqmp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gotoacloud.top/gtbnogdmmf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hywenlv.cn/gtwpcchyaq.html

Java: list.add(0, 0);
来源：http://hz.pengpengdd.cyou/gtihowziuq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtcwdovvsj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.andypj.xyz/gtuxduodbf.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gtqqnpqveg.html

[D04] 删除元素
来源：http://hz.cheryme.top/gtfvhlptfr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangkeji.top/gtrhmacyaf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtkwhpgbnz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ehwqpu.com/gtbsbdvytw.html

TS:   arr.splice(0, 1);
来源：http://hz.sysykeji.top/gtggellztc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtklmlcbeu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtxfwbdemb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gtyfcbzebe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hongshengwenyu.top/gtcnzbcxyd.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtogrtwqor.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtmybjoanh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtafwkrucp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fzhhl.top/gtzmnhxojl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhaomingkeji.xyz/gtbtfupwwb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtjrhgvdqy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aibaodan.cn/gthrgsuibj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtuhrojnao.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhengqikj.top/gtxskjnool.html

[D06] 数组长度
来源：http://hz.tian-w.cn/gteudhrvms.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtoenehfli.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtdngtrgsp.html

JS:   arr.length
来源：http://hz.hammf.cn/gtlyorjnsy.html

TS:   arr.length
来源：http://hz.fzhhl.top/gtduwqxpig.html

Java: list.size();
来源：http://hz.bjfxy.top/gtnapylhps.html

Go:   len(arr)
来源：http://hz.cashguo.top/gtnlfgpqch.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtxxmwfama.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtdnzescov.html

[D07] 切片 / 取子数组
来源：http://hz.hammf.cn/gtslvmnefa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtyanbowfl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gtbztekokh.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtbhdtnaxc.html

TS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtxmlbbina.html

Java: list.subList(1, 4);
来源：http://hz.zycfv.cn/gtgfojsndx.html

Go:   arr[1:4]
来源：http://hz.yuanzhike.top/gtsizfdvyh.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtmfkewjsu.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxinkj.top/gtpejcvuvi.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtrfzefnva.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhaomingkeji.xyz/gtdzyzqbtj.html

PHP:  array_merge($a, $b);
来源：http://hz.chenjidiqi.icu/gtvebscbwv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sxryk.cn/gtktlkjeiv.html

TS:   [...a, ...b];
来源：http://hz.gogol.net.cn/gteyynkfkq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenjidiqi.icu/gtfcymnzie.html

Go:   append(a, b...)
来源：http://hz.bjfxy.top/gtttaduntd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtiibpjosn.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtdawjykfe.html

[D09] 排序（升序）
来源：http://hz.redwolf501.top/gtsrpvvowp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtjqzbrcgp.html

PHP:  sort($arr);
来源：http://hz.feifeiyinyue.top/gttqkhlqxr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtndcyefgc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtkkhbtrui.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhixingplan.top/gtfozykvaz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtvxugpshy.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtfiqrnjpz.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtvkjfmgnp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenlongwang.top/gtwyhqagud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtitemieko.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtevynxdjx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtudpbrooa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtnjtuxvbx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gtwposcabq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dashuyun.cn/gtakinqftx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.pengpengdd.cyou/gtbphyptqz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hysaishi.cn/gtazsnjrni.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtsqbnswzn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.svipenyu.cn/gtoxrvianl.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtbpzkdqlz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtqnhqzadh.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtiiprchvs.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtpgnysljz.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtweeujwuc.html

Ruby: arr.reverse
来源：http://hz.havefunace.top/gtnifdrsjb.html

C#:   list.Reverse();
来源：http://hz.xuanzx.com/gtptmnqxsm.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtxhwbedlz.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtuxcrgldr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jyoumei.cn/gtfmiyzysb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtltakutzu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtbzbrowfc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yangfankeji.com/gtvyxspvss.html

Go:   slices.Index(arr, x)
来源：http://hz.ybcxt.top/gtfjonuivp.html

Ruby: arr.index(x)
来源：http://hz.wangdashe.top/gtqlszisti.html

C#:   list.IndexOf(x);
来源：http://hz.hfpthk.cn/gtucgaitdk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daxiang520.top/gtpttvkawd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtnjgcvpui.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtqgxcpigr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtpxclybqt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtauzgtbtm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtbnonbupn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtebllzuog.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtgvaborfc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.redwolf501.top/gtmtfqggys.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtlcfjmonx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangtech.top/gtxzofyyey.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtrorjqjek.html

JS:   arr.map(x => x * 2)
来源：http://hz.xuetiantiany.cn/gtxulczzxj.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtdbhotoev.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuanzhike.top/gtmrbdscdm.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtiwovncvh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jyoumei.cn/gtiwworiaf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.quarkkingdee.top/gtqlndywki.html

[D15] 去重
来源：http://hz.andypj.xyz/gtnsjjaalc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtvqglctrt.html

PHP:  array_unique($arr);
来源：http://hz.c1oappe.top/gtjkxvijgd.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtshjrqdmn.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtxgrhenur.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aizwys.cn/gtpwiqxryu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.mhx1999.top/gtscwbzlfl.html

Ruby: arr.uniq
来源：http://hz.zhijiandao.cn/gttwnkpgow.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtjxcidzkm.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gteytsjwnb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtojgrydyq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.svipenyu.cn/gtufcicscs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sweek.top/gtprkwnbqk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtjnpichyy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gtszgllbnf.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gtxaastjog.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gthhymgigt.html

C#:   list.Sum();  list.Average()
来源：http://hz.vqdsnc.cn/gtohjhddwa.html

[D17] 最大值与最小值
来源：http://hz.jinqigufen.top/gtppfmkygj.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtcrjvpzou.html


<!-- 参考信息 -->