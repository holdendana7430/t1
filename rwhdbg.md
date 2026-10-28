代发 wailian999

Py:   return a, b
来源：http://hz.316326.xyz/gtghdbckmx.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gtyqcsanbd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xylfe.cn/gtqreliqsk.html

TS:   return { a, b };
来源：http://hz.316326.xyz/gtwxtgzpsa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gthrwybeaa.html

Go:   return a, b
来源：http://hz.guowangkeji.top/gtfyuypeug.html

Ruby: return a, b
来源：http://hz.cashguo.top/gtmcbljgdl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yueranfly.top/gtphhofbgp.html

[C06] 匿名函数 / lambda
来源：http://hz.shangyingyoupin.top/gtlwxbwoib.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtvkcrgxgv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258.top/gtzboldsly.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gttmlvxywt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.9152youxi.cn/gtuxyfzzus.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jqgufenzy.top/gtsndxcmar.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.svipenyu.cn/gtrvpnhybg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.daxiang520.top/gtglnprmtj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.smart0.xyz/gtborfoakt.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtqppihfeu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yangfankeji.com/gtneavomhk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gthkholexb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yueranfly.top/gtuxcbpyff.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtbgynjbgn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yvedp.cn/gtzhfyxvoq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yonumen.top/gthmgiocfn.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtpwispisl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinyuanbaomall.cn/gtehhdjddl.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gttyvbovdm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtmfvnnkfy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xziqi.cn/gtdckkhctz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtrmccplzf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gthpwdltaf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dashuyun.cn/gtulaxfqyq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258.top/gthngccagd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtcvubhieu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtstvtcpun.html

[C09] 递归
来源：http://hz.smart0.xyz/gtspoosdqt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtygdmtxky.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cqqwz.cn/gtdwmlrntj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtuoebcpsb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtympnaxta.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtbpndvets.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtbzbyebwu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nanxuanxn.top/gtojcoeiat.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jqgfzy.top/gtynadlezn.html

[C10] 变量作用域
来源：http://hz.nanxuanxn.top/gtmygpvbnq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hammf.cn/gtrqvdsjwb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.9152youxi.cn/gtwlmllvdb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gzhubu.top/gtuzrlrmxn.html

TS:   同 JS
来源：http://hz.cheryme.top/gtxqrojzfp.html

Java: 方法内为块级作用域
来源：http://hz.yj202588.top/gtnabdljkd.html

Go:   花括号块级作用域
来源：http://hz.yonumen.top/gtqrgtyyej.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dashuyun.cn/gtxjusbfnp.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtbqdlzmhf.html

[C11] 模块导入与导出
来源：http://hz.ppjwa.cn/gtfqulzavt.html

Py:   from module import func
来源：http://hz.xingfuxueyuan.xyz/gtgsmyoygo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtscfkjeac.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenlongwang.top/gtsdgsefug.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.haohaochexian.top/gtwgscczli.html

Java: import java.util.List;
来源：http://hz.jinqigfzy.top/gtfqtjwxmo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gtphmtsaah.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtzqhnltqt.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtdftzfoaf.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gthbsiixjv.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtxlhtsaaz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhengqikj.top/gtauygigxk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtlvekfwqr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtvhrzafmk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtjrpiiwrh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jyoumei.cn/gtixvsmjjk.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtytjcevvp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sufxvd.cn/gtgiflgubc.html

[C13] 类型声明 / 类型注解
来源：http://hz.quarkkingdee.top/gtslxacfis.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gtlsjwznsg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtqbkmnoqp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ehwqpu.com/gtrshykyte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtigcsrzwa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gterwimzxz.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gthlyevwxm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guannengcc.top/gtgktqxygb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinqigfzy.top/gtidzpdmxq.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtktsurewj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtcmrjttks.html

PHP:  // 无泛型
来源：http://hz.sufxvd.cn/gtecnhzjuz.html

JS:   // 无泛型
来源：http://hz.yj20258.top/gtzvpmmfte.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtdcldoxrn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuanzx.com/gticejvocg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.iojbl.cn/gtvafrjqts.html

Ruby: # 无泛型
来源：http://hz.andypj.xyz/gtedhdekwa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtlwphnywo.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtkypvlvwv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtxrdgoohy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gthuzrvbdt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtacuiubem.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shuidangran.top/gtbgsyeqls.html

Java: // 无解构
来源：http://hz.jinqigfzy.top/gtcjfdbamr.html

Go:   // 无解构
来源：http://hz.pengpengdd.cyou/gtoavpshka.html

Ruby: a, b = pair
来源：http://hz.cheryme.top/gtecxbhdoi.html

C#:   var (a, b) = pair;
来源：http://hz.aibaodan.cn/gtynfnkjtn.html

