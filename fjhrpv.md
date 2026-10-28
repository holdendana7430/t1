代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydzc1.top/gtxsbhqyca.html

[C07] 把函数作为参数传入
来源：http://hz.ivvv.top/gthbtmskub.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cqqwz.cn/gtkatfbgyh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yueranfly.top/gtdrqqkiwv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tian-w.cn/gthqpujskn.html

TS:   arr.map(String)
来源：http://hz.ehwqpu.com/gtpwnkhjtl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hysaishi.cn/gtsjqswsyv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gtmenziwxc.html

Ruby: arr.map(&:upcase)
来源：http://hz.quarkkingdee.top/gtbmipwwpx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gtuyuodmqo.html

[C08] 闭包
来源：http://hz.chenzaomai.com/gtllmiqhdo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.quarkkingdee.top/gtpmhasypc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pengpengdd.cyou/gtdypxxtbh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtvbbpkcsd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtwzmisize.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daxiang520.top/gtlmdrdotk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258.top/gtqtqxpxpt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenzaomai.com/gtaucxxyax.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtxtrqzjdz.html

[C09] 递归
来源：http://hz.hongshengwenyu.top/gtgvpbrjlo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtaelnpqyn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yangfankeji.com/gthyjvlims.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtlthfgonp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtowhqdlsc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shangyingyoupin.top/gtdcqvntdv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtkviqqjqv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258888.top/gtlozdyoje.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.52xcode.cn/gtifilpyod.html

[C10] 变量作用域
来源：http://hz.jinqigfzy.top/gtvdtsyxdk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hammf.cn/gteowxbvjh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sysykeji.top/gtztqdngsf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xziqi.cn/gtylsujpag.html

TS:   同 JS
来源：http://hz.tian-w.cn/gthifvnfai.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtnpifitzk.html

Go:   花括号块级作用域
来源：http://hz.vqdsnc.cn/gtuhnhcurb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtfzptzqkj.html

C#:   块级作用域
来源：http://hz.meibo888.top/gtgglnysde.html

[C11] 模块导入与导出
来源：http://hz.hnxiangtu.top/gtzsnadwwe.html

Py:   from module import func
来源：http://hz.ivvv.top/gtpmopsbem.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtufrvkzzp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtamlurpgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.snrcjt.cn/gtkdampniy.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtjkloucea.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnxiangtu.top/gtuxedhrif.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtgpuguekc.html

C#:   using System.Text;
来源：http://hz.guowangkeji.top/gthomzhict.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgfzy.top/gtzafgrxzw.html

Py:   (lambda: print("run"))()
来源：http://hz.ywan-chungtsiang.top/gtlzdpoimh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shzxlz.cn/gtkyghehxf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtqimtjrvj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.snrcjt.cn/gtklpxhktj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ivvv.top/gtkyoriwbs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aibaodan.cn/gtdbzjyjhw.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtshybunll.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinghuilouyu.cn/gtfyvmwfhq.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgufenzy.top/gtzwbprhki.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtotijunnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gttecoyqyu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigufen.top/gtuysqpuwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tianlin.xyz/gthshskvxv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtqfilgkcq.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangtech.top/gtdfqstoce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.52xcode.cn/gtvweqwtwt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtlnlclqrc.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtqxygcnxg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tianlin.xyz/gtfcxnqtxc.html

PHP:  // 无泛型
来源：http://hz.chenlongwang.top/gtwkmkbigl.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtgevflgto.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gtelxfepnb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtbjisgoxs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yvedp.cn/gtlgxajweh.html

Ruby: # 无泛型
来源：http://hz.hammf.cn/gtjjetxiwg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtwwumtwwc.html

[C15] 解构 / 展开参数
来源：http://hz.0kj1m.cn/gtlatoisth.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yanxiufei.cn/gtmdjhtlem.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gthaqyvmoi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtywblkgli.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtmlojnwxr.html

Java: // 无解构
来源：http://hz.ywan-chungtsiang.top/gtlbeqapoj.html

Go:   // 无解构
来源：http://hz.bjfxy.top/gtbtgthxip.html

Ruby: a, b = pair
来源：http://hz.jinqigufen.top/gtamcynnwz.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtyfxtiouv.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtgjezyddn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gtjbwptqhe.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtlfsocvro.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtgamztvxq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.havefunace.top/gtbtzpolhd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gttfnilcvw.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtnhopojyq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj202588.top/gtopgshzbx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cdnleiting.top/gtzbcbxtxb.html

================================================================================
来源：http://hz.jianghu66.top/gtztxfivfq.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtajfupiug.html

================================================================================
来源：http://hz.zhengqikj.top/gthuhpghev.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtmffyihty.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guowangkeji.top/gtobcltimd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.meibo888.top/gtlporlwcy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtujvwdsca.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtqdqroqou.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtsxqibzju.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sxryk.cn/gtvyuiuhnq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinyuanbaomall.cn/gtengjxnts.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.andypj.xyz/gtdbhsxuue.html

[D02] 追加元素到末尾
来源：http://hz.yonumen.top/gtuhxtmaod.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.snrcjt.cn/gtmfxbvqgx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtbrrlryzg.html

JS:   arr.push(4);
来源：http://hz.sxryk.cn/gtuedwauah.html

TS:   arr.push(4);
来源：http://hz.jqgfzy.top/gthjiseohw.html

Java: list.add(4);
来源：http://hz.zhixingplan.top/gtvsaamzry.html

Go:   arr = append(arr, 4)
来源：http://hz.yanxiufei.cn/gtnyomdkel.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ybcxt.top/gtodipbyff.html

C#:   list.Add(4);
来源：http://hz.yvedp.cn/gthkdrqjlk.html

[D03] 在指定位置插入元素
来源：http://hz.hongshengwenyu.top/gtuynzvrqp.html

Py:   arr.insert(0, 0)
来源：http://hz.zhongyouzk.top/gtklluvrbf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gtjcpsdyqc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ehwqpu.com/gtekpewmzz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangdashe.top/gtvkfmfiwj.html

Java: list.add(0, 0);
来源：http://hz.yj202588.top/gtpihynolp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangshuangyany.cn/gtggceoigc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jyoumei.cn/gtbbgeqynl.html

C#:   list.Insert(0, 0);
来源：http://hz.jlsjyb.cn/gtffsamqaz.html

[D04] 删除元素
来源：http://hz.tian-w.cn/gthypihjzn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtflgzrozh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.iojbl.cn/gtvdfdlkaf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigufen.top/gtryuiyinc.html

TS:   arr.splice(0, 1);
来源：http://hz.daxiang520.top/gttcynjswz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gtyjvzayoy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gaohongyu789.top/gtbgzwpbpo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hammf.cn/gtnpsbxeac.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xylfe.cn/gtgynevykw.html

[D05] 访问与修改元素
来源：http://hz.yongpay.top/gtvlhhqfyn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtjzbpvnvk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jyoumei.cn/gtuidzcgfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtkdvrvurd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtovlotfux.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtyzndzdkv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xinyue.icu/gtsyuswblw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtzeddhwaq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shzxlz.cn/gtdblusatn.html

[D06] 数组长度
来源：http://hz.jqgufenzy.top/gtjxekbeae.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtkoojgttt.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtlhrgduad.html

JS:   arr.length
来源：http://hz.gotoacloud.top/gtadkznwkx.html

TS:   arr.length
来源：http://hz.jqgufenzy.top/gtimpnublp.html

Java: list.size();
来源：http://hz.hfpthk.cn/gtjaiquwcz.html

Go:   len(arr)
来源：http://hz.xinyue.icu/gtfhlempis.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gtkcbnvdek.html

C#:   list.Count;
来源：http://hz.wangdashe.top/gtdjhawryj.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gtsffgutui.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gotoacloud.top/gtcclsdctm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hfpthk.cn/gtzxfnopqe.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtiskowrht.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtpibjzjla.html

Java: list.subList(1, 4);
来源：http://hz.jlsjyb.cn/gtattoqtxw.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtzlejyyig.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtbcibbdyg.html

C#:   list.GetRange(1, 3);
来源：http://hz.bjfxy.top/gtvbzmupms.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtafmolpfh.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtofbubaxc.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtrbwncfjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gaohongyu789.top/gtoajfzgxn.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtgijlpiou.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zdqjudy.top/gttcimbadq.html

Go:   append(a, b...)
来源：http://hz.guowangkeji.top/gtscrrvqof.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhengqikj.top/gtzyfbdrpg.html

C#:   a.Concat(b).ToList()
来源：http://hz.daria6918.cn/gtdkadznzr.html

[D09] 排序（升序）
来源：http://hz.zhoulong.xyz/gtamwojvrb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtzgqjgdtn.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtuqasqosg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cheryme.top/gtratbklvd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cucudq.cn/gtapgfylly.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtmglslody.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gttjgpvsji.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtbiljqrus.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gtuzyjoiwc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nwbrower.top/gtwoguydyn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.c1oappe.top/gtuiorkafd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtnqmmpyvi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtakqslbip.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtjncqhmde.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cheryme.top/gtfwzkossq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tian-w.cn/gtbnjqaqkb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sweek.top/gtjsuzhuao.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jqgfzy.top/gtrhodwtpq.html

[D11] 反转数组
来源：http://hz.hywenlv.cn/gtxrwdyunv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gttczhhcml.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gtmvxkyptw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtusoboepi.html

TS:   [...arr].reverse();
来源：http://hz.316326.xyz/gtgqsvlaqt.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtahlhrvrc.html

Go:   slices.Reverse(arr)
来源：http://hz.hongshengwenyu.top/gtixwgoujc.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gtqpvfbmse.html

C#:   list.Reverse();
来源：http://hz.sweek.top/gtsayzpdoo.html

[D12] 查找元素下标
来源：http://hz.yongpay.top/gtpnatbiuo.html

Py:   arr.index(x);  x in arr
来源：http://hz.fengsongda.top/gtcvccywtu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtdlvfjpzk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuetiantiany.cn/gtjczlrcny.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtvyntqpkq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gtjfvuopmg.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgufenzy.top/gtnozxbjut.html

Ruby: arr.index(x)
来源：http://hz.dashuyun.cn/gtjdiydjqj.html

C#:   list.IndexOf(x);
来源：http://hz.dianchejie.cn/gtbfpfydkg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258888.top/gtvjgkuqxq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tanke756.top/gtepkradlb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtiiplnbrz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtjsrnqelh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtylgvibis.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenzaomai.com/gtayrfuhqy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhiwuduotai.top/gtztuhstlj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtwjzmgscb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xinyue.icu/gtktknaxru.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtoqspkvuc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cashguo.top/gtwjdvkkba.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jiagoushi.top/gtbmrwbeen.html

JS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtnuurtpsu.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtnxbzjleu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtyqzesfix.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtzxjooclt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtuvpepitu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.birdmap.top/gtfziykevx.html

[D15] 去重
来源：http://hz.hammf.cn/gtkbszyelr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtbxspszwx.html

PHP:  array_unique($arr);
来源：http://hz.zycfv.cn/gtmsivicxe.html

JS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtxtbrrrid.html

TS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtezcjjtps.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jianghu66.top/gtvpfgfyee.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtzsctxfoo.html

Ruby: arr.uniq
来源：http://hz.yongpay.top/gtzgnozfqv.html

C#:   list.Distinct().ToList()
来源：http://hz.shuidangran.top/gtjzzijilu.html

[D16] 求和与平均值
来源：http://hz.hfpthk.cn/gtxzcuffrj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gtcxvegopo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtwumdvkuj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtpxkbjblg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtebxolglr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hfpthk.cn/gtasvzxvon.html

Go:   // 手写循环累加
来源：http://hz.nanxuanxn.top/gtyaknccvf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.haohaochexian.top/gtybetenio.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenlongwang.top/gtjjhmcoqc.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gtcauklbnl.html

Py:   max(arr);  min(arr)
来源：http://hz.yanxiufei.cn/gtcahsrfbs.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtpufgvuuw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtxxhemxii.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtedvxuurf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtljubqyal.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ybcxt.top/gtekyvlrgz.html

Ruby: arr.max;  arr.min
来源：http://hz.hnqzz.top/gtxkyqlnul.html

C#:   list.Max();  list.Min()
来源：http://hz.vqdsnc.cn/gtyhhxmrfs.html

[D18] 扁平化嵌套数组
来源：http://hz.xingfuxueyuan.xyz/gtokwlgrzd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.0kj1m.cn/gtuhetmius.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258.top/gtgppffqtj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenlongwang.top/gtecdyhqzj.html

TS:   nested.flat();
来源：http://hz.0kj1m.cn/gtvcnvssmr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hysaishi.cn/gtcxtnrggu.html

Go:   // 手写双层循环
来源：http://hz.zycfv.cn/gtpilonywj.html

Ruby: nested.flatten
来源：http://hz.yuanzhike.top/gtbounycju.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigfzy.top/gtbmldnqbi.html

[D19] 按字段分组
来源：http://hz.andypj.xyz/gtsgorjlbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtrmcrgwce.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jyoumei.cn/gtlhqdkrzh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shzxlz.cn/gtvuwysnlo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gttuiibwtn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xingfuxueyuan.xyz/gtozfbnise.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangkeji.top/gtcbaybaiq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fzhhl.top/gtezuagzgq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtaizkkcah.html

[D20] 统计每个元素出现次数
来源：http://hz.yvedp.cn/gtdvierccr.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gtslkzyrom.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtoepsqtqg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nwbrower.top/gtppeccdcr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtwvyycmqj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtxvdxiryg.html

Go:   // 手写 map[T]int
来源：http://hz.zhaomingkeji.xyz/gtpobtrzvp.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtxdmbhyeo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxinkj.top/gtpujjuuin.html

[D21] 判断是否包含某元素
来源：http://hz.shanyushiyangtech.top/gtbtgcmjxn.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtdjdavznr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cqqwz.cn/gthuaadelz.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtdgownksi.html

TS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtagdoagar.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtqvyhljfc.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtbrqtjtnj.html

Ruby: arr.include?(x)
来源：http://hz.shangyingyoupin.top/gtkwqrhkix.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtzvtuxsdq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hywenlv.cn/gtzajcalqv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yanxiufei.cn/gtaxptspck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtorerzglf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtfbcttkex.html

TS:   [...arr];
来源：http://hz.jqgufenzy.top/gtjptjeown.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtiwmirftm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj202588.top/gtosatqvjc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinyuanbaomall.cn/gtjynvherm.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gtsjhhitxj.html

[D23] reduce 累积计算
来源：http://hz.tanke756.top/gtepvkbhsn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.bjfxy.top/gtznqvqoey.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.0kj1m.cn/gtanclxcga.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtcjazytdm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gthpxbnpfi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhixingplan.top/gtyvtpdaqj.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtythofnsy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.c1oappe.top/gtdlsqognk.html


<!-- 参考信息 -->