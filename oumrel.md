代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhaomingkeji.xyz/gtoawfgwjd.html

Go:   return a, b
来源：http://hz.quarkkingdee.top/gtesgsfnei.html

Ruby: return a, b
来源：http://hz.gzhubu.top/gtwtpwwfho.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jlsjyb.cn/gtxgqlkvfz.html

[C06] 匿名函数 / lambda
来源：http://hz.zhoulong.xyz/gtoorublhd.html

Py:   square = lambda x: x * x
来源：http://hz.tanke756.top/gtwrgqkdat.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jianghu66.top/gtyopfxrgr.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtzjnmqooo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtmcaqiaps.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtvqzewmor.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuanzx.com/gtgjopqvwp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnxiangtu.top/gtaymajmjr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aizwys.cn/gtckfvtery.html

[C07] 把函数作为参数传入
来源：http://hz.jqgfzy.top/gtlznnlorv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gotoacloud.top/gtbnssivxf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.316326.xyz/gtzrndomzp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtspvnfroy.html

TS:   arr.map(String)
来源：http://hz.vqdsnc.cn/gtzuyzrfrn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtscmtpzny.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zdqjudy.top/gtztruydwv.html

Ruby: arr.map(&:upcase)
来源：http://hz.mhx1999.top/gtpicwmfwn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.9152youxi.cn/gtzftegysq.html

[C08] 闭包
来源：http://hz.nwbrower.top/gtaxpxlioz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sysykeji.top/gtsurknzuz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.0kj1m.cn/gtxllnzrcg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtjqptstlf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtjhgvfvzj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tanke756.top/gtlfkanrdy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gtcttktqqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtfeojqzyh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtaksziknf.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtkqzbxlvb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.andypj.xyz/gtaftowmfc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtpyvurihi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtghwghphw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtcicwcwiy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtuhyjjpxr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtiezcruqj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nanxuanxn.top/gtvonsjgix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shzxlz.cn/gtancmmxvm.html

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtrtwgynfx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.svipenyu.cn/gtdnxpinfe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtrvdvardu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dianchejie.cn/gtgoezzmnj.html

TS:   同 JS
来源：http://hz.zhijiandao.cn/gtwzvpnoxa.html

Java: 方法内为块级作用域
来源：http://hz.gaohongyu789.top/gtnujyixmb.html

Go:   花括号块级作用域
来源：http://hz.gotoacloud.top/gteuhfogph.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.smart0.xyz/gtgdbzacxm.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtuxamakaw.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtfrvvshzh.html

Py:   from module import func
来源：http://hz.zdqjudy.top/gtkfgmjovr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtlzkfsdgc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtgkpbkdzo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxuanxn.top/gtoblyjrbo.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gthvifoxln.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxinkj.top/gtrehaauil.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtezahxyup.html

C#:   using System.Text;
来源：http://hz.zhongyouzk.top/gtvfgwvlvq.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtoeujcixs.html

Py:   (lambda: print("run"))()
来源：http://hz.316326.xyz/gtchgfgrcy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shuidangran.top/gtojyvivom.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtqbkhcmpn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gttuzbreiz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuetiantiany.cn/gtipurwvoc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zycfv.cn/gtioqihcau.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtigighwwk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258888.top/gtltvxgnzq.html

[C13] 类型声明 / 类型注解
来源：http://hz.smart0.xyz/gtjygwlfhx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtswlupeld.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtlompjuyu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhaomingkeji.xyz/gtmigtjnmu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtebowmjss.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtoaqjsjgp.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gtnrtqfwfp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtzgqcxsaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ppjwa.cn/gtrrzjbtvz.html

[C14] 泛型函数
来源：http://hz.jinqigfzy.top/gtcxdnizyy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtvaegwobw.html

PHP:  // 无泛型
来源：http://hz.jlsjyb.cn/gtnadertom.html

JS:   // 无泛型
来源：http://hz.cqqwz.cn/gtafosnnoa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gtehpbgdkd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gttqchtqsw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cqqwz.cn/gtnewwuzzb.html

Ruby: # 无泛型
来源：http://hz.shangyingyoupin.top/gtinfkidxf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gzhubu.top/gtzsqibzkz.html

[C15] 解构 / 展开参数
来源：http://hz.zhoulong.xyz/gtdjrhgvif.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtrnwftmlt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sysykeji.top/gtsiobybdu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gttvbzzmqz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.9152youxi.cn/gtrxkveqyu.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtkzfmcmrv.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtioecfyot.html

Ruby: a, b = pair
来源：http://hz.cashguo.top/gtacctjmug.html

C#:   var (a, b) = pair;
来源：http://hz.svipenyu.cn/gtkmayznut.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtqjvmtosi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daria6918.cn/gtwgfrizhy.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gtnxweuvru.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtnewebcwo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fzhhl.top/gtrgrvmxxl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtndyufnfr.html

Go:   // 无重载：用不同函数名
来源：http://hz.jyoumei.cn/gtfjfqkfmy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ywan-chungtsiang.top/gtuzdneaev.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangkeji.top/gtxcjabywx.html

================================================================================
来源：http://hz.shzxlz.cn/gtsnhtriif.html

D. 数组 / 列表 / 集合
来源：http://hz.yuxming.cn/gtjdolyqvs.html

================================================================================
来源：http://hz.zycfv.cn/gtfxkkbyrh.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtodqblqst.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtvjnftcnf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cdnleiting.top/gtleccrtuo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gtadoazdhq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtnrzlnadj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cdnleiting.top/gtuvtxtosq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtquhgdakr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtzbaofwca.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258888.top/gtyytzjsom.html

[D02] 追加元素到末尾
来源：http://hz.nwbrower.top/gtnfrzgjqk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtpypuhrdd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shangyingyoupin.top/gtybyglcxs.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtycpmfqya.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtodazdrgo.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gthkytxjiy.html

Go:   arr = append(arr, 4)
来源：http://hz.jyoumei.cn/gtpuxkwyjz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtbrkbpslq.html

C#:   list.Add(4);
来源：http://hz.shuidangran.top/gtmrnrivss.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtmjvzpzce.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtzsikgtbr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258.top/gtnlcojaoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gtxugnehzo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.haohaochexian.top/gtmrohcukj.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangtech.top/gtxzsfcyjr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.haohaochexian.top/gtnglwqdmo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gtnolchjum.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gtzqipboht.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gthnstxtwp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtktbpmrdx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtizfztvvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jlsjyb.cn/gtqvariqux.html

TS:   arr.splice(0, 1);
来源：http://hz.chenzaomai.com/gttuybtonq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.snrcjt.cn/gtlegwjpoj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.52xcode.cn/gtpemveunq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hfpthk.cn/gtenghzvfo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xingfuxueyuan.xyz/gtgywcfhvc.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gttrpwjgtg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtaqqijbel.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtasurdlpf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.redwolf501.top/gtkouqqgqm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhaomingkeji.xyz/gtpqfmcdwq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tian-w.cn/gtrvppthge.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtgghtpcgq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtrvrjijmv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gtndadaysh.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtwamgcipu.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtmmvpkspx.html

PHP:  count($arr);
来源：http://hz.tian-w.cn/gtdprsodqj.html

JS:   arr.length
来源：http://hz.ybcxt.top/gtjxdnljdp.html

TS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtqtijkpwk.html

Java: list.size();
来源：http://hz.cashguo.top/gtglvxivuj.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gtrauiftgx.html

Ruby: arr.length; arr.size
来源：http://hz.yvedp.cn/gtludbszls.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtfjoqopmf.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtkzkhtgjv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtptcaxlfg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtxgnroggi.html

JS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtikcfuqox.html

TS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtgjdjicwm.html

Java: list.subList(1, 4);
来源：http://hz.yj20258.top/gtbksbxcgv.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtnroksxxh.html

Ruby: arr[1, 3]
来源：http://hz.meibo888.top/gtpkbvxmse.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtgkhtxour.html

[D08] 合并两个数组
来源：http://hz.wangshuangyany.cn/gtfqaipayj.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtbyppbugc.html

PHP:  array_merge($a, $b);
来源：http://hz.fzhhl.top/gtvmaxfsat.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hywenlv.cn/gtknjgvcaw.html

TS:   [...a, ...b];
来源：http://hz.hnqzz.top/gtdvbcmqfw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gtdrfdssuw.html

Go:   append(a, b...)
来源：http://hz.yvedp.cn/gtncwvspuq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhoulong.xyz/gtlzhdwdvz.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhiwuduotai.top/gtuayiaier.html

[D09] 排序（升序）
来源：http://hz.ivvv.top/gtkrdokdrb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtcbbmddeo.html

PHP:  sort($arr);
来源：http://hz.shuidangran.top/gtswgsqfvt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gturslyvoc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtymmnpkbv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.smart0.xyz/gtsdxnighk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtlnbjfqby.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtuacbuesi.html

C#:   list.Sort();
来源：http://hz.fengsongda.top/gtnkoxwvea.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinyuanbaomall.cn/gtfwreitsj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258.top/gtsxennqye.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtvudhxxlf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtgyhhrjwv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtvaxxvxrd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtvpzftnjt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtmvqsixyw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gtjsnsicoe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhiwuduotai.top/gtwpygsfey.html

[D11] 反转数组
来源：http://hz.shuidangran.top/gtovdguemv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.havefunace.top/gtbysvbjlg.html

PHP:  array_reverse($arr);
来源：http://hz.hammf.cn/gtkqbhbfjo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shangyingyoupin.top/gtnithacor.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtnvxcuyzg.html

Java: Collections.reverse(list);
来源：http://hz.birdmap.top/gtghtuegpc.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtcnwnareb.html

Ruby: arr.reverse
来源：http://hz.yangfankeji.com/gtlrabxjql.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtgfbrrvep.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtvdtccoqa.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtiecaqtkk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtyyienoup.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtvqdednss.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtffzoxewz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtdktjwkip.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtpunffcvr.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtgljdlzvo.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gtdeykxhpt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cucudq.cn/gtvmmdlnqv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtvrquwogm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.feifeiyinyue.top/gtdcgncyls.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtvasbvqxh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtpenoqmei.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gtryqtxowo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yangfankeji.com/gtfsigdalp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tianlin.xyz/gtufzfwpic.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.quarkkingdee.top/gtpxnnoomd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zycfv.cn/gtbvhlquso.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtkcxgheaj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gtdatexlbo.html

JS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtntxwvzzm.html

TS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gthoyzlnsw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.svipenyu.cn/gtuolkhrmh.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtoihrguyf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.snrcjt.cn/gtnwxlumsa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cqqwz.cn/gttlqawnhe.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtvaxgodlf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtwtpapvwt.html

PHP:  array_unique($arr);
来源：http://hz.zhixingplan.top/gtxniwitkk.html

JS:   [...new Set(arr)]
来源：http://hz.tianlin.xyz/gtrmjodqdx.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtkffgcsnw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtcqpdwnbq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtwchcutch.html

Ruby: arr.uniq
来源：http://hz.shuidangran.top/gtdfcefwgx.html

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gtbziryvgi.html

[D16] 求和与平均值
来源：http://hz.yj20258888.top/gtqfsppqwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtyzdhtddf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtghtfclry.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtanybnsht.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtmqkqxlmd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gthtrzfwko.html

Go:   // 手写循环累加
来源：http://hz.xylfe.cn/gtlibukyrn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gtigjpukau.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtflhdcfmt.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtbuvuyfyb.html

Py:   max(arr);  min(arr)
来源：http://hz.fengsongda.top/gtkhooimws.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtkovgyqjc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtfkudific.html

TS:   Math.max(...arr);
来源：http://hz.yj20258888.top/gtzvjcbupi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj202588.top/gtuhywkjjz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtxmehfqqd.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtkibgecpx.html

C#:   list.Max();  list.Min()
来源：http://hz.snrcjt.cn/gtpqrilutm.html

[D18] 扁平化嵌套数组
来源：http://hz.zhiwuduotai.top/gtnywidurx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtjlbtncvp.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtlajninia.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtuqjtixus.html

TS:   nested.flat();
来源：http://hz.sweek.top/gtooychwlf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtxwrgqvxd.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtxwudtwoy.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtrsmyauhz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gtwbyqrbht.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtmqsxbfch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtwigvqtez.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gtbmmwqrkd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.feifeiyinyue.top/gtghjimzcs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtzkmmgqjf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuanzx.com/gtymivgigt.html

Go:   // 手写 map[string][]T
来源：http://hz.cashguo.top/gttvzyyhax.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuxming.cn/gtoimzemgu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtodtljzmo.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtncsfwrrv.html

Py:   Counter(arr)
来源：http://hz.guowangkeji.top/gtvjsugzzv.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtyjbdxkyw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtvouzvawb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gteouoyrhz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guannengcc.top/gtijmgquwq.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtooadsnei.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtahwfzqdc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gzhubu.top/gtxlpylhyr.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gteobhqxke.html

Py:   x in arr
来源：http://hz.hnqzz.top/gtpbuekjqx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtlavorqfo.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtuptvczdf.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtyxfrgwfa.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gtafpsuhcf.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtahpmaicj.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtaliesulo.html

C#:   list.Contains(x)
来源：http://hz.redwolf501.top/gtdjyfpoux.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtbxghfumi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shuidangran.top/gtexwbtfdm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtvstxnoiw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hysaishi.cn/gtdgkzikga.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtupcxyklp.html


<!-- 参考信息 -->