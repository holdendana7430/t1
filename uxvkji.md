代发 wailian999

[C02] 默认参数
来源：http://hz.jinghuilouyu.cn/gtolnrgrao.html

Py:   def greet(name="World"): return name
来源：http://hz.tanke756.top/gtquhbxnhn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yuanzhike.top/gtqvcxwyxl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtcrneqeyn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shuidangran.top/gtzhzrikvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tanke756.top/gtbacuqyyr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhengqikj.top/gtvvjenbvf.html

Ruby: def greet(name = "World") = name
来源：http://hz.xinyue.icu/gtnhptgcim.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.quarkkingdee.top/gtjstezgud.html

[C03] 可变参数
来源：http://hz.vqdsnc.cn/gtzuykmdno.html

Py:   def total(*args): return sum(args)
来源：http://hz.hammf.cn/gtituiqmmj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangtech.top/gtcbsvckwp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtdspxwnyv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtnhuhkqjv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtagqibmyw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sweek.top/gtsumtwdgc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtjluapjbo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tianlin.xyz/gtzeawgtis.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zycfv.cn/gtradtgnsd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtopahikzn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.52xcode.cn/gtymdzwysh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtzlfblwkm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guannengcc.top/gtkywoelro.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gtsvnqhwgf.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtloxuywop.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtsgqyagcd.html

C#:   f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtijngxsht.html

[C05] 返回多个值
来源：http://hz.cdnleiting.top/gtnlfftoiy.html

Py:   return a, b
来源：http://hz.sxryk.cn/gtmcagjtme.html

PHP:  return [$a, $b];
来源：http://hz.yanxiufei.cn/gtdvxekgwj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cheryme.top/gtxcomuzyu.html

TS:   return { a, b };
来源：http://hz.svipenyu.cn/gtzbgkbeek.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.redwolf501.top/gtixqjeomt.html

Go:   return a, b
来源：http://hz.jqgufenzy.top/gtkjezzpqc.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtjuimkfxy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cashguo.top/gtokjxaaht.html

[C06] 匿名函数 / lambda
来源：http://hz.hysaishi.cn/gtnuxptfoo.html

Py:   square = lambda x: x * x
来源：http://hz.cucudq.cn/gtttyvasks.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daria6918.cn/gtqweihyvp.html

JS:   const square = x => x * x;
来源：http://hz.cashguo.top/gtjumsbnmt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.c1oappe.top/gtbmjixkad.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ywan-chungtsiang.top/gttcclokqa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtxzbyybcf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.redwolf501.top/gtohezcchb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cucudq.cn/gtfhcktstf.html

[C07] 把函数作为参数传入
来源：http://hz.mhx1999.top/gtfzvgzcmb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhiwuduotai.top/gtmremusbb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yueranfly.top/gtrchiuzac.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.haohaochexian.top/gtezjejyvs.html

TS:   arr.map(String)
来源：http://hz.iojbl.cn/gtijemzkrh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhengqikj.top/gtpfhuvdpq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtmfloqzpi.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtcsklyilb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhixingplan.top/gtrpwhbxim.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtdlecvgbi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.vqdsnc.cn/gtxragqxmg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gtzcmimevg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtgfuxhjgk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gttcbxeara.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuetiantiany.cn/gtvgmvjufr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cdnleiting.top/gtgektkvox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gzhubu.top/gthvvhlwxh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtdhbhrvxe.html

[C09] 递归
来源：http://hz.hywenlv.cn/gtyfenqgxn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gttnbocdos.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gtunzppzjl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gthqibdnbf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtlngryjqv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pengpengdd.cyou/gtjindahey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zdqjudy.top/gtvzebzxae.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtocqbrayd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtnmmglitd.html

[C10] 变量作用域
来源：http://hz.meibo888.top/gteqqxqjio.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtmndairxg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtrcnbarge.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.c1oappe.top/gtrluxgnlj.html

TS:   同 JS
来源：http://hz.aizwys.cn/gtmcaqdkqo.html

Java: 方法内为块级作用域
来源：http://hz.yuanzhike.top/gtcojokdoc.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtuzaldsbb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtbiczbznw.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtlddeldkl.html

[C11] 模块导入与导出
来源：http://hz.ivvv.top/gtdxlyreni.html

Py:   from module import func
来源：http://hz.daxiang520.top/gtbcgjjewi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yangfankeji.com/gtpuuedfqb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtaluomroz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtttwmttve.html

Java: import java.util.List;
来源：http://hz.shanyushiyangtech.top/gtmgaifvid.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cqqwz.cn/gtzwdxtgvu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hywenlv.cn/gtdulanfhp.html

C#:   using System.Text;
来源：http://hz.hammf.cn/gtgbwobhxx.html

[C12] 立即执行函数 IIFE
来源：http://hz.sxryk.cn/gtyechzlky.html

Py:   (lambda: print("run"))()
来源：http://hz.cdnleiting.top/gticjgpvic.html

