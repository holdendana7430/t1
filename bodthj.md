代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuxming.cn/gtshpvgurl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hammf.cn/gtxzmskvkr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtjajjcysp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dianchejie.cn/gthoqvzppf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.0kj1m.cn/gtzspnqcxw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ydjk.org.cn/gtyhgbcjyc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gtzzfbsuyf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtpuiofjku.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtpzgsbnlx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtauexazbz.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtipqkvwmx.html

[C05] 返回多个值
来源：http://hz.shanyushiyangkeji.top/gtvbddzxtd.html

Py:   return a, b
来源：http://hz.redwolf501.top/gtgqzhvivz.html

PHP:  return [$a, $b];
来源：http://hz.9152youxi.cn/gtljlzhmqn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pycfn.com/gtfmkpthrr.html

TS:   return { a, b };
来源：http://hz.yj202588.top/gtyeunufws.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuxming.cn/gtlfaaapwd.html

Go:   return a, b
来源：http://hz.cucudq.cn/gtkxdsnjpr.html

Ruby: return a, b
来源：http://hz.ehwqpu.com/gtlitnqnra.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhaomingkeji.xyz/gtrqzyigcu.html

[C06] 匿名函数 / lambda
来源：http://hz.birdmap.top/gtuomkoyhu.html

Py:   square = lambda x: x * x
来源：http://hz.gaohongyu789.top/gttpftrwkl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuanzhike.top/gtbxrkxjsn.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gttcemmhxe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.iojbl.cn/gtohxgwpag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aibaodan.cn/gthhzuggqn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sweek.top/gtiohfoybi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenlongwang.top/gtctasquev.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tianlin.xyz/gtktcqkged.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gttoznorcp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tanke756.top/gtferumelp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ywan-chungtsiang.top/gtskglvdyy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.mhx1999.top/gtymxbvbgv.html

TS:   arr.map(String)
来源：http://hz.nanxinkj.top/gtqlwsryrt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ywan-chungtsiang.top/gtqgltrasl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gtsewkozfe.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtiwubacmg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ppjwa.cn/gtuixqemjo.html

[C08] 闭包
来源：http://hz.daxiang520.top/gttmvicjnb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtkdupezjs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtwndnuaaf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtxmybmatt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtejkesdjz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gtoepfvkit.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gtgcwepgoi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cheryme.top/gtwwiyutxo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.vqdsnc.cn/gtrqnxcwfb.html

[C09] 递归
来源：http://hz.zdqjudy.top/gthnqmtbve.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtuxfgvmsj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.vqdsnc.cn/gtiusacihg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daria6918.cn/gtyvtmvbyu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtruugqtyo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jiagoushi.top/gtxvgbvdug.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gttdqtkgae.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtejazfedx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtvppklxwy.html

[C10] 变量作用域
来源：http://hz.cucudq.cn/gtpqqrbgsn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aibaodan.cn/gtuxpyhznq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pycfn.com/gtmtovbqas.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtvpeeehdq.html

TS:   同 JS
来源：http://hz.jyoumei.cn/gtbfilhkyc.html

Java: 方法内为块级作用域
来源：http://hz.aibaodan.cn/gtdkxwgoko.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtakddhmvd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tianlin.xyz/gteczmsxgt.html

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtzqabazol.html

[C11] 模块导入与导出
来源：http://hz.birdmap.top/gtyyihczxk.html

Py:   from module import func
来源：http://hz.sweek.top/gttmiolzrv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ywan-chungtsiang.top/gtywaiehwh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgufenzy.top/gtngfunlpk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yangfankeji.com/gtmaqquhja.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtnovjfodt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.meibo888.top/gtkdgpcsqu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hysaishi.cn/gtxfzkemfs.html

C#:   using System.Text;
来源：http://hz.snrcjt.cn/gtdrvgfhxp.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhoulong.xyz/gtqgxjnheu.html

Py:   (lambda: print("run"))()
来源：http://hz.gotoacloud.top/gtvulkowmw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtketraqfv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gtkdmubnub.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gtaqvhdlqi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tianlin.xyz/gtybgcopyp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtiaxrbdwl.html

Ruby: -> { puts "run" }.call
来源：http://hz.dianchejie.cn/gtluefunvz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtuxwavymt.html

[C13] 类型声明 / 类型注解
来源：http://hz.dashuyun.cn/gtsftbfxfs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.kuanghao11.cn/gtpsjykfto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gthsotwemk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtpkgufxsq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtdelzijlf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtllcvegrg.html

Go:   func add(a, b int) int
来源：http://hz.wangshuangyany.cn/gtlfnxhzer.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cucudq.cn/gtfvupcsum.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtogngmwlk.html

[C14] 泛型函数
来源：http://hz.xuanzx.com/gtrwwxhlai.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuanzhike.top/gtwwpjdkhi.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtxpfgxmxv.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtftaqwhco.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydjk.org.cn/gtzazrxycw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydjk.org.cn/gtmoqugfnt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gtyipbgoiy.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtcykgssly.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ybcxt.top/gtzjdrmkcw.html

[C15] 解构 / 展开参数
来源：http://hz.hnqzz.top/gtexojjdai.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aizwys.cn/gtfrekrphy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtyocakgav.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtubayesvj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gtyxiqvaec.html

Java: // 无解构
来源：http://hz.gogol.net.cn/gtgjkepxfg.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtwqskubhx.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtgrvdayxm.html

C#:   var (a, b) = pair;
来源：http://hz.jlsjyb.cn/gtorbeevml.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtlxndndtg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shzxlz.cn/gtzicnvfla.html

PHP:  // 无重载
来源：http://hz.jqgufenzy.top/gttlhnnfqs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gotoacloud.top/gtnplfyfqb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtdtyglszw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtespexybh.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhiwuduotai.top/gthsnzqnkd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.meibo888.top/gtvbhubvew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gtspdpinhz.html

================================================================================
来源：http://hz.dashuyun.cn/gtxljjykei.html

D. 数组 / 列表 / 集合
来源：http://hz.daria6918.cn/gtfxkoqmyr.html

================================================================================
来源：http://hz.xylfe.cn/gtwmlrihon.html

[D01] 创建数组 / 列表
来源：http://hz.guowangkeji.top/gtcmoyvvbf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtwrlzqvbg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtschsuwsn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtmkzjbcrm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtgbjhyblq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtxqtkxnap.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jlsjyb.cn/gtqgwmqqxw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xylfe.cn/gtkkkjwvwx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtbmfqmrpw.html

[D02] 追加元素到末尾
来源：http://hz.kuanghao11.cn/gtjecfkvjf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtcixfjfgh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gtoqbaasut.html

JS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtebolbfjv.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtveypaxfc.html

Java: list.add(4);
来源：http://hz.yonumen.top/gtspvrdkfl.html

Go:   arr = append(arr, 4)
来源：http://hz.feifeiyinyue.top/gtgfezzmnq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtdyufrcbr.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtafidjzhm.html

[D03] 在指定位置插入元素
来源：http://hz.havefunace.top/gttwnqemnw.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtwzhkuirl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zycfv.cn/gtzosodvbo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnqzz.top/gtfbfvnikl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cdnleiting.top/gtrpfqfgee.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gtxyufekam.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gthtaylvex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtoleadmor.html

C#:   list.Insert(0, 0);
来源：http://hz.zycfv.cn/gtkqfnrqoy.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtgrtnlkna.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shangyingyoupin.top/gtojzdouqc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinghuilouyu.cn/gtydwgsest.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gttvntfphc.html

TS:   arr.splice(0, 1);
来源：http://hz.tian-w.cn/gtcsjyomdm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258.top/gtelpazczl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtssrtzpaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258.top/gtdlcdtgov.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinyuanbaomall.cn/gtdjioemfa.html

[D05] 访问与修改元素
来源：http://hz.cdnleiting.top/gtbavrcbnl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtxiewibto.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtxybegjrj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtfgkxujos.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtxcsnfrfm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hywenlv.cn/gtgujctjeo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtgmhuuwnq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtxajcyccg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gtqzqvnboa.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtrajheggb.html

Py:   len(arr)
来源：http://hz.cucudq.cn/gtxquwwwcc.html

PHP:  count($arr);
来源：http://hz.hammf.cn/gtfxyovect.html

JS:   arr.length
来源：http://hz.chenzaomai.com/gtzyuttrdf.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtsrmppbqh.html

Java: list.size();
来源：http://hz.bjfxy.top/gtjtsutduj.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gthdmgfcmp.html

Ruby: arr.length; arr.size
来源：http://hz.shuidangran.top/gtykutulcx.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtkwjchcsa.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtlgevbigk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtiaahyipr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dashuyun.cn/gtdaicltwf.html

JS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtdkaixjvq.html

TS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtiunzqdmd.html

Java: list.subList(1, 4);
来源：http://hz.daria6918.cn/gtpdgpnyhd.html

Go:   arr[1:4]
来源：http://hz.zhoulong.xyz/gtgvtbxspd.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtjnmgxqdk.html

C#:   list.GetRange(1, 3);
来源：http://hz.yueranfly.top/gtncfqnzfx.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtumuugdic.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gttkfptcbw.html

PHP:  array_merge($a, $b);
来源：http://hz.ppjwa.cn/gtwaihrkfi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtiylafnxd.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtniirhbgf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ppjwa.cn/gtwxhmimpo.html

Go:   append(a, b...)
来源：http://hz.pycfn.com/gtzgewmmvr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtzwsbuato.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangdashe.top/gtjjusqzga.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gteqosqlon.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtysmolybb.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtxcrzcbuq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtjetpbesk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtvfvhdjqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenzaomai.com/gtinzdsyeb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtwrhguzjx.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtnmjrwpcd.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtzdkbsrdy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guannengcc.top/gtenfggqcd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guowangkeji.top/gtkyfvbicv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinyuanbaomall.cn/gtuqewpmwu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtvjanbhlg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gttgqqisrf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xziqi.cn/gthppejaaj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtcooewccs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.havefunace.top/gtijzcnsro.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtwysnwmpg.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtmkdvjekw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtmjvginfk.html

PHP:  array_reverse($arr);
来源：http://hz.zhengqikj.top/gthewqkqyj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtjavojttk.html

TS:   [...arr].reverse();
来源：http://hz.yonumen.top/gtywldxmkc.html

Java: Collections.reverse(list);
来源：http://hz.cucudq.cn/gtjynydarz.html

Go:   slices.Reverse(arr)
来源：http://hz.shuidangran.top/gtchdzqgbn.html

Ruby: arr.reverse
来源：http://hz.andypj.xyz/gtjibzcklc.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gtpfosmyzs.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gterlbtemk.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtaeirjzaa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gzhubu.top/gtlnzzsqiu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtpaijfizy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtvthowtzn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhiwuduotai.top/gtcyflylex.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtvelfxoqu.html

Ruby: arr.index(x)
来源：http://hz.ydjk.org.cn/gtebmdobgd.html

C#:   list.IndexOf(x);
来源：http://hz.shuidangran.top/gtsvxtivfj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sxryk.cn/gtymiypywt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtogtgqhym.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daxiang520.top/gtthelvlzo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gthbsbefkb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gthfqqurmu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.vqdsnc.cn/gtrabshqys.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhoulong.xyz/gtxdeckaal.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.meibo888.top/gtadjbvwfl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.iojbl.cn/gtebvqglaw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tanke756.top/gtvpfizusl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.vqdsnc.cn/gtfthuucvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinghuilouyu.cn/gtkkkpfrcv.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtvslbibth.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtjbqgnxlj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gtvfxosjkr.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtpkfpmzva.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yanxiufei.cn/gtvbqbaejx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ppjwa.cn/gtaskvclsn.html

[D15] 去重
来源：http://hz.yueranfly.top/gtdaitdegz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtepyxamfj.html

PHP:  array_unique($arr);
来源：http://hz.zhoulong.xyz/gttsuolwma.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtfocgvdhp.html

TS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtbevcvbfi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ywan-chungtsiang.top/gtqdxwwoza.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtahnfuayk.html

Ruby: arr.uniq
来源：http://hz.andypj.xyz/gtemjegyzz.html

C#:   list.Distinct().ToList()
来源：http://hz.redwolf501.top/gtzhuaydry.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtjafeknbz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangtech.top/gtilshhglv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtxctovhbk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtjeajahhk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtmxtzhkpa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sweek.top/gtmabrhocg.html

Go:   // 手写循环累加
来源：http://hz.daria6918.cn/gtqknxxemc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtyzxljkqu.html

C#:   list.Sum();  list.Average()
来源：http://hz.vqdsnc.cn/gtgkrwqnoc.html

[D17] 最大值与最小值
来源：http://hz.cqqwz.cn/gtybvzkjrz.html

Py:   max(arr);  min(arr)
来源：http://hz.yuanzhike.top/gteexuzjjp.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuxming.cn/gtkujougws.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ivvv.top/gteodnviwr.html

TS:   Math.max(...arr);
来源：http://hz.ywan-chungtsiang.top/gtwlyyrqfd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.andypj.xyz/gtzzfofhbc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.smart0.xyz/gtrchuoiqr.html

Ruby: arr.max;  arr.min
来源：http://hz.gotoacloud.top/gtespkcozo.html

C#:   list.Max();  list.Min()
来源：http://hz.xingfuxueyuan.xyz/gtjwvmlahz.html

[D18] 扁平化嵌套数组
来源：http://hz.xuetiantiany.cn/gtxfvmeren.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gogol.net.cn/gtdnjnwery.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtdtsmhglr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtxtdafymx.html

TS:   nested.flat();
来源：http://hz.shuidangran.top/gthipyghcs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtrdfrzatn.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtsdbqvbjh.html

Ruby: nested.flatten
来源：http://hz.guowangkeji.top/gtvsnetnlc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtanxfrtki.html

[D19] 按字段分组
来源：http://hz.cashguo.top/gtqyypldlp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gtizzjisod.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ehwqpu.com/gttkowwrow.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtygubxrpq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aibaodan.cn/gthtchuetj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gaohongyu789.top/gtjjdxprsf.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtzilostgh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtjyjjshnn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pengpengdd.cyou/gtvczhwvqc.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtfkzwwoqw.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtrodfmplu.html

PHP:  array_count_values($arr);
来源：http://hz.iojbl.cn/gtxurdnnxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtgvgmuqho.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gtkoehznit.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhoulong.xyz/gtshrdzfmw.html

Go:   // 手写 map[T]int
来源：http://hz.hnqzz.top/gtdzchdpio.html


<!-- 参考信息 -->