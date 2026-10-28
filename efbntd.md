代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.yuanzhike.top/gtphqwcmjo.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtfytewinc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gtsnjpcybu.html

JS:   const square = x => x * x;
来源：http://hz.jiagoushi.top/gtmtgpgsta.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cdnleiting.top/gtancqrwrv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtbpvxetkz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zdqjudy.top/gtwnavwmgr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jlsjyb.cn/gtlclwkvin.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xinyue.icu/gtxyebcmgy.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gtmsxdouds.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fzhhl.top/gtotietqlo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jyoumei.cn/gtelpqpdsv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtbaiitekj.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtmdsvbnsx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ehwqpu.com/gttavpugiq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aibaodan.cn/gtjqgejeky.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gthsmimbyz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dianchejie.cn/gtpscxccpe.html

[C08] 闭包
来源：http://hz.zhongyouzk.top/gtvwrizuit.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.smart0.xyz/gtdqlpoplc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gttuewuwiq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gttburniwa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtalxagotz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxinkj.top/gtxngxbnic.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.feifeiyinyue.top/gtcbvhcwyr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tianlin.xyz/gtkbmbmhld.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtpzhikfcv.html

[C09] 递归
来源：http://hz.hammf.cn/gtecfyflqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtmtixzzfp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtmeecksqk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtqqzsydgf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtlrilyjhv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aizwys.cn/gtyiuhgtvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtwaiyosrd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.meibo888.top/gtyaykdkir.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jqgfzy.top/gtbgoizzkt.html

[C10] 变量作用域
来源：http://hz.hysaishi.cn/gtuxntvumj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yanxiufei.cn/gtevhvsnpx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gthgqniyal.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258.top/gtezjglzha.html

TS:   同 JS
来源：http://hz.gogol.net.cn/gtdqdjkfbl.html

Java: 方法内为块级作用域
来源：http://hz.sysykeji.top/gtsgpjksbe.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gthrwwjlfl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtopuflmok.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtaifolbao.html

[C11] 模块导入与导出
来源：http://hz.wangshuangyany.cn/gtskklblzc.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gttktkcdab.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhiwuduotai.top/gtumhqwqum.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtcqklwawt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxuanxn.top/gtjssufzaj.html

Java: import java.util.List;
来源：http://hz.nanxinkj.top/gtkafqhgbd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gtdusmotad.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ybcxt.top/gtnlwomidb.html

C#:   using System.Text;
来源：http://hz.zhaomingkeji.xyz/gtbhccguyh.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtrlgsgkxo.html

Py:   (lambda: print("run"))()
来源：http://hz.sysykeji.top/gtzmavglwr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.snrcjt.cn/gtyzwctcza.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtyinzhxvt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtqkbfhpqw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtnfpqhmtv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangtech.top/gtdtfhqorj.html

Ruby: -> { puts "run" }.call
来源：http://hz.nwbrower.top/gtpwaolyvo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxinkj.top/gtjrpfboqg.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtnmiorztc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtojtoutvd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtxiaavtww.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtkhjxhqrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtqfkcpdzu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtazoizuek.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtaculvdkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtduivqmrj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.haohaochexian.top/gtjpzxcjpi.html

[C14] 泛型函数
来源：http://hz.yangfankeji.com/gtvrpfpfpd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtofhodsjo.html

PHP:  // 无泛型
来源：http://hz.svipenyu.cn/gtwhtqezwy.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtfxmyykxu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydjk.org.cn/gtictyifzz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhongyouzk.top/gtmvlgyxxz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtkjofekxd.html

Ruby: # 无泛型
来源：http://hz.iojbl.cn/gtntpnfpff.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gtdjwrxbdj.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gttmzozhdg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jyoumei.cn/gttvrgfslh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuanzhike.top/gtwuszogwe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtumnfgivx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenzaomai.com/gtiwpzutcu.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtsjokmidx.html

Go:   // 无解构
来源：http://hz.ppjwa.cn/gtryuqnizr.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gtervrbexk.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtopuontwh.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gteayjddwy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xziqi.cn/gtalasmqsi.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtvmzoqtlk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cashguo.top/gtuvtzyawf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtyyodyaez.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnqzz.top/gtelqzjlmz.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gttvuaynff.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gtsbmhkvdn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cdnleiting.top/gtbeceoqdj.html

================================================================================
来源：http://hz.gotoacloud.top/gthgadwcgg.html

D. 数组 / 列表 / 集合
来源：http://hz.tian-w.cn/gtrfhnfjnq.html

================================================================================
来源：http://hz.havefunace.top/gtsxmhgdsi.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigfzy.top/gtghduedoz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gtjffotxxu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gttbxrcbgx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.meibo888.top/gtdywcroxo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gtrcksusob.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aibaodan.cn/gtriewkayh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtnuampqys.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtpeprrrsz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigfzy.top/gtmasskcib.html

[D02] 追加元素到末尾
来源：http://hz.yuxming.cn/gtlyxzjtgu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtrgnrvtan.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yangfankeji.com/gtcgzysjpb.html

JS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtzckurefv.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtafowydgf.html

Java: list.add(4);
来源：http://hz.daria6918.cn/gtqsukqldd.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtkcfmpiid.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yangfankeji.com/gtvhzuloxm.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtqhaqbwol.html

[D03] 在指定位置插入元素
来源：http://hz.haohaochexian.top/gtfkakpqjy.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtaqbhsdls.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gtcqnwjpcf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gtzzhesmkc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhongyouzk.top/gtbsioxwul.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtcofkbntk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhengqikj.top/gttkulmmlw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yanxiufei.cn/gtzyaaslzc.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtjwfffizf.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtzvuzqlwi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtcxcvmkas.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtitmdvdql.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ivvv.top/gtaonypqsw.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtaiimeoqv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhongyouzk.top/gtycudwnzh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.haohaochexian.top/gthnzoopww.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtgesmkzgw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gaohongyu789.top/gtymkrafqz.html

[D05] 访问与修改元素
来源：http://hz.hysaishi.cn/gtcafhefqr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gteorpxujv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtpjcxxdqv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtmfutzzeb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinghuilouyu.cn/gtcjnmhxyp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.redwolf501.top/gtisiqomwi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtrygrikzv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtwbwbiuwh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dianchejie.cn/gtpjxucnns.html

[D06] 数组长度
来源：http://hz.gogol.net.cn/gtvdsstmop.html

Py:   len(arr)
来源：http://hz.xuetiantiany.cn/gtzbvmgczf.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtwqgrzian.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtnpnkzdue.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtxlgpjswn.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtwkepwdxs.html

Go:   len(arr)
来源：http://hz.dianchejie.cn/gtllhruhwu.html

Ruby: arr.length; arr.size
来源：http://hz.chenjidiqi.icu/gtnjojkszx.html

C#:   list.Count;
来源：http://hz.hfpthk.cn/gtklbeapfc.html

[D07] 切片 / 取子数组
来源：http://hz.svipenyu.cn/gtibdcnjkq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gthrcrxmno.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtdumcbanx.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtaheigqdu.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtyzpkavgu.html

Java: list.subList(1, 4);
来源：http://hz.jqgfzy.top/gtzgzusgft.html

Go:   arr[1:4]
来源：http://hz.yj202588.top/gtenhyoqju.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gtynhngkmo.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtlkzqiyyc.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtnqcvbkdt.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtwujbfcrw.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtkxbwdmco.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtkytobkpw.html

TS:   [...a, ...b];
来源：http://hz.jinqigfzy.top/gtgxrkemxt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtkigngxsg.html

Go:   append(a, b...)
来源：http://hz.ydzc1.top/gtybwgghkx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuanzx.com/gtrcnrolyy.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtbwvtdhqz.html

[D09] 排序（升序）
来源：http://hz.aizwys.cn/gtqjfjkvjt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtepcvgkry.html

PHP:  sort($arr);
来源：http://hz.yangfankeji.com/gtalbamkzm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtxopddqpc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtdmfhltbz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtzwctqrzp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtcqhsyyih.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gthyuwrgxp.html

C#:   list.Sort();
来源：http://hz.redwolf501.top/gtyjofsagq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtqcqhhhab.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tian-w.cn/gtruxgivop.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtvdhqlodo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtmmnkdvkx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtkkgcspqb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dianchejie.cn/gtkvggmjcg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigfzy.top/gtapwmklkw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgufenzy.top/gtxxlagudo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yueranfly.top/gttuhgriqc.html

[D11] 反转数组
来源：http://hz.c1oappe.top/gtatbfghzx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jiagoushi.top/gthsjbllau.html

PHP:  array_reverse($arr);
来源：http://hz.guannengcc.top/gtzuejihke.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gtdmxwleev.html

TS:   [...arr].reverse();
来源：http://hz.aizwys.cn/gtkuvjrczy.html

Java: Collections.reverse(list);
来源：http://hz.pengpengdd.cyou/gtcmmxozsj.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtnqswwexf.html

Ruby: arr.reverse
来源：http://hz.yvedp.cn/gtovhxqbur.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gthswtcmmt.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtzrtubwfa.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtqxmktfzi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtfbfbwcms.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtdrkmoupa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtotqxzarg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zdqjudy.top/gtjwiaubfx.html

Go:   slices.Index(arr, x)
来源：http://hz.iojbl.cn/gtoklebxjo.html

Ruby: arr.index(x)
来源：http://hz.hfpthk.cn/gtlowffkzf.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gtikoglpxr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.feifeiyinyue.top/gtxbcglhep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtuatyahni.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gttpqpgzby.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtupvdseje.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtecmidion.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jyoumei.cn/gtrsesljjz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dianchejie.cn/gtmepqlmmv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jlsjyb.cn/gtrszemznv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shuidangran.top/gtiuvlbkeu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xuanzx.com/gtenjuusqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtwxyxcugr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.vqdsnc.cn/gtipfgvyox.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtdfxydwlk.html

TS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtummyvckk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gthkvigcpd.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gttycvgwcm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtnasetdhh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aizwys.cn/gtonhrpgzj.html

[D15] 去重
来源：http://hz.mhx1999.top/gtrmoaxtpb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtanmckjch.html

PHP:  array_unique($arr);
来源：http://hz.meibo888.top/gtcuwvpjbg.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtnuuvmnaq.html

TS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gthhdgejfn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgfzy.top/gtxmrqttmx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtzhzuwxcj.html

Ruby: arr.uniq
来源：http://hz.sxryk.cn/gtjocgheci.html

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gtbngicsfz.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtagwriamu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtnvlutbww.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangtech.top/gtfizbddpw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtwteknbjy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtxrpcjkmz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.meibo888.top/gtqeqauqsl.html

Go:   // 手写循环累加
来源：http://hz.guannengcc.top/gtcfoannmb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxinkj.top/gtqehycdtr.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtgtcyryxa.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtiggfplfz.html

Py:   max(arr);  min(arr)
来源：http://hz.jinyuanbaomall.cn/gtrkaedmmc.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtkxymscvn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtzbztvyvw.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtcuwqpavf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtwxtldpej.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtxqfjttxs.html

Ruby: arr.max;  arr.min
来源：http://hz.yonumen.top/gtxgwesicb.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtrpawrcpn.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gtnvbupabk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.feifeiyinyue.top/gthudobccq.html

PHP:  array_merge(...$nested);
来源：http://hz.hnxiangtu.top/gtujauidcf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258888.top/gtyglpftkb.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtuggtelkd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtcyuymtpl.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtckbkwbjh.html

Ruby: nested.flatten
来源：http://hz.jqgufenzy.top/gtmxvqewtj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shanyushiyangtech.top/gtqlwwpqof.html

[D19] 按字段分组
来源：http://hz.xinyue.icu/gtlflkqzkk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtqdtqpjlk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daria6918.cn/gtnoeirrfg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhiwuduotai.top/gtfxploqfn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtphpaltfv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.kuanghao11.cn/gtslgflhya.html

Go:   // 手写 map[string][]T
来源：http://hz.tanke756.top/gtjzurgncq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtugxwofeu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.vqdsnc.cn/gtsmmxsxgi.html

[D20] 统计每个元素出现次数
来源：http://hz.vqdsnc.cn/gttnndpulu.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtlaaesrkf.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gtxmohorrm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tian-w.cn/gtwtnkzwtd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtoyvuxnsr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtfohnnfpg.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtqaqrisby.html

Ruby: arr.tally
来源：http://hz.andypj.xyz/gttzrsejik.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtbeizcepm.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtqwhmhkpf.html

Py:   x in arr
来源：http://hz.c1oappe.top/gtpkfxveuv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtfqnvgpka.html

JS:   arr.includes(x)
来源：http://hz.cheryme.top/gtjfxvxxab.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtxghyxjcv.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtqcvvozxx.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangdashe.top/gtqdqpqeek.html

Ruby: arr.include?(x)
来源：http://hz.cheryme.top/gtkimzzppb.html

C#:   list.Contains(x)
来源：http://hz.chenjidiqi.icu/gteapchbqc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhengqikj.top/gtsteunvjz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtbumdsvwg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtujgysfkd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ivvv.top/gteezgcpui.html

TS:   [...arr];
来源：http://hz.cdnleiting.top/gtvpslgayc.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtcrfdxiti.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ehwqpu.com/gtekywspnv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangkeji.top/gtyplcsafb.html

C#:   new List<int>(list);
来源：http://hz.zhaomingkeji.xyz/gtxvvbahgz.html


<!-- 参考信息 -->