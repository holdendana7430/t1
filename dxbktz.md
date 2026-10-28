代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gaohongyu789.top/gtykadiapi.html

Go:   return a, b
来源：http://hz.zycfv.cn/gtitcmwxmb.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtiiuxzhnh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.smart0.xyz/gtkfbcdame.html

[C06] 匿名函数 / lambda
来源：http://hz.xuanzx.com/gtbguukgvx.html

Py:   square = lambda x: x * x
来源：http://hz.xuetiantiany.cn/gtugpzbren.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtgqvadnim.html

JS:   const square = x => x * x;
来源：http://hz.9152youxi.cn/gtpnbtrayn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydzc1.top/gtcrcldnfe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.iojbl.cn/gtrvcbooey.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gtejdqlqav.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhoulong.xyz/gttpbcwidk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnxiangtu.top/gtjfkuorwr.html

[C07] 把函数作为参数传入
来源：http://hz.52xcode.cn/gtcoedskxc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtlzinyoyl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xingfuxueyuan.xyz/gtcdktjvkt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhixingplan.top/gtiikesvzg.html

TS:   arr.map(String)
来源：http://hz.zhoulong.xyz/gtuciarpnz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnxiangtu.top/gtalcmlfbi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gthrxfvxji.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtgucivojw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtpgvjdlko.html

[C08] 闭包
来源：http://hz.hywenlv.cn/gtalktzbtd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtktgvxvtb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtfedrcwjk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtgpldufnz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtglaefavc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258888.top/gtrhuqfhuc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxuanxn.top/gtqejmzwto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zycfv.cn/gthwdsmjny.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtvreddxog.html

[C09] 递归
来源：http://hz.zhaomingkeji.xyz/gtwvfullpa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shuidangran.top/gtvgyultdd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtlpbesxuu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtkbxsbjfq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtvbmfvixk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtopuhsjwc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtvckxscad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yvedp.cn/gtzfscfbsx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinyuanbaomall.cn/gtfgwmuzot.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gtnlxboysx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtclrsdqek.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhongyouzk.top/gtxtlymshc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangdashe.top/gtjultefup.html

TS:   同 JS
来源：http://hz.c1oappe.top/gtmwfowamp.html

Java: 方法内为块级作用域
来源：http://hz.hnxiangtu.top/gtflybfljq.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtsboyqbmx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinghuilouyu.cn/gtqcdocosk.html

C#:   块级作用域
来源：http://hz.gzhubu.top/gtvyzqpdci.html

[C11] 模块导入与导出
来源：http://hz.316326.xyz/gtpszshaqe.html

Py:   from module import func
来源：http://hz.daria6918.cn/gtypbljmjh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtijezrslx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jiagoushi.top/gtwfiknrhb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuanzhike.top/gtmwmkfxzz.html

Java: import java.util.List;
来源：http://hz.daxiang520.top/gtjrbeiixp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yangfankeji.com/gtanyhydun.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.c1oappe.top/gtrehjsnht.html

C#:   using System.Text;
来源：http://hz.pengpengdd.cyou/gtrwdtoukv.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxuanxn.top/gtiharwpic.html

Py:   (lambda: print("run"))()
来源：http://hz.xuanzx.com/gtaksqpdvo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cashguo.top/gtvojvqgxa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gteiezwype.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtsfgjqgxn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhoulong.xyz/gtppeomwkh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sysykeji.top/gtzdpkarsh.html

Ruby: -> { puts "run" }.call
来源：http://hz.c1oappe.top/gtdjuxfbkb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xziqi.cn/gtptxhuzbr.html

[C13] 类型声明 / 类型注解
来源：http://hz.dashuyun.cn/gtslnzqqwb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gtwqlmdyxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtzilxxudd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.52xcode.cn/gtrhuqlxrs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtwupdjqdf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtpeqcuwet.html

Go:   func add(a, b int) int
来源：http://hz.aizwys.cn/gtfffbktrt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnqzz.top/gttewrhfka.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sysykeji.top/gtoekcpmyo.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gteofloupy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tianlin.xyz/gtiyxrtyky.html

PHP:  // 无泛型
来源：http://hz.mhx1999.top/gtiglsncua.html

JS:   // 无泛型
来源：http://hz.iojbl.cn/gttfcsicux.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daria6918.cn/gtxgjogphu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtxebbxwop.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.havefunace.top/gtwusrmeuc.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangkeji.top/gtwsyscqgt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daria6918.cn/gtobvzcijs.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gtwueypmue.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gtpvciumfc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cdnleiting.top/gthxglhjwz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtbdtylyoh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxinkj.top/gtzqmiepde.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtqckigcnq.html

Go:   // 无解构
来源：http://hz.kuanghao11.cn/gtsbrhvrap.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gtrscmuoah.html

C#:   var (a, b) = pair;
来源：http://hz.fzhhl.top/gtobzjmjzi.html

