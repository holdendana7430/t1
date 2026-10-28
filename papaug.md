代发 wailian999

Py:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtadziekkx.html

PHP:  return [$a, $b];
来源：http://hz.tanke756.top/gtffwllioq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gzhubu.top/gtwovdcokx.html

TS:   return { a, b };
来源：http://hz.fzhhl.top/gtskhabnss.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.52xcode.cn/gtgcdwecab.html

Go:   return a, b
来源：http://hz.daxiang520.top/gtwawlhrqi.html

Ruby: return a, b
来源：http://hz.yuanzhike.top/gtwxjulxfu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydzc1.top/gtpqoeyput.html

[C06] 匿名函数 / lambda
来源：http://hz.birdmap.top/gtkywsxjzd.html

Py:   square = lambda x: x * x
来源：http://hz.zhixingplan.top/gtjhvfiemu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shangyingyoupin.top/gtxdbixrpl.html

JS:   const square = x => x * x;
来源：http://hz.gzhubu.top/gtkcfggecd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ppjwa.cn/gtgkloemwd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangtech.top/gticcvpwny.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hammf.cn/gtxiiavidx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.feifeiyinyue.top/gtoegzuyxp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gtdwzdxwbm.html

[C07] 把函数作为参数传入
来源：http://hz.yuxming.cn/gtlepmqgmj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.smart0.xyz/gtxhccwgoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuxming.cn/gtdpjnccam.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtphlwrvnw.html

TS:   arr.map(String)
来源：http://hz.cashguo.top/gtvvmtpxcu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gttvxolvjg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daria6918.cn/gtrsltmlfj.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnxiangtu.top/gtjgdgvkss.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtgegdcecn.html

[C08] 闭包
来源：http://hz.yonumen.top/gtmrbfsrvx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gzhubu.top/gtudrnbykd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gtzfvwvvxg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtzksfqoqd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtvyuxtclf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tanke756.top/gtoqsqtxtc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258.top/gtnghsuhdc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenjidiqi.icu/gtvmxoybwn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtudivcwxg.html

[C09] 递归
来源：http://hz.yj202588.top/gtojqelhif.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtgnpvsvsc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ppjwa.cn/gtofmgpzhf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtoanupeaz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtidjktdxl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gthnvsrhxe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jiagoushi.top/gtxxdtikxu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ybcxt.top/gtbhwtgryt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuanzx.com/gtkxbslkps.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gtuphcfrge.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.smart0.xyz/gtjrcaaonk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuxming.cn/gtcsrkoorp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtzcewtgtl.html

TS:   同 JS
来源：http://hz.shanyushiyangtech.top/gtxciuvfxb.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtnfrtulow.html

Go:   花括号块级作用域
来源：http://hz.wangdashe.top/gtkdqjilqo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxuanxn.top/gtgzkxbrci.html

C#:   块级作用域
来源：http://hz.zhengqikj.top/gtjdqbiblr.html

[C11] 模块导入与导出
来源：http://hz.0kj1m.cn/gtkczmkmim.html

Py:   from module import func
来源：http://hz.tian-w.cn/gtynjyibpn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.birdmap.top/gtuefrbytb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhongyouzk.top/gtdsxjedem.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtrmxpxqiu.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtclgcxini.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtdeofxska.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtegkmqrsv.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtrmdzrkxs.html

[C12] 立即执行函数 IIFE
来源：http://hz.gotoacloud.top/gtadgqfsdo.html

Py:   (lambda: print("run"))()
来源：http://hz.gogol.net.cn/gtlhkirfiy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangshuangyany.cn/gttfmlhfld.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gttvhcddbl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtfvtiwiue.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtvqqsapsb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtzuqixdfp.html

Ruby: -> { puts "run" }.call
来源：http://hz.316326.xyz/gtkrzayhmf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tian-w.cn/gtklcxppzv.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gtmqvwzkwn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtgadrkzby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtcqegbyyk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.c1oappe.top/gtwkdyyqaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtyfusmezr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtycfwdtzf.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtxfbhjinn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cucudq.cn/gtbcvauksa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.redwolf501.top/gtuxlwobzs.html

[C14] 泛型函数
来源：http://hz.cashguo.top/gtymtuhrvp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jlsjyb.cn/gtxzuoqeed.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gttreepcmm.html

JS:   // 无泛型
来源：http://hz.gaohongyu789.top/gtvwljqhbc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gtcwwbyqtu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pycfn.com/gtrmuezsbg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xziqi.cn/gtrqjvzgnp.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtczfphkpm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtaluichvv.html

[C15] 解构 / 展开参数
来源：http://hz.hywenlv.cn/gtayueqckn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hysaishi.cn/gtnzvyrjes.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtztgtyfcs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gttoukgnfz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yongpay.top/gtdijqkoss.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtkhmwxejf.html

