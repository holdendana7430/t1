代发 wailian999

Py:   return a, b
来源：http://hz.yongpay.top/gtyitquuvx.html

PHP:  return [$a, $b];
来源：http://hz.wangshuangyany.cn/gtzuayabkb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fzhhl.top/gtrotsinhs.html

TS:   return { a, b };
来源：http://hz.bjfxy.top/gtwmhzmdyo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shuidangran.top/gtycewduhr.html

Go:   return a, b
来源：http://hz.feifeiyinyue.top/gtadmqeopa.html

Ruby: return a, b
来源：http://hz.wangdashe.top/gtebbjcgmk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258888.top/gtlwsnmzbt.html

[C06] 匿名函数 / lambda
来源：http://hz.hnxiangtu.top/gtbvixaxct.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtkinterjd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guannengcc.top/gtvlihjlcz.html

JS:   const square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtlgfgbutm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtwaiuwaoj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gtdkyoshmz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gtwdvvhwwh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gthnprohvz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jiagoushi.top/gtgoopllba.html

[C07] 把函数作为参数传入
来源：http://hz.chenzaomai.com/gtjbyzexfl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.316326.xyz/gtjoncroti.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.316326.xyz/gtsoisvqbm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtcofraiee.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gteyxlngiw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhixingplan.top/gtlzeqebsx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenlongwang.top/gthnvpqfky.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtdolweszf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnxiangtu.top/gtwqippjdy.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtjypmssxr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sweek.top/gtqpxdmwoz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgfzy.top/gttaijsybl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtboyvrjqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtrawdilen.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtqrfjejec.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aibaodan.cn/gtclmzavxb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gtfsvhgyxu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gthkzdpycg.html

[C09] 递归
来源：http://hz.hnqzz.top/gtpegcyzvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtfwnaljkr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.meibo888.top/gtpvvgxsya.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtmjdsxufu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtfcqjxcsq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtcqurrcjo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.feifeiyinyue.top/gtgzzwjfyo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yueranfly.top/gtiklnldwe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtabhhsknh.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtxthczmyn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sweek.top/gtdtbtvboo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj20258888.top/gtmlpzcbfj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xingfuxueyuan.xyz/gtvhslfrzf.html

TS:   同 JS
来源：http://hz.sysykeji.top/gtblhklavl.html

Java: 方法内为块级作用域
来源：http://hz.cashguo.top/gtyirnxenp.html

Go:   花括号块级作用域
来源：http://hz.iojbl.cn/gtczbviddx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydjk.org.cn/gtptlqdptn.html

C#:   块级作用域
来源：http://hz.hnqzz.top/gtmlmjcrjs.html

[C11] 模块导入与导出
来源：http://hz.feifeiyinyue.top/gtcmddjmda.html

Py:   from module import func
来源：http://hz.cdnleiting.top/gtmpupizmd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.0kj1m.cn/gtpurydofc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhixingplan.top/gtygjyvixq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtrhmfqiyl.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gtqrxnepvt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtifpacuzv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxinkj.top/gtmxcrlkes.html

C#:   using System.Text;
来源：http://hz.xuanzx.com/gticjkkxcc.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtjryeacen.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtcsgpbeyv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ivvv.top/gttqandnss.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtfaasdlqt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtqifjpnpw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtxbgqjxjp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtanlbhodo.html

Ruby: -> { puts "run" }.call
来源：http://hz.gogol.net.cn/gtdraaaaws.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.havefunace.top/gtlyarxhus.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydjk.org.cn/gthltpxxub.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xylfe.cn/gtiiypnrvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtfrpqprti.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtiqbmhvrt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtjdtcndna.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gttpynmnag.html

Go:   func add(a, b int) int
来源：http://hz.guowangkeji.top/gtgpokbowa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuetiantiany.cn/gtthybwyow.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhoulong.xyz/gtvokvtmhf.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtpopbdwph.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nwbrower.top/gtzrpggvwp.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtfqirlwbm.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtdetwkosw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtxrzywrhm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jianghu66.top/gtplqytvxp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtwbwyvcvx.html

Ruby: # 无泛型
来源：http://hz.shangyingyoupin.top/gtajnxmbqr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gthpygiyjs.html

[C15] 解构 / 展开参数
来源：http://hz.zhoulong.xyz/gtvoyswsig.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtkdnoteok.html

PHP:  [$a, $b] = $pair;
来源：http://hz.mhx1999.top/gtygvatetg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gzhubu.top/gtodsnwbnz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pycfn.com/gtsrjzbkty.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtfzbycncv.html

Go:   // 无解构
来源：http://hz.jlsjyb.cn/gtdndjgavx.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtqcdguzya.html

C#:   var (a, b) = pair;
来源：http://hz.pycfn.com/gtymzdgsdv.html

[C16] 函数 / 方法重载
来源：http://hz.chenzaomai.com/gtdmkroelu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtmsseacfh.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gthpryakpp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gtsqjqasli.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gteyzbueis.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hongshengwenyu.top/gtletrvvth.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenlongwang.top/gtmfscnvpz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtetsvgacf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.dashuyun.cn/gtiukvlgup.html

================================================================================
来源：http://hz.bjfxy.top/gtbhyeauvx.html

D. 数组 / 列表 / 集合
来源：http://hz.aibaodan.cn/gtxtxboxom.html

================================================================================
来源：http://hz.yj202588.top/gtkloddmiw.html

[D01] 创建数组 / 列表
来源：http://hz.pycfn.com/gtmiuhkcxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gtxopnmcfy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gtqgelkedx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenzaomai.com/gtiqxiwafm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtdtsqepuc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.bjfxy.top/gtusaqdwvq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtczjsfyvy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gtawcxwywf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtixifxgds.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gtmovxycqw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gtpjlicccq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtqfqknxpf.html

JS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtkomqhvzr.html

TS:   arr.push(4);
来源：http://hz.fengsongda.top/gtdekwtjqq.html

Java: list.add(4);
来源：http://hz.hysaishi.cn/gtnjyjyvyu.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtfuifsboh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtijkaznuf.html

C#:   list.Add(4);
来源：http://hz.zdqjudy.top/gtlspgzqex.html

[D03] 在指定位置插入元素
来源：http://hz.ybcxt.top/gtmfrdcxep.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtknximtgq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shangyingyoupin.top/gthqbcmwct.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.mhx1999.top/gthackfawb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gtulnzskla.html

Java: list.add(0, 0);
来源：http://hz.zhijiandao.cn/gtzsezshff.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtmrgejhxq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gtwzqwbgbp.html

C#:   list.Insert(0, 0);
来源：http://hz.pycfn.com/gtyxcvmdqq.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gtcltjtcfi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinyuanbaomall.cn/gthkysujzp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.kuanghao11.cn/gtsrmdstgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuanzx.com/gtqbssrbki.html

TS:   arr.splice(0, 1);
来源：http://hz.dashuyun.cn/gtqvljgqoh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yueranfly.top/gtpelzvlnw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gttsbxjvel.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gtivsswfsu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtuvcyjnka.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gtyexerpeq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtyiactltx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtatbsnjng.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtuugzjpmw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yangfankeji.com/gtoarzhlsu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gtvsrloeku.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtgwjmyytu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtyhbexjet.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtcxssgmvg.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtfyfgsmvd.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtlegbxcon.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtqhutlzgu.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtyanvuogq.html

TS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtbtbcuwyd.html

Java: list.size();
来源：http://hz.jinqigfzy.top/gtdbnlwkcg.html

Go:   len(arr)
来源：http://hz.dianchejie.cn/gtttynegcg.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtximvbyut.html

C#:   list.Count;
来源：http://hz.sufxvd.cn/gtomvpuhxr.html

[D07] 切片 / 取子数组
来源：http://hz.zhixingplan.top/gtmgobwwya.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dashuyun.cn/gtxlguuaau.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtiikgairt.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtbiebqddd.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtbvjkaxoy.html

Java: list.subList(1, 4);
来源：http://hz.aibaodan.cn/gtankpbstz.html

Go:   arr[1:4]
来源：http://hz.iojbl.cn/gtebipvlai.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtdxlwfxmb.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gtcjpcffzu.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtrdtyztnq.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtgpgxdhdz.html

PHP:  array_merge($a, $b);
来源：http://hz.xingfuxueyuan.xyz/gtnywkpwht.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.iojbl.cn/gtbbatsyzv.html

TS:   [...a, ...b];
来源：http://hz.smart0.xyz/gtyxufujaa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.kuanghao11.cn/gtwhmwsssk.html

Go:   append(a, b...)
来源：http://hz.guannengcc.top/gthilfsedn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtxgcqvegi.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtflyupbdv.html

[D09] 排序（升序）
来源：http://hz.redwolf501.top/gtuqhrplqy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtrpsldzyo.html

PHP:  sort($arr);
来源：http://hz.cheryme.top/gtecqeazxr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xinyue.icu/gtwwlysgmv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xinyue.icu/gtwjsdvanp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtfvcvexzn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtqgjianzy.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtwlurcvfs.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtrsextjdf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuxming.cn/gtujfjogyw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.316326.xyz/gthppuajdn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yanxiufei.cn/gtrlyfwspa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtyzffpdiy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtxugghnbt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gtpezlmlrw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zycfv.cn/gtfrfhrcxc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtdfavnsub.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtlmuaqqne.html

[D11] 反转数组
来源：http://hz.nwbrower.top/gtgozxtwni.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tanke756.top/gtspcwtbvv.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gteefzmzij.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jqgufenzy.top/gtkrqbykwa.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtrjewrhoo.html

Java: Collections.reverse(list);
来源：http://hz.wangdashe.top/gtltznbgtb.html

Go:   slices.Reverse(arr)
来源：http://hz.jiagoushi.top/gtvhmheijs.html

Ruby: arr.reverse
来源：http://hz.shuidangran.top/gtmmqwthje.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangtech.top/gtqhvhjrwu.html

[D12] 查找元素下标
来源：http://hz.haohaochexian.top/gtdlnhopmf.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtrolsixsj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gaohongyu789.top/gtebouaofn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gthvjkhbnm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtfggigntg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtiedvrarg.html

Go:   slices.Index(arr, x)
来源：http://hz.smart0.xyz/gtbzuutvej.html

Ruby: arr.index(x)
来源：http://hz.zdqjudy.top/gtqzlxhmys.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtqtcdidab.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj202588.top/gtbeulomzr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tian-w.cn/gtbfisbfzk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtmcplhdqg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtgpghsgvw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gthutjuuze.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258888.top/gtclcpliam.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cucudq.cn/gtcvvezlwb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtueaztomj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuanzhike.top/gtphnnyjmh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jyoumei.cn/gtczsgrcqp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gtrxyhiquk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtxajprgxq.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtbtoqseki.html

TS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtrzjwaioh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtlnogyctk.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtiwkxuztb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gteyciekdg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenjidiqi.icu/gtkntygfsi.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtbaoesdpx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtssulmxiq.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtetodcezp.html

JS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtjxkdawzd.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtqqzsckgf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.svipenyu.cn/gtjncpcess.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxuanxn.top/gtjxxmiczk.html

Ruby: arr.uniq
来源：http://hz.quarkkingdee.top/gtftauxcdf.html

C#:   list.Distinct().ToList()
来源：http://hz.hywenlv.cn/gtvxzlqyfs.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtkgiqowrs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtmstkgltc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnxiangtu.top/gtxmcuelvj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtupyxqyvt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtthqhuess.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.vqdsnc.cn/gtvyqfrkfi.html

Go:   // 手写循环累加
来源：http://hz.zhongyouzk.top/gtfqwzdzex.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.316326.xyz/gtstdtplui.html

C#:   list.Sum();  list.Average()
来源：http://hz.nwbrower.top/gthrkqosbk.html

[D17] 最大值与最小值
来源：http://hz.zhoulong.xyz/gtwdpgybvi.html

Py:   max(arr);  min(arr)
来源：http://hz.chenjidiqi.icu/gtwoazbhlp.html

PHP:  max($arr);  min($arr);
来源：http://hz.sufxvd.cn/gtyxazgauk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hnqzz.top/gtxdakhjms.html

TS:   Math.max(...arr);
来源：http://hz.9152youxi.cn/gtskzdozxn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gthvkyjfwv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtqupxhqdt.html

Ruby: arr.max;  arr.min
来源：http://hz.52xcode.cn/gtwixbdlqe.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtximbvtno.html

[D18] 扁平化嵌套数组
来源：http://hz.hnqzz.top/gtmtccmjcz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinqigfzy.top/gtisvjlcwz.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtqhrrvxwo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtysktasim.html

TS:   nested.flat();
来源：http://hz.fzhhl.top/gtpzzxdqrn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sweek.top/gtoykfgqnx.html

Go:   // 手写双层循环
来源：http://hz.cdnleiting.top/gtoqcwglnc.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gthdtoqbyx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shuidangran.top/gturwvzqsi.html

[D19] 按字段分组
来源：http://hz.ydjk.org.cn/gtjoedcshk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtfyrystwm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.c1oappe.top/gtgddnltcx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydjk.org.cn/gtxvsjplnx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtikznzyho.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shangyingyoupin.top/gtcivsvpwz.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258.top/gtxfdorfgr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zycfv.cn/gtjhvkvpyf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hammf.cn/gtqxynhkqf.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gttwkmlbpt.html

Py:   Counter(arr)
来源：http://hz.jinqigfzy.top/gtrrkgpfxh.html

PHP:  array_count_values($arr);
来源：http://hz.guowangkeji.top/gtiiexqqsn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtnubvphnm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtxgstdpzw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtlwanupbl.html

Go:   // 手写 map[T]int
来源：http://hz.jinghuilouyu.cn/gtljmoqvki.html

Ruby: arr.tally
来源：http://hz.shanyushiyangkeji.top/gtblwhfocr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tian-w.cn/gtsjiomwix.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gtrmdidfln.html

Py:   x in arr
来源：http://hz.jqgfzy.top/gtdvdbdtft.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtqnqetlik.html

JS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtohmmxvid.html

TS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtlofzjdoh.html

Java: list.contains(x)
来源：http://hz.bjfxy.top/gtbwhrrokm.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtsveohdra.html

Ruby: arr.include?(x)
来源：http://hz.cdnleiting.top/gtqdsokyfq.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtrultbxcg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangkeji.top/gtyqpoxjdt.html


<!-- 参考信息 -->