[C16] 函数 / 方法重载
来源：http://hz.dashuyun.cn/gtugntagcw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtqihgaspk.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtvhlfmlqu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cucudq.cn/gthnvlepzo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gtpxkovulj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.0kj1m.cn/gtxrpfcdno.html

Go:   // 无重载：用不同函数名
来源：http://hz.jlsjyb.cn/gtrpgfpays.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhixingplan.top/gtledeqyam.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guannengcc.top/gtnxjttlfm.html

================================================================================
来源：http://hz.chenlongwang.top/gtlklilrph.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtgeyubgjj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqgobwmze.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtrodowifh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zdqjudy.top/gtlxaddjkb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtswbhmwjx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtslizninb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtgpmhmtaa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnxiangtu.top/gtbipshfau.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydzc1.top/gtekglgvmq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fzhhl.top/gtevrhndtr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtrzhoadts.html

[D02] 追加元素到末尾
来源：http://hz.guannengcc.top/gtyvafdwrd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jyoumei.cn/gtuhuffjmt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.0kj1m.cn/gtubyrdaah.html

JS:   arr.push(4);
来源：http://hz.yvedp.cn/gtcnvpulbv.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtjurcprkf.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtqzhbwcfg.html

Go:   arr = append(arr, 4)
来源：http://hz.smart0.xyz/gtfgxkcvnt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtvvdjhgbg.html

C#:   list.Add(4);
来源：http://hz.vqdsnc.cn/gtkngenqgs.html

[D03] 在指定位置插入元素
来源：http://hz.pengpengdd.cyou/gtaczsfndk.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtezzyjfpd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtrmindros.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zdqjudy.top/gtgscxdxtx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtbprbfbwl.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gtuxlnyyou.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yvedp.cn/gtmbyuddfg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fengsongda.top/gtaenurvop.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtxsbonucz.html

[D04] 删除元素
来源：http://hz.tanke756.top/gtnmxqfcgp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zdqjudy.top/gtvotoklbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gtlxeaaoqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtbpmqfnlh.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtxrnkydbd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtwelkgmcy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangdashe.top/gtaanuiocn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gttqqvnhcy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtraiaocpk.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gtjqhcrbmy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtuxcrctxs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgfzy.top/gtleyagpuh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fzhhl.top/gtnwpxqbhr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gtrembqtur.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtghwtfqgk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xziqi.cn/gtrisjutnm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtknyejnuh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtjpsucpng.html

[D06] 数组长度
来源：http://hz.nanxuanxn.top/gtqfrlnxju.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtjcyjufew.html

PHP:  count($arr);
来源：http://hz.cdnleiting.top/gtdpsxfdom.html

JS:   arr.length
来源：http://hz.ivvv.top/gtlvscleyn.html

TS:   arr.length
来源：http://hz.hnqzz.top/gtlwvhedbc.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtcsyhnsmo.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtedlicxwu.html

Ruby: arr.length; arr.size
来源：http://hz.svipenyu.cn/gtrviyaoiy.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtewbixask.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtwbhwjjdt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gthzdmxabv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhaomingkeji.xyz/gtbxirsshc.html

JS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtegjagswq.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtafoyrcmu.html

Java: list.subList(1, 4);
来源：http://hz.kuanghao11.cn/gtiucqlcna.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtsehsbuor.html

Ruby: arr[1, 3]
来源：http://hz.jiagoushi.top/gtsyichyzb.html

C#:   list.GetRange(1, 3);
来源：http://hz.gzhubu.top/gtkevccuxr.html

[D08] 合并两个数组
来源：http://hz.iojbl.cn/gtxjttealj.html

Py:   a + b;  a.extend(b)
来源：http://hz.ywan-chungtsiang.top/gtgriwmyvg.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtkhapfeyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtixrpqzxa.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtnsopnhfg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtkxttwfqv.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gtyetcwyhr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtuuvbgcbn.html

C#:   a.Concat(b).ToList()
来源：http://hz.ivvv.top/gtbomehzod.html

[D09] 排序（升序）
来源：http://hz.yj20258888.top/gtnyagcsbl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtfbsadibx.html

PHP:  sort($arr);
来源：http://hz.jinqigufen.top/gtfgoxbjnt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtdfgkrfez.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gtciptmaxj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jyoumei.cn/gtlfyytsqy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtosbfgnke.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtscpjwafv.html

C#:   list.Sort();
来源：http://hz.cdnleiting.top/gtqeggptzz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.smart0.xyz/gtcaehhbhb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ehwqpu.com/gtbpppuhht.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtnzwchdut.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtmeqsigja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtivskcnec.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gtfpvhjavm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sysykeji.top/gtniahgwly.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangdashe.top/gtniclauro.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtwbshdbud.html

[D11] 反转数组
来源：http://hz.sweek.top/gtzfbahden.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhijiandao.cn/gtsmebauto.html