[C16] 函数 / 方法重载
来源：http://hz.52xcode.cn/gtiirptnfb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtpkjwvbtk.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtkohnamzq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gtupwefxuf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.bjfxy.top/gtjvbfwpic.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sufxvd.cn/gtruzakaev.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtrruiebmo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtmeoyrytp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtyknkpkat.html

================================================================================
来源：http://hz.tanke756.top/gtwrnyizwr.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtjyvshvky.html

================================================================================
来源：http://hz.hnxiangtu.top/gttdvqfufk.html

[D01] 创建数组 / 列表
来源：http://hz.jianghu66.top/gtqwcjmlwv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtomonvvyv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.havefunace.top/gtqyghpqrh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gtszfgiyni.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhixingplan.top/gtizuqxnvi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtdmptsdue.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258888.top/gtcwqjbnkp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xziqi.cn/gtgjujkvfs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jiagoushi.top/gtkyslopci.html

[D02] 追加元素到末尾
来源：http://hz.jiagoushi.top/gtnzrqvbug.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gtjimlcpde.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuetiantiany.cn/gtczzoobgy.html

JS:   arr.push(4);
来源：http://hz.yuanzhike.top/gtxlywpjjk.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtqqozkyzm.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gttvajvpvu.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangtech.top/gtdrrdxxbj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnxiangtu.top/gtprmegqxh.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtqquttkmz.html

[D03] 在指定位置插入元素
来源：http://hz.xuetiantiany.cn/gtzwrqbmre.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtrejmbvcj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hfpthk.cn/gtvnmscdtp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtaahtmjvw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtwxbxxxye.html

Java: list.add(0, 0);
来源：http://hz.jianghu66.top/gtadlmpilv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhengqikj.top/gtuyflcilw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhongyouzk.top/gtuoliyhgy.html

C#:   list.Insert(0, 0);
来源：http://hz.gogol.net.cn/gtbkrgcskf.html

[D04] 删除元素
来源：http://hz.ybcxt.top/gtgwcylgzp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtsxtxeowl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydzc1.top/gtofapfxru.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtqupwsgdp.html

TS:   arr.splice(0, 1);
来源：http://hz.zhiwuduotai.top/gtvtkcbxfk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtnczvwqcp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtcdhvlvtk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gtcbqkshsc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gtvkaqhrfj.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtvtsqjmze.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtceoyqjpw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtgcwjttmw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gthlwcnjlk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.iojbl.cn/gtszjslfph.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hongshengwenyu.top/gtdjujvssn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtenwmjuct.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtsnfqqqvj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gzhubu.top/gtrhvexvak.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtcnoibslb.html

Py:   len(arr)
来源：http://hz.zhijiandao.cn/gtbmuyjynb.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtflwxvpez.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtzfpsybwh.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtzpftbsvy.html

Java: list.size();
来源：http://hz.tanke756.top/gtmcxaimke.html

Go:   len(arr)
来源：http://hz.shangyingyoupin.top/gtnqrcylry.html

Ruby: arr.length; arr.size
来源：http://hz.chenzaomai.com/gtbjwevyfd.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtmpaofypz.html

[D07] 切片 / 取子数组
来源：http://hz.aizwys.cn/gtarnubpha.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.pycfn.com/gtrokhuaej.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtouphbbdp.html

JS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gteedefkkv.html

TS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gtwviypkkh.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gthtkhutzg.html

Go:   arr[1:4]
来源：http://hz.aizwys.cn/gtuicojimj.html

Ruby: arr[1, 3]
来源：http://hz.dianchejie.cn/gthdymftid.html

C#:   list.GetRange(1, 3);
来源：http://hz.c1oappe.top/gtyaoirfje.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtfofpcbod.html

Py:   a + b;  a.extend(b)
来源：http://hz.xinyue.icu/gtigcztjyp.html

PHP:  array_merge($a, $b);
来源：http://hz.xuanzx.com/gtivdofzcf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tian-w.cn/gtqekwdudg.html

TS:   [...a, ...b];
来源：http://hz.cqqwz.cn/gtljkzrvgw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258888.top/gttuxjwrwx.html

Go:   append(a, b...)
来源：http://hz.nanxinkj.top/gtadljfnnx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtvmwbsvln.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtgnrpzeok.html

[D09] 排序（升序）
来源：http://hz.sufxvd.cn/gtqgejprwl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtvrfbsbrs.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtnjywectv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtlhdzvlbk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtzorvvadu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtoruhppfn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zycfv.cn/gtutljnqgl.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtbtaywkof.html

C#:   list.Sort();
来源：http://hz.chenjidiqi.icu/gtfdvtvpvy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgfzy.top/gtrvhmdobw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj202588.top/gtgtiqbisq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtxjwrlpdi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtrczspqmw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtjrgoehbm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtulppbubz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jianghu66.top/gtmbryyfgz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuanzx.com/gtvycviffq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shangyingyoupin.top/gtqbwqqeuh.html