Go:   // 无解构
来源：http://hz.316326.xyz/gtjlgcqkga.html

Ruby: a, b = pair
来源：http://hz.sufxvd.cn/gtutvszful.html

C#:   var (a, b) = pair;
来源：http://hz.zhixingplan.top/gtrtutvchb.html

[C16] 函数 / 方法重载
来源：http://hz.zhaomingkeji.xyz/gtulcfvisk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtclusxtkl.html

PHP:  // 无重载
来源：http://hz.haohaochexian.top/gtjdtbwwnt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ybcxt.top/gtlxetllxb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yongpay.top/gtgpuwbqli.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtymcpahil.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtrgifgmea.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtqqtcflvj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtkphztieb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzskoihmx.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gtbokedvls.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmcdyfiop.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtpkzcpysk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shangyingyoupin.top/gtjwotdsdk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258888.top/gtowngedbe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gtyhoskypw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnqzz.top/gtgqrkfiwz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258888.top/gtdehdljxq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xziqi.cn/gtkbaninoz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xziqi.cn/gtptappbgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtisrshhus.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gtyvbnflsw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yvedp.cn/gtsryfuhoj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tianlin.xyz/gtktucwwqn.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtdduodalt.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtfkphpypy.html

Java: list.add(4);
来源：http://hz.ehwqpu.com/gtfwluzrah.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gtdztpqvgo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ivvv.top/gtbbvhvteo.html

C#:   list.Add(4);
来源：http://hz.xuanzx.com/gtrtchcpdj.html

[D03] 在指定位置插入元素
来源：http://hz.jinyuanbaomall.cn/gtxvrxerdc.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gtgdjogwby.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gtgsmdqsqs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtonuaqrdu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtcwvmcnsm.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtebglknfa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dashuyun.cn/gtlwajuenh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gthjnrgeag.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gtmrwlpewx.html

[D04] 删除元素
来源：http://hz.shanyushiyangkeji.top/gtyivxdgry.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtstjatgzu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gtaqruepjz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtvwrvpowa.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtnevfwmcy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yonumen.top/gtdtjcnzcr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtyqzpmtwr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtedykrhqy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtpqsigktn.html

[D05] 访问与修改元素
来源：http://hz.xinyue.icu/gtzsjsmuqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtbyqbcmun.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtmpubrntq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.wangdashe.top/gtotwpjrfh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zdqjudy.top/gtjxazkuuf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtkhrskcjk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtsfkisnra.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fengsongda.top/gtwhiqmogu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtdamwfise.html

[D06] 数组长度
来源：http://hz.shuidangran.top/gtxdtahzcc.html

Py:   len(arr)
来源：http://hz.redwolf501.top/gtlggdoaay.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gtzldprneh.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtnweaywzp.html

TS:   arr.length
来源：http://hz.smart0.xyz/gtppflikij.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtcwgrrkng.html

Go:   len(arr)
来源：http://hz.9152youxi.cn/gtbllfqeki.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtorlozfbx.html

C#:   list.Count;
来源：http://hz.yuanzhike.top/gtdecaxjjs.html

[D07] 切片 / 取子数组
来源：http://hz.9152youxi.cn/gtnbgvnmih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtocbwaugv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gttvtzbaeb.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtftmxtrtj.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtvfxkajlt.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtfkwvcblt.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtdmzyqzin.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtzegfeqeh.html

C#:   list.GetRange(1, 3);
来源：http://hz.xziqi.cn/gtkeifinhn.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gtwrjzfvbz.html

Py:   a + b;  a.extend(b)
来源：http://hz.shuidangran.top/gtxqswpmkd.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtysdabofm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtdvsbxpih.html

TS:   [...a, ...b];
来源：http://hz.hammf.cn/gtijgwgpbp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.wangdashe.top/gtuzptbshm.html

Go:   append(a, b...)
来源：http://hz.chenjidiqi.icu/gtttrburqi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yangfankeji.com/gtqmzsttgg.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtzmhnzrtk.html

[D09] 排序（升序）
来源：http://hz.zhijiandao.cn/gtknyerldx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtmiwauaxe.html

PHP:  sort($arr);
来源：http://hz.zhiwuduotai.top/gtdkifpxxe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtfaosuwls.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.birdmap.top/gtttohswnh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pycfn.com/gtcxpsyvas.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtlenuofrn.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtjbgfgcgm.html

C#:   list.Sort();
来源：http://hz.nwbrower.top/gtipephfeq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sweek.top/gttfnnbchd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xylfe.cn/gtuddswpud.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtynkvccya.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtrcyftjfi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtisqhgazy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigfzy.top/gtsbqoyhte.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.snrcjt.cn/gtteplwjia.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtlhqniqtk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.quarkkingdee.top/gttudiqtnr.html