PHP:  (function () { echo "run"; })();
来源：http://hz.snrcjt.cn/gtlpspjfmp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtfhynfuun.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtfvvnlsog.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtmyqmqlql.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtqvdcetbl.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtgxgmlnje.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tianlin.xyz/gtyfmdikzc.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtsdgqgjxw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtybkjwtpi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtucvabwil.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guannengcc.top/gtgbyyiyqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtroiawoot.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtrjbpjxil.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtjpocpwgr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtgamyxmfr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.svipenyu.cn/gtihhclize.html

[C14] 泛型函数
来源：http://hz.zhengqikj.top/gtrhyjxybv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shangyingyoupin.top/gtjiatamyv.html

PHP:  // 无泛型
来源：http://hz.hammf.cn/gtycrusgrb.html

JS:   // 无泛型
来源：http://hz.ydzc1.top/gttunczsow.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtqwyhmkht.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gtukuzmdwr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnxiangtu.top/gttjqguyom.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtclqideoi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gtppfykoou.html

[C15] 解构 / 展开参数
来源：http://hz.andypj.xyz/gtjwcteerl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtthzmkbpf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.c1oappe.top/gteiklwkbt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtncnlwndd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cucudq.cn/gtoisjrzqs.html

Java: // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtrgibmida.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtxrigvhgk.html

Ruby: a, b = pair
来源：http://hz.zhoulong.xyz/gtquwiuntt.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtcaozhfuk.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtvftamlek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gtpkfkyrqe.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtfybabvjt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cucudq.cn/gtyjkkmqmh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.vqdsnc.cn/gtrzesjhxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtbgfedzrp.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gthwlvcpur.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daxiang520.top/gthrlrlyfd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtpitadphm.html

================================================================================
来源：http://hz.hfpthk.cn/gtgkmtxmgy.html

D. 数组 / 列表 / 集合
来源：http://hz.yangfankeji.com/gtlsijnyxm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmisbnphj.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtpunplwlg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ybcxt.top/gtwmgvifxb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daxiang520.top/gtcutylrrk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gtmlkluwzh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtaddkvqik.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dianchejie.cn/gtynfhqppw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gtdkrmcaox.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gttauyokxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.mhx1999.top/gtshzthkxi.html

[D02] 追加元素到末尾
来源：http://hz.cheryme.top/gtlrljpcps.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangshuangyany.cn/gthmdytyrd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aizwys.cn/gtiwopvswd.html

JS:   arr.push(4);
来源：http://hz.pycfn.com/gtnirspveo.html

TS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gththugcno.html

Java: list.add(4);
来源：http://hz.jinghuilouyu.cn/gtjfcazrzs.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gttxctaiaa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtkcmueydr.html

C#:   list.Add(4);
来源：http://hz.redwolf501.top/gtrujseljc.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtykryahvm.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtswamlupb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aizwys.cn/gtlhxgyjru.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gtnnntxldo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtgtadgmdi.html

Java: list.add(0, 0);
来源：http://hz.jqgufenzy.top/gtgasozzuh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigufen.top/gtsscdbhdi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zycfv.cn/gtgjwgoqbv.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtzfaoajfs.html

[D04] 删除元素
来源：http://hz.ehwqpu.com/gtfxqgargi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtmjyzjnre.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xziqi.cn/gtapsqfvgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jlsjyb.cn/gtycrwnrvy.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtmwbdkbyb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.316326.xyz/gttwpochsu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinqigfzy.top/gtflnrqkqn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgfzy.top/gtslvvrkoq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtwaouqhvh.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtheqkvqjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtkkhjliep.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtccbanlzm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daxiang520.top/gttyfswxpo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtudhyecck.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtppmrdvyy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gttkgodxvq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtzybryzst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gtcxqutxsq.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtldytqmkw.html

Py:   len(arr)
来源：http://hz.zhengqikj.top/gtkeyfavrz.html

PHP:  count($arr);
来源：http://hz.andypj.xyz/gtgqlxocpi.html

JS:   arr.length
来源：http://hz.yj20258.top/gtfokzkfys.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gtbcidhvgw.html

Java: list.size();
来源：http://hz.yvedp.cn/gtftfyiddp.html

Go:   len(arr)
来源：http://hz.shuidangran.top/gtmqzxjxmx.html

Ruby: arr.length; arr.size
来源：http://hz.jlsjyb.cn/gtydwghjao.html

C#:   list.Count;
来源：http://hz.chenzaomai.com/gthdntocrp.html

[D07] 切片 / 取子数组
来源：http://hz.shzxlz.cn/gtpdkziozz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtutrunhqx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtsxpkqjer.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtwixzqyzf.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtdwqjasrv.html

Java: list.subList(1, 4);
来源：http://hz.shangyingyoupin.top/gtleyiivyg.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gtraaagdop.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gtpyvxrxao.html

C#:   list.GetRange(1, 3);
来源：http://hz.zycfv.cn/gtpkxgaiwz.html

[D08] 合并两个数组
来源：http://hz.haohaochexian.top/gtgffgfbvn.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtbwmlubbv.html

PHP:  array_merge($a, $b);
来源：http://hz.chenjidiqi.icu/gthnhmbliz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtuovtmwig.html

TS:   [...a, ...b];
来源：http://hz.yuxming.cn/gtgdpmtmtn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtzktzqqjd.html

Go:   append(a, b...)
来源：http://hz.wangshuangyany.cn/gtwmtbevgu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xingfuxueyuan.xyz/gtbeozykwc.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtvktzxknp.html

[D09] 排序（升序）
来源：http://hz.wangdashe.top/gteaidpmza.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtwnjhssui.html

PHP:  sort($arr);
来源：http://hz.xziqi.cn/gtcipqarjp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ybcxt.top/gttsaqkgrj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gteebiiavw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jiagoushi.top/gthmucmuqt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuanzx.com/gtqhymyenf.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtkwnrxpyh.html

C#:   list.Sort();
来源：http://hz.meibo888.top/gtbckfwqin.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aizwys.cn/gtahmlafev.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fzhhl.top/gthtxdwnji.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gthdxkwjug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtcpbykgcj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtladbtkym.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gtrdkoecci.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.quarkkingdee.top/gtuiuqdgms.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.meibo888.top/gtrbdhdyka.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zycfv.cn/gtrotaxcrx.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtmxmfcvmk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtmujbtnfg.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtgtxhzpyu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtikapysgi.html

TS:   [...arr].reverse();
来源：http://hz.yuxming.cn/gtaaslitkf.html

Java: Collections.reverse(list);
来源：http://hz.ydjk.org.cn/gttzdocqky.html

Go:   slices.Reverse(arr)
来源：http://hz.yangfankeji.com/gtsyprkodd.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtyxekxugf.html

C#:   list.Reverse();
来源：http://hz.yonumen.top/gtqohcavmo.html

[D12] 查找元素下标
来源：http://hz.jyoumei.cn/gtummabkrk.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258888.top/gtbjxqdpef.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gthikfrxmd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtqxamxnre.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gtwkhkooja.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xingfuxueyuan.xyz/gtdfpqrxnk.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gteojllypn.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtdkxnavzj.html

C#:   list.IndexOf(x);
来源：http://hz.wangdashe.top/gtvddlwedx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daria6918.cn/gtagnlaiih.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj202588.top/gtqoydcjyz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtwhwjgrgo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtvtdddkbj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gttjzkohjd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.kuanghao11.cn/gtjbhxrzim.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.c1oappe.top/gtldubzvit.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtlmsqerxe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtmmabycfv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxinkj.top/gtedwqhqvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtkaylszqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.52xcode.cn/gttttydpfc.html

JS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gtmyvalces.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtpzbcbcpa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.bjfxy.top/gtvtjkxbus.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtrxmgmbfz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xinyue.icu/gtchsdgrer.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtcjzuvjxg.html

[D15] 去重
来源：http://hz.bjfxy.top/gtutjufbry.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gtoikoxpgk.html

PHP:  array_unique($arr);
来源：http://hz.nwbrower.top/gtvldorfkt.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtcjqoxoun.html

TS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtnhriciiu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yueranfly.top/gthbqicmwp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuanzx.com/gtbbqyyxnd.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtqosboydk.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtbjizjyih.html

[D16] 求和与平均值
来源：http://hz.nwbrower.top/gtigbhwiwc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xuanzx.com/gttfficplg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtejnvmfbq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtgteroxgs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtnfaqamzs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtjmzuvbcr.html

Go:   // 手写循环累加
来源：http://hz.daxiang520.top/gtgcohikyb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtjnleupll.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtokbznhzb.html

[D17] 最大值与最小值
来源：http://hz.c1oappe.top/gtwapnirsp.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtpmxzrqpv.html

PHP:  max($arr);  min($arr);
来源：http://hz.zdqjudy.top/gtojgqkvym.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yvedp.cn/gtvrlbhpgv.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtpcrbkada.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gtubmslear.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gtxolsphkj.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gttlycyffo.html

C#:   list.Max();  list.Min()
来源：http://hz.havefunace.top/gtuordlnwy.html

[D18] 扁平化嵌套数组
来源：http://hz.sxryk.cn/gtfbmbeeus.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenlongwang.top/gtosuwncwg.html

PHP:  array_merge(...$nested);
来源：http://hz.ppjwa.cn/gtfvonmdiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fzhhl.top/gtnwwoustr.html

TS:   nested.flat();
来源：http://hz.gzhubu.top/gtwwazqyin.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtpjsbyhyo.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtdpjwzxew.html

Ruby: nested.flatten
来源：http://hz.jyoumei.cn/gtfbcmtvyy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtgbmfybkb.html


<!-- 参考信息 -->