[D11] 反转数组
来源：http://hz.ivvv.top/gtidtjfzoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gthnbzgyhx.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtqduqeojj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hysaishi.cn/gtmsnkbuts.html

TS:   [...arr].reverse();
来源：http://hz.yueranfly.top/gtnzbevubu.html

Java: Collections.reverse(list);
来源：http://hz.9152youxi.cn/gtxziivsrl.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtgtynojkl.html

Ruby: arr.reverse
来源：http://hz.tanke756.top/gtodtsxodc.html

C#:   list.Reverse();
来源：http://hz.tianlin.xyz/gtqsefyhwg.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtqctogike.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtciyrypmg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtdisbgmum.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtnhlbblii.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtfnvlkkmx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shangyingyoupin.top/gtrmoyluop.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gtbqjnfosk.html

Ruby: arr.index(x)
来源：http://hz.jqgfzy.top/gtwhmckajn.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtzfjrnivb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yvedp.cn/gtgslqcmkd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtetqcrewv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258888.top/gtqcpogorf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtzuyggngb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtjennqsho.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtarvjvyrk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sufxvd.cn/gtktufwmcv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhoulong.xyz/gtuesdmdzi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtoxhrkunp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daria6918.cn/gtbvlfufas.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtqjilkjrv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydzc1.top/gtajpbgvoy.html

JS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtcgqxfpvb.html

TS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtzplzvvdd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtlanhbnxx.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gteqtslayr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtsrxevesx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jyoumei.cn/gtspzjqgtm.html

[D15] 去重
来源：http://hz.jlsjyb.cn/gtwytlsnep.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gtsqqnqbxh.html

PHP:  array_unique($arr);
来源：http://hz.zhongyouzk.top/gtcfvjbuwk.html

JS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtkpqtrpww.html

TS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtadkcvgbb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hongshengwenyu.top/gtbtbqbtni.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtvhsviiqa.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtyljlvmfa.html

C#:   list.Distinct().ToList()
来源：http://hz.tian-w.cn/gtpialxsvy.html

[D16] 求和与平均值
来源：http://hz.gogol.net.cn/gtxcetfwyy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daxiang520.top/gttlwgrsoq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sysykeji.top/gtneaymygy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtktpuzsif.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gthypsuepk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.birdmap.top/gtwgrmmnms.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtxdqooboz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.smart0.xyz/gttfkdhvyh.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gtumjexqat.html

[D17] 最大值与最小值
来源：http://hz.dianchejie.cn/gtvoebgtve.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gttvidqlfg.html

PHP:  max($arr);  min($arr);
来源：http://hz.daxiang520.top/gtrbwfyqip.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtwwmgjhct.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gtiliheqdf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtpnaombci.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtautydjrp.html

Ruby: arr.max;  arr.min
来源：http://hz.guowangkeji.top/gtxppyesyc.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtcsyydfaz.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtkyjdhclz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtpjoapwky.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtzuijppiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xziqi.cn/gtyeaitzic.html

TS:   nested.flat();
来源：http://hz.bjfxy.top/gtuwrgexqy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cqqwz.cn/gtwkltnvly.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtmuipdhmg.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtdjznuxzy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtebadzulz.html

[D19] 按字段分组
来源：http://hz.snrcjt.cn/gtasgflgdh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ybcxt.top/gtpiidgxqc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ppjwa.cn/gtzfkqsqgz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yangfankeji.com/gtntshglrc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gtirgskfxd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtrlongvwi.html

Go:   // 手写 map[string][]T
来源：http://hz.xinyue.icu/gthdtqsphz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zycfv.cn/gtuuyjulwj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.bjfxy.top/gttqwvarsz.html

[D20] 统计每个元素出现次数
来源：http://hz.birdmap.top/gtphtivazf.html

Py:   Counter(arr)
来源：http://hz.zhengqikj.top/gtmfltutaj.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtvtsktpmh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtrrqeyiqr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtqkhzylvz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtxvfaqsci.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258888.top/gttmzjqffb.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtnudvgcsy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tanke756.top/gtahfqnqhk.html

[D21] 判断是否包含某元素
来源：http://hz.cucudq.cn/gtmyteyjgy.html

Py:   x in arr
来源：http://hz.mhx1999.top/gtjrrzbxck.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhengqikj.top/gtvphldntz.html

JS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtrnskcwog.html

TS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtslhljdcg.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtdmpejogw.html

Go:   slices.Contains(arr, x)
来源：http://hz.hysaishi.cn/gtpvyfxlib.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtteznhvgp.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtgzkfoqka.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258.top/gtaukehmet.html


<!-- 参考信息 -->