PHP:  array_reverse($arr);
来源：http://hz.316326.xyz/gtyfczfeiz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangshuangyany.cn/gtrveioxyo.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gttpeltell.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtmxqruyip.html

Go:   slices.Reverse(arr)
来源：http://hz.haohaochexian.top/gtaxnlputr.html

Ruby: arr.reverse
来源：http://hz.aizwys.cn/gtropgemzu.html

C#:   list.Reverse();
来源：http://hz.cheryme.top/gtfyjkyfdd.html

[D12] 查找元素下标
来源：http://hz.wangshuangyany.cn/gttqydqqss.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtmsswiouf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtbvgxppks.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtrlkagqfp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtkcpahkdq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258888.top/gthctcbhsd.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgfzy.top/gtxxzaipgp.html

Ruby: arr.index(x)
来源：http://hz.ybcxt.top/gtneuklrme.html

C#:   list.IndexOf(x);
来源：http://hz.wangdashe.top/gtnviexity.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtinmryctu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yangfankeji.com/gtlansencr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgfzy.top/gtmjxaaueb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenzaomai.com/gtcantjxiq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gtvxgzfxdt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gtewlbpnvx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jyoumei.cn/gtsdatwezj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jlsjyb.cn/gtkwwafars.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gogol.net.cn/gtgnwrvpio.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtbjxqtkql.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cucudq.cn/gtanwsrrxo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtsqvbhdhr.html

JS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtkodidgvb.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtcvyzpefu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.c1oappe.top/gtdqysrcus.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtatbkxhzz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tianlin.xyz/gtlbkvqqex.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gthuzupfbf.html

[D15] 去重
来源：http://hz.sweek.top/gteyoxykee.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtpmfytuin.html

PHP:  array_unique($arr);
来源：http://hz.chenjidiqi.icu/gtfwhtutyv.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtjtibsfon.html

TS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtnzzvppio.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtwgoudese.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ppjwa.cn/gtejnnipbs.html

Ruby: arr.uniq
来源：http://hz.pycfn.com/gtzrgqibzo.html

C#:   list.Distinct().ToList()
来源：http://hz.ybcxt.top/gtzjaczrhf.html

[D16] 求和与平均值
来源：http://hz.wangshuangyany.cn/gtrguatufe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tanke756.top/gtwxtqwlsu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangkeji.top/gtvstqktdn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtxkvbaduk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtqudlabxc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.meibo888.top/gtkpwgiipo.html

Go:   // 手写循环累加
来源：http://hz.birdmap.top/gtqmkgaxkb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pycfn.com/gtkhjgphop.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtcbokyqgh.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtgklypcla.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gthyotcmke.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj202588.top/gtewnudyvw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtzxofjnah.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangtech.top/gtzyvateho.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtaorogqls.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.kuanghao11.cn/gtlgyaydlm.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangtech.top/gtpvuuuskg.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtdnbttkle.html

[D18] 扁平化嵌套数组
来源：http://hz.daxiang520.top/gtxknyvelm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gtoargczpt.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtzihptqkn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtmbeidywd.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtgpwrrgry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gogol.net.cn/gticvqittd.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gttjgzvsgb.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtgghmofuz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gtougizdwr.html

[D19] 按字段分组
来源：http://hz.yj20258.top/gtbpgemgox.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtounbzhuf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gtlruphimr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xinyue.icu/gtbnvkmibn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtrpruybws.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gtrmgwyove.html

Go:   // 手写 map[string][]T
来源：http://hz.vqdsnc.cn/gtycgqfvjb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtxjcwjpwf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tianlin.xyz/gtswygnnzt.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gtaoxzqdeu.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtmbhubooz.html

PHP:  array_count_values($arr);
来源：http://hz.yuanzhike.top/gtwedjcfxt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtovjiqqvo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtgesenucv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtkylpqwdb.html

Go:   // 手写 map[T]int
来源：http://hz.ivvv.top/gttuxpmckq.html

Ruby: arr.tally
来源：http://hz.snrcjt.cn/gtudfrxkct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtolqdvjlm.html

[D21] 判断是否包含某元素
来源：http://hz.kuanghao11.cn/gthplpyojd.html

Py:   x in arr
来源：http://hz.cheryme.top/gtzadrkjlc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gtjgzcajsq.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtcugiftyr.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtsqlpxxbw.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtkkvdtoqv.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtqlvfsnvx.html

Ruby: arr.include?(x)
来源：http://hz.xuetiantiany.cn/gtgiqkqsnl.html

C#:   list.Contains(x)
来源：http://hz.jinqigufen.top/gtbdugztru.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gogol.net.cn/gtlsufyfdg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ywan-chungtsiang.top/gtumbdjkke.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangdashe.top/gtcwsnitgq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtoiplwyzk.html

TS:   [...arr];
来源：http://hz.xinyue.icu/gtfndqpbml.html


<!-- 参考信息 -->