[D11] 反转数组
来源：http://hz.yj20258.top/gtcuqmxzuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yuxming.cn/gthmwfdauo.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtvphpgvwk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtexbgcwfx.html

TS:   [...arr].reverse();
来源：http://hz.jiagoushi.top/gtsiambbbu.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtxizjzafq.html

Go:   slices.Reverse(arr)
来源：http://hz.zhengqikj.top/gtkencvmmb.html

Ruby: arr.reverse
来源：http://hz.jlsjyb.cn/gtywikatyd.html

C#:   list.Reverse();
来源：http://hz.hammf.cn/gtphozrqrp.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtxscfkjey.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gtcznamqpj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxinkj.top/gtezfeikhh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtdauqxvrd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtqeccamdt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangkeji.top/gtysipjybs.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtrqvjwkyu.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtsnwwfyyv.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gthtmhnijg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhiwuduotai.top/gtjdnqgfpy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.havefunace.top/gtofhhlvoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtxorjtlkr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtrkrbyfcv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtbftvocxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nwbrower.top/gtwutvmdbg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aizwys.cn/gtjdrfmyhw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtdlsalcpf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258.top/gtvjpwnsps.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhiwuduotai.top/gtmpzkbfzi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yvedp.cn/gtwdcrraza.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtmpvqzdto.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtrbbhhegs.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtuoojdopy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtzoczotet.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtqofrrzqi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.bjfxy.top/gtfcmoujqa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gttqvobzli.html

[D15] 去重
来源：http://hz.meibo888.top/gtadckdhlq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtjimnesjt.html

PHP:  array_unique($arr);
来源：http://hz.zhixingplan.top/gtbvhuklcc.html

JS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtwskectct.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtceqfzyvb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.316326.xyz/gtirgwjwfr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hysaishi.cn/gtbnkijdkn.html

Ruby: arr.uniq
来源：http://hz.jlsjyb.cn/gtkedbomzs.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtzsvidpby.html

[D16] 求和与平均值
来源：http://hz.xylfe.cn/gtfxswmnqy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydjk.org.cn/gttqlfgzcc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtbjclpttm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtagqetedf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtaztvkkkp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtdxsjjdzk.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtrklckudb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.svipenyu.cn/gtkcrkciap.html

C#:   list.Sum();  list.Average()
来源：http://hz.zdqjudy.top/gtodihhcpo.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtuuygczet.html

Py:   max(arr);  min(arr)
来源：http://hz.gogol.net.cn/gtwtsuuuxn.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtauxtdirc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cqqwz.cn/gtpajwzpxg.html

TS:   Math.max(...arr);
来源：http://hz.xziqi.cn/gtpjivcofy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtbtqdbmyo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtwnuuukkd.html

Ruby: arr.max;  arr.min
来源：http://hz.zhiwuduotai.top/gtygwniivo.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtmglioeqc.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtwurkbubl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtgogkbfuk.html

PHP:  array_merge(...$nested);
来源：http://hz.gzhubu.top/gttaarbdzj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtjocqklgo.html

TS:   nested.flat();
来源：http://hz.yueranfly.top/gtswnaivzy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xingfuxueyuan.xyz/gthscwlprj.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtgugqeddt.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtufzbexwt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtzucdhoqr.html

[D19] 按字段分组
来源：http://hz.hywenlv.cn/gtgdjfsftz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtnhbyxisy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinghuilouyu.cn/gtstjpyynq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuanzx.com/gtavbqyjus.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cucudq.cn/gtyrapkopy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgufenzy.top/gtmbzlcqwh.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxinkj.top/gtymwpajym.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhaomingkeji.xyz/gtubfqtwus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cucudq.cn/gtzkfzcfto.html

[D20] 统计每个元素出现次数
来源：http://hz.shzxlz.cn/gtqtjtjycn.html

Py:   Counter(arr)
来源：http://hz.nwbrower.top/gtilzhydad.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtqdjfwooz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtazwvtdzf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtzmvwikrq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtvddwqgqh.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gtxfmroooh.html

Ruby: arr.tally
来源：http://hz.vqdsnc.cn/gtrkegzrcj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtnqnomely.html

[D21] 判断是否包含某元素
来源：http://hz.haohaochexian.top/gtudlijjsu.html

Py:   x in arr
来源：http://hz.zhongyouzk.top/gtoiuyytms.html

PHP:  in_array($x, $arr, true);
来源：http://hz.bjfxy.top/gtgamnogqz.html

JS:   arr.includes(x)
来源：http://hz.yj20258.top/gtqxryeowy.html

TS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtlhtkfkop.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gtbuvdxurb.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigfzy.top/gtyyptioqi.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtvczyntgs.html

C#:   list.Contains(x)
来源：http://hz.tianlin.xyz/gtrpkfalrs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gtqdoovelt.html


<!-- 参考信息 -->