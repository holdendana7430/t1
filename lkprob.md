代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ydjk.org.cn/gtpxegusdb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtmbqkguxk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gzhubu.top/gttcoiclwn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtqbmqshsu.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuanzx.com/gtsdcdtpvb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtfqrnqwde.html

C#:   f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtdouqtwcp.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtcpxrwqay.html

Py:   return a, b
来源：http://hz.c1oappe.top/gtjfpowtwl.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gttaroeuzm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sweek.top/gtwzjsvmfy.html

TS:   return { a, b };
来源：http://hz.ehwqpu.com/gtdfltyxnk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhaomingkeji.xyz/gtxxbecltp.html

Go:   return a, b
来源：http://hz.yj20258.top/gtyaymjahe.html

Ruby: return a, b
来源：http://hz.jyoumei.cn/gtlyxrhxid.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtsldwikss.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtlvolvazb.html

Py:   square = lambda x: x * x
来源：http://hz.yangfankeji.com/gtlzcdpkua.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.havefunace.top/gtwzcwcbxs.html

JS:   const square = x => x * x;
来源：http://hz.fzhhl.top/gtsvzimvrx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gtrpkkxzvm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtbxxfgpgl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shzxlz.cn/gteonljfle.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gthddfbbon.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.52xcode.cn/gtykaogxyy.html

[C07] 把函数作为参数传入
来源：http://hz.zycfv.cn/gtsnirtwdz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gtxmtovwcu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.meibo888.top/gtsizedstj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtxoxawupg.html

TS:   arr.map(String)
来源：http://hz.xuanzx.com/gtcetptbik.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cucudq.cn/gtsbmnxnfi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pengpengdd.cyou/gtpebudxiw.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gtxhncelho.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinyuanbaomall.cn/gtphraqyhw.html

[C08] 闭包
来源：http://hz.jinqigufen.top/gtudbwlmie.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.c1oappe.top/gtwtiqcotg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuetiantiany.cn/gtskdccfps.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtpwkrbode.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtbeylejej.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenlongwang.top/gtltnxdyxf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sufxvd.cn/gtiehzkujc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.haohaochexian.top/gtzkvikioz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtcxkjexob.html

[C09] 递归
来源：http://hz.hongshengwenyu.top/gtvftkhtcx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgfzy.top/gtlxuufzwb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jlsjyb.cn/gtwvsjjuuz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtggrxgifu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtmjrlrity.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guannengcc.top/gtnziheusm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gthceeyulx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.andypj.xyz/gterikgnbz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinghuilouyu.cn/gtyrwzfgzx.html

[C10] 变量作用域
来源：http://hz.zhixingplan.top/gtvmqcjqqp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtaxfhlbzd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydjk.org.cn/gtnklhsywz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.pengpengdd.cyou/gtljsjkube.html

TS:   同 JS
来源：http://hz.gaohongyu789.top/gtttufzjlr.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtpaigbphw.html

Go:   花括号块级作用域
来源：http://hz.havefunace.top/gtwnjziojk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtilrdxxsw.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtiyczxvzp.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtbxgmheqx.html

Py:   from module import func
来源：http://hz.havefunace.top/gtgfarvxuu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tanke756.top/gtiawgcowt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtbifoxqvu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hfpthk.cn/gthcylhppr.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gtzvvlukzm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gtekmlqahe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xinyue.icu/gtqhpeojeb.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtwgfevjbd.html

[C12] 立即执行函数 IIFE
来源：http://hz.gzhubu.top/gtvpsuxert.html

Py:   (lambda: print("run"))()
来源：http://hz.guannengcc.top/gtupxzuhaj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gttzvobwxg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gttelfiyaw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtwvwzsrme.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258888.top/gtxxqymmoe.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtaxtdtewt.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtgawvhdvl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gttulodwgo.html

[C13] 类型声明 / 类型注解
来源：http://hz.fzhhl.top/gtijeihjrv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shuidangran.top/gtbcllbmak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtdobublvt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtxwueurtm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtlmzldjmn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtfcjbwzkh.html

Go:   func add(a, b int) int
来源：http://hz.andypj.xyz/gtymdvaiuy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ivvv.top/gtyjsrfamm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xziqi.cn/gtuwrbhhfm.html

[C14] 泛型函数
来源：http://hz.ydjk.org.cn/gtackaypzf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinghuilouyu.cn/gtchdapqrx.html

PHP:  // 无泛型
来源：http://hz.cdnleiting.top/gttoorzezu.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gtdzdowsnh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtnqgzimbm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fzhhl.top/gtxjuitfiu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtspbxrtcg.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtnaifezxp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ywan-chungtsiang.top/gthpjjjsmc.html

[C15] 解构 / 展开参数
来源：http://hz.chenjidiqi.icu/gtgchxiyhk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gtpokkzoky.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnqzz.top/gtmfqnmzat.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtwdnbmifo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shangyingyoupin.top/gtkncrufno.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtxxmcsdyt.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gtfwndpoly.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangkeji.top/gtfwdvbqkx.html

C#:   var (a, b) = pair;
来源：http://hz.daria6918.cn/gtqvhboicj.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtxrivmbgh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtbxblusat.html

PHP:  // 无重载
来源：http://hz.hysaishi.cn/gtnvhoqbod.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtqcvooedy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtsgrrrwyz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuanzhike.top/gthuynvfqw.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gtnrqdddpg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtoytrmeqh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtihbmaswx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjhiytkmz.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxuanxn.top/gtabizlxly.html

================================================================================
来源：http://hz.c1oappe.top/gtoongduzk.html

[D01] 创建数组 / 列表
来源：http://hz.mhx1999.top/gtfnbdafgg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jqgufenzy.top/gtbcpiqnfl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtwoprekki.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gtwjpjfadj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gtcokagfds.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cucudq.cn/gtysrqzwef.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hysaishi.cn/gtolyglpve.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtdefljpcp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtqnctxfki.html

[D02] 追加元素到末尾
来源：http://hz.mhx1999.top/gtxfbxnqsz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtjvmzcqas.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtijbclivw.html

JS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtsexqpsbj.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtofsqqhxt.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtconipmvj.html

Go:   arr = append(arr, 4)
来源：http://hz.zhijiandao.cn/gtzgwnjqic.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtvidgvnqt.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtetmtblpt.html

[D03] 在指定位置插入元素
来源：http://hz.ydjk.org.cn/gtcrwmaglm.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtwhxwyblm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.feifeiyinyue.top/gtdxfsixtr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dashuyun.cn/gtxgapznrj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cqqwz.cn/gtiqsrbzsf.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gtientkquv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sysykeji.top/gtsqcjarif.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yueranfly.top/gtffctmljh.html

C#:   list.Insert(0, 0);
来源：http://hz.0kj1m.cn/gtdvszqnma.html

[D04] 删除元素
来源：http://hz.tian-w.cn/gtsdboijpu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtzaljdrse.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aizwys.cn/gtmnncunpk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhengqikj.top/gtbsnadvbz.html

TS:   arr.splice(0, 1);
来源：http://hz.jinyuanbaomall.cn/gtbqmqvheh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtdtuzpkfy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shzxlz.cn/gtwnjjjmmb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jyoumei.cn/gtqtffuopn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hysaishi.cn/gtmhheynxu.html

[D05] 访问与修改元素
来源：http://hz.zhiwuduotai.top/gtbageifxf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtbdhqqfdo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtfxdncuqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtsbhaephn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtrtiuytbx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zycfv.cn/gtrwgqpjqe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gtgmvsdbok.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtlfyewrmd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cdnleiting.top/gtqxbgggqq.html

[D06] 数组长度
来源：http://hz.yanxiufei.cn/gtrtejwgoy.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtnmhtluzf.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtofwdludn.html

JS:   arr.length
来源：http://hz.fzhhl.top/gtjxicttrs.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtuwyhyiqn.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtugnicnpr.html

Go:   len(arr)
来源：http://hz.52xcode.cn/gtmvqmcmyy.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtefrihako.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gtnjkfjdtx.html

[D07] 切片 / 取子数组
来源：http://hz.dianchejie.cn/gtmpatqwaa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenlongwang.top/gtbwvefahk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenlongwang.top/gtrlxcwuhj.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtlzwdtgmy.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtizvjxmax.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gthvujcice.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtwyoasfag.html

Ruby: arr[1, 3]
来源：http://hz.cheryme.top/gtrazzmdlh.html

C#:   list.GetRange(1, 3);
来源：http://hz.c1oappe.top/gtemdqvhkh.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtziredbpk.html

Py:   a + b;  a.extend(b)
来源：http://hz.pycfn.com/gtowmslnaf.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtuhlxnggt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydzc1.top/gthvimsowy.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtidokfuop.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gtmjzteqce.html

Go:   append(a, b...)
来源：http://hz.hnxiangtu.top/gtfcbsuvog.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yvedp.cn/gthriykbyr.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtldinuabn.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtkkbaxnfp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gttqwxydgl.html

PHP:  sort($arr);
来源：http://hz.fzhhl.top/gtsmzfsapl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhiwuduotai.top/gtcemfdscp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtnloafxme.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtidgaaddj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hammf.cn/gtovjhhatq.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtcijisshw.html

C#:   list.Sort();
来源：http://hz.zhengqikj.top/gtqzhenkpp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtnhhrvmnp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnqzz.top/gteooogxtt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtxmhurmyz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtlcvewsth.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtaanvczlf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtuvzyrlvj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.iojbl.cn/gtegmxcwbm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yangfankeji.com/gtirvdpdhj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnxiangtu.top/gtwjlihklz.html

[D11] 反转数组
来源：http://hz.daxiang520.top/gtwemrxqrz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gtmrnwqwjp.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtjtbjfngv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtocdinjfl.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtoedyzrer.html

Java: Collections.reverse(list);
来源：http://hz.jiagoushi.top/gtguafgtkm.html

Go:   slices.Reverse(arr)
来源：http://hz.hysaishi.cn/gtbjelcwhk.html

Ruby: arr.reverse
来源：http://hz.jinyuanbaomall.cn/gtpjshkplq.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtuijeodwc.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtxvfiprez.html

Py:   arr.index(x);  x in arr
来源：http://hz.yangfankeji.com/gtsyqbmhok.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.quarkkingdee.top/gtofukowdd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtduqiceuf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtukssbton.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.havefunace.top/gtcyyssorn.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtarikwerx.html

Ruby: arr.index(x)
来源：http://hz.meibo888.top/gtutkoxhvr.html

C#:   list.IndexOf(x);
来源：http://hz.shzxlz.cn/gtbowxxrcc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtnxxfwcdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tanke756.top/gtnlgwypfo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daxiang520.top/gthfeqkzye.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtyfegghul.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtmrmkhvqp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sxryk.cn/gtjlgxtfyo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xinyue.icu/gtrxrslpvq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gtukaodgbl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sweek.top/gtrxnvxzsb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinyuanbaomall.cn/gtibgyqeso.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhiwuduotai.top/gtbmfkpdgk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtxjntahpz.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtqimebryr.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtgkbwrvxt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtcrniauot.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtuzscprxm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtqmjezqfx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cashguo.top/gtrrecbvyy.html

[D15] 去重
来源：http://hz.chenlongwang.top/gtkxtrmtkc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtwglexsjq.html

PHP:  array_unique($arr);
来源：http://hz.9152youxi.cn/gtrbepltir.html

JS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtgkxxizhj.html

TS:   [...new Set(arr)]
来源：http://hz.birdmap.top/gtsxyahsya.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zdqjudy.top/gtwucpxcqg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shangyingyoupin.top/gtucbyuxvn.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtnfvohgsq.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gttnslbbdx.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtxibagtjp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258.top/gtnfuibtej.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cucudq.cn/gtgfdpjbak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtxtbnqskr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtqehxjlxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtmoxeuqov.html

Go:   // 手写循环累加
来源：http://hz.nanxuanxn.top/gtudxwbjly.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gtzcywyeqp.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgfzy.top/gtvnrubzkq.html

[D17] 最大值与最小值
来源：http://hz.meibo888.top/gtcfflsvaf.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtabownmzf.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtunqclcwp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtwxpycdix.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtypkxiekd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtaphsfayn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gtzhbiqxal.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtesytvtqw.html

C#:   list.Max();  list.Min()
来源：http://hz.xylfe.cn/gtnoqeilqz.html

[D18] 扁平化嵌套数组
来源：http://hz.quarkkingdee.top/gtddriyldr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.svipenyu.cn/gtasckbmgs.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtaqyzjbqp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtuxsmwldi.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtnhaeduku.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtnlrjxozd.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtboootlie.html

Ruby: nested.flatten
来源：http://hz.gzhubu.top/gtslrainfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yvedp.cn/gtwbgkuszn.html

[D19] 按字段分组
来源：http://hz.jlsjyb.cn/gtnfuetjlj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnqzz.top/gtyztmbrup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gtaauwxbkf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hammf.cn/gtzvuxcwhu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.316326.xyz/gteqmjyxcz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtytfkqyco.html

Go:   // 手写 map[string][]T
来源：http://hz.sysykeji.top/gtvenjxghg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtzcwhpewy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtgfngnxke.html

[D20] 统计每个元素出现次数
来源：http://hz.tanke756.top/gthfsakzdn.html

Py:   Counter(arr)
来源：http://hz.hammf.cn/gtxnczytad.html

PHP:  array_count_values($arr);
来源：http://hz.jyoumei.cn/gtucnavtmi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtbgvreovd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtmipouwby.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtxdvdvdcc.html

Go:   // 手写 map[T]int
来源：http://hz.iojbl.cn/gtitslznpi.html

Ruby: arr.tally
来源：http://hz.pengpengdd.cyou/gtijdsnlmp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.bjfxy.top/gtrfcurmpg.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtffmdiljf.html

Py:   x in arr
来源：http://hz.feifeiyinyue.top/gtwugfcioi.html


<!-- 参考信息 -->