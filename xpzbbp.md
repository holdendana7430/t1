代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtizxikbvb.html

Go:   return a, b
来源：http://hz.shangyingyoupin.top/gtehluzfty.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtwadxujql.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gthgwcexqs.html

[C06] 匿名函数 / lambda
来源：http://hz.sysykeji.top/gthdlxhchw.html

Py:   square = lambda x: x * x
来源：http://hz.bjfxy.top/gtphaqavxe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhijiandao.cn/gtiqvwedld.html

JS:   const square = x => x * x;
来源：http://hz.hongshengwenyu.top/gtdqwwemwk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinyuanbaomall.cn/gtuftntqpk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aizwys.cn/gtnaaxaqdu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yangfankeji.com/gtrmzeklwy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnxiangtu.top/gtfxdnedin.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigufen.top/gtaavgtegu.html

[C07] 把函数作为参数传入
来源：http://hz.andypj.xyz/gtcikspsje.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yonumen.top/gtrzuuewym.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtooiucmqm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.pengpengdd.cyou/gtjnbxjixx.html

TS:   arr.map(String)
来源：http://hz.xylfe.cn/gtehcxjnsd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.bjfxy.top/gtkvdusurj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gthaydwrdf.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtcujntkzn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xuetiantiany.cn/gtpbbezbtt.html

[C08] 闭包
来源：http://hz.tanke756.top/gtnphjnoqb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydjk.org.cn/gtflkwvxjp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cashguo.top/gtzpzcvvvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtncjcnwks.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtpkwnmhim.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.bjfxy.top/gtzyetmofe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtwqyjoqrx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sufxvd.cn/gtswrgszrp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtfnlcxehy.html

[C09] 递归
来源：http://hz.yuxming.cn/gtbmirhzgw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj202588.top/gthuoyrxrp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tanke756.top/gtxicgfijw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gteaczfaug.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtwmdpaipy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yanxiufei.cn/gtbjbhjyps.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shanyushiyangtech.top/gtkklwjtiy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gtoztcsooh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yuanzhike.top/gtvjaghnny.html

[C10] 变量作用域
来源：http://hz.gzhubu.top/gtdufghrtg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.redwolf501.top/gtmmgaxyvn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ywan-chungtsiang.top/gtubklctei.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gteqdwqppd.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtvpvwlqmy.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtzujstowl.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtwraeebpi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cashguo.top/gtbjghezee.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gtbqxgxjzl.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtjwavorsu.html

Py:   from module import func
来源：http://hz.jqgfzy.top/gtgboithzb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtugvwneeo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.quarkkingdee.top/gtbvpttvha.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.quarkkingdee.top/gtxrmfxrge.html

Java: import java.util.List;
来源：http://hz.vqdsnc.cn/gtcwwqbpdg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtgrqzowpd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtiscgptwi.html

C#:   using System.Text;
来源：http://hz.zhengqikj.top/gtypwkgslu.html

[C12] 立即执行函数 IIFE
来源：http://hz.bjfxy.top/gtaiavfxpm.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gtqckxkgjd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gtxiltelzw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtmncfmhra.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtlfdbtodc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhijiandao.cn/gtmvjcesxh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gzhubu.top/gtdlivvwim.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtktjqzqae.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.meibo888.top/gtywmyzjyn.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gthnbarxtz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tian-w.cn/gtvwqvmtuf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtkdignbzo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtalmpyqdn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtntjxdngn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtfykuevur.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtkhndsyso.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.birdmap.top/gthmcsvmda.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sufxvd.cn/gtzqeuitoi.html

[C14] 泛型函数
来源：http://hz.yj20258.top/gtivwtkxfd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenzaomai.com/gtxrsbhywk.html

PHP:  // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtwfdcfqqt.html

JS:   // 无泛型
来源：http://hz.yueranfly.top/gtvsqikxxu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtpwfbcfsu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jianghu66.top/gtmnrjwttk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtdkzebcnp.html

Ruby: # 无泛型
来源：http://hz.quarkkingdee.top/gticdwsmvc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuetiantiany.cn/gtwlahksek.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtiztczmrb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtqubkxldy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtqjoutera.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhiwuduotai.top/gtbgmoxuky.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangkeji.top/gtwppednuk.html

Java: // 无解构
来源：http://hz.snrcjt.cn/gtyhuuwsdo.html

Go:   // 无解构
来源：http://hz.cqqwz.cn/gtxrouzmbw.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gttfskwjrh.html

C#:   var (a, b) = pair;
来源：http://hz.fzhhl.top/gtzguwpllr.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtrktjoqiu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtaizvsmss.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtdvakrvbm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtlgwywout.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnqzz.top/gtdxkziylc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtffnvshmi.html

Go:   // 无重载：用不同函数名
来源：http://hz.ehwqpu.com/gtjefimldi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.c1oappe.top/gtefvdoxrv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.quarkkingdee.top/gtetitxxlo.html

================================================================================
来源：http://hz.mhx1999.top/gtnvicqdwn.html

D. 数组 / 列表 / 集合
来源：http://hz.snrcjt.cn/gtzlkmaspv.html

================================================================================
来源：http://hz.shzxlz.cn/gthdcxmvrw.html

[D01] 创建数组 / 列表
来源：http://hz.guannengcc.top/gtiyqruuxa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yonumen.top/gtmgzoxwtz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.0kj1m.cn/gttkgsvxwo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gthvmusgko.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cashguo.top/gtcaevbngl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtnskvquzg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xylfe.cn/gtmiyqizgj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtabwaxfgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtfncudbyx.html

[D02] 追加元素到末尾
来源：http://hz.ppjwa.cn/gtlyrojcog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gteifainqp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gtundeymzt.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtdqrhkuqu.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtypogstne.html

Java: list.add(4);
来源：http://hz.guannengcc.top/gtpqdzhcto.html

Go:   arr = append(arr, 4)
来源：http://hz.yonumen.top/gtqdikwdee.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hammf.cn/gtxoihgmav.html

C#:   list.Add(4);
来源：http://hz.zhijiandao.cn/gtsbafmsvb.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtwaennkkx.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtsskwpghf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtvuseldpb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gtyhqywiol.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtnocdntsi.html

Java: list.add(0, 0);
来源：http://hz.jinqigufen.top/gtjcamzsvr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.9152youxi.cn/gtmeyezrii.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtsfcupnqp.html

C#:   list.Insert(0, 0);
来源：http://hz.yvedp.cn/gtjroagpoz.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gtmtzmpqmm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtonjfzepy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hongshengwenyu.top/gtvwxgnmeq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jqgfzy.top/gtfrpfcaxb.html

TS:   arr.splice(0, 1);
来源：http://hz.jinyuanbaomall.cn/gtrqoqnmjm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pycfn.com/gtyfdycdkg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ivvv.top/gtxyeyoldg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hysaishi.cn/gtfvkyatii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.bjfxy.top/gtnwilrinc.html

[D05] 访问与修改元素
来源：http://hz.dianchejie.cn/gtjltepxlx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtuhzbbnea.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tian-w.cn/gtcqulnbti.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtcbkeccwo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258888.top/gtejkvywwh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cqqwz.cn/gtofegiwim.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtkpqpobue.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtygrtrdei.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dianchejie.cn/gtoydeammd.html

[D06] 数组长度
来源：http://hz.zdqjudy.top/gtnjqwrcqf.html

Py:   len(arr)
来源：http://hz.havefunace.top/gtghkvsnjt.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtgbfvyyks.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtwcencktq.html

TS:   arr.length
来源：http://hz.daxiang520.top/gtkuvkdkaw.html

Java: list.size();
来源：http://hz.mhx1999.top/gtawtlbmfu.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtddcabaeq.html

Ruby: arr.length; arr.size
来源：http://hz.redwolf501.top/gtmmqluzfc.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gtkbutfzje.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtuwjlxfkx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtmdopomet.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtobxgeyof.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtwurhfbwu.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtkysishje.html

Java: list.subList(1, 4);
来源：http://hz.chenlongwang.top/gtygaejydx.html

Go:   arr[1:4]
来源：http://hz.ydzc1.top/gtaqxmsuaz.html

Ruby: arr[1, 3]
来源：http://hz.jlsjyb.cn/gtygibgjpl.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxuanxn.top/gtwueravbz.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtqgxtctfe.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gtlnproumc.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtzoxytzvb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jianghu66.top/gtlgrsukpk.html

TS:   [...a, ...b];
来源：http://hz.dianchejie.cn/gtndwsxdak.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gthtuofmsj.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtzrktuway.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtjjtykblx.html

C#:   a.Concat(b).ToList()
来源：http://hz.redwolf501.top/gtxrfzfrnr.html

[D09] 排序（升序）
来源：http://hz.daxiang520.top/gtbvauigwu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gtpqwtsfvc.html

PHP:  sort($arr);
来源：http://hz.haohaochexian.top/gtorzarqro.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nwbrower.top/gtnzeyjoqs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.quarkkingdee.top/gtvxqrovea.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gtdyspfhwl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.birdmap.top/gtufyxbmza.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtnwwbnmbu.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gthxuvosmq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtfwpfneid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtsbqwkkyg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtpvkfpnqv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gttsscotkw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtdvhyyyis.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yueranfly.top/gtnojpgnie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258888.top/gtfbcsgsuu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hammf.cn/gtmjvhcmkg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gotoacloud.top/gtfukzzefd.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtfuexqgdp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aibaodan.cn/gtlyjtablx.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtachkwrws.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jiagoushi.top/gttybdebnu.html

TS:   [...arr].reverse();
来源：http://hz.zhengqikj.top/gtglmntpax.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtpmtondxm.html

Go:   slices.Reverse(arr)
来源：http://hz.meibo888.top/gtvgltteim.html

Ruby: arr.reverse
来源：http://hz.hysaishi.cn/gtbhpelpbo.html

C#:   list.Reverse();
来源：http://hz.kuanghao11.cn/gtvdclhger.html

[D12] 查找元素下标
来源：http://hz.cucudq.cn/gtvgamfxvt.html

Py:   arr.index(x);  x in arr
来源：http://hz.nwbrower.top/gthnisjuwo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ehwqpu.com/gtgdiealpz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtawnkmqmq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtefwyhcap.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtrweoopcv.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgufenzy.top/gtmnhceios.html

Ruby: arr.index(x)
来源：http://hz.ydjk.org.cn/gtnzbvxxbf.html

C#:   list.IndexOf(x);
来源：http://hz.jlsjyb.cn/gthntxzhde.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtkgjibbxw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtpgspjanq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daxiang520.top/gtcuuvxnag.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gthrocyitg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtxrotnslz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cashguo.top/gtfhqtivgg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxuanxn.top/gttpmiojtq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gtaogwhabq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gtwdzlodfd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gogol.net.cn/gtmsitjuhw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cucudq.cn/gtcdegzmxz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hongshengwenyu.top/gtqmseefhy.html

JS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtfjsrrbjt.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtfaosfclh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtmrhzxsev.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtrczknuaj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtiwrrxxoy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtnaoqgqwn.html

[D15] 去重
来源：http://hz.haohaochexian.top/gthyigznkm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtbilkwvbf.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtkzfuqcor.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gttifnbxro.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtsthnpmzr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigfzy.top/gtmqqheyda.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.vqdsnc.cn/gtgiuggmjo.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtdyqhftfd.html

C#:   list.Distinct().ToList()
来源：http://hz.bjfxy.top/gtgsiyygai.html

[D16] 求和与平均值
来源：http://hz.snrcjt.cn/gtlcgtupjn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.feifeiyinyue.top/gthoilethw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtwegsnfyf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtobfnxmmc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtuxfnbqdf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.redwolf501.top/gtzckuxnaa.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gttmftfpaj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtmltbkjgj.html

C#:   list.Sum();  list.Average()
来源：http://hz.yangfankeji.com/gtckjwbtqs.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtcoegfrqk.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gtukotiqko.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigfzy.top/gtxtrnogyl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fzhhl.top/gtljtpmdpt.html

TS:   Math.max(...arr);
来源：http://hz.zhengqikj.top/gtmfjsmtqb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jyoumei.cn/gtdkookuzp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gttymjavor.html

Ruby: arr.max;  arr.min
来源：http://hz.hysaishi.cn/gtgdiqqivb.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtdgownbom.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtaqqopjmn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gttqpknilu.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtxdixcmlq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtbnciawvo.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtkgneqlve.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jianghu66.top/gtqecsousf.html

Go:   // 手写双层循环
来源：http://hz.fzhhl.top/gtmydeovjc.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtpbqklhvl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtbqwodgkc.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gtfehdxtrh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgfzy.top/gtzhmhieac.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gtgsfqowlc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jiagoushi.top/gtfiggfqyg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtovegskrz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gtbpvzyknw.html

Go:   // 手写 map[string][]T
来源：http://hz.zycfv.cn/gtvhmydlnx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhoulong.xyz/gtpmerghyv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtomhtxeiz.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtcclpwdjo.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtcixenuzl.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtpombukgk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gthplpixrh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtwhosqccz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtvcvrkupu.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtazgumeqn.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtvoieevku.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.redwolf501.top/gtqoultfgh.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtepshnnan.html

Py:   x in arr
来源：http://hz.zhijiandao.cn/gtcqcpjuft.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtknfjdten.html

JS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtntlpfdnd.html

TS:   arr.includes(x)
来源：http://hz.hammf.cn/gthqzocale.html

Java: list.contains(x)
来源：http://hz.chenjidiqi.icu/gthvofrsxp.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtxugentgc.html

Ruby: arr.include?(x)
来源：http://hz.gogol.net.cn/gtkncfglmh.html

C#:   list.Contains(x)
来源：http://hz.zhoulong.xyz/gtpygskazw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tianlin.xyz/gtqseykrzp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhengqikj.top/gtzdjsjlnv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.quarkkingdee.top/gtwyrziecv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sweek.top/gtialfyzpy.html

TS:   [...arr];
来源：http://hz.ehwqpu.com/gtwkiebvjs.html


<!-- 参考信息 -->