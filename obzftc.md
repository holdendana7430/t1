代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gttofysqvq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yonumen.top/gtgfqidzhi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtjenrywna.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gotoacloud.top/gttfhfrbxu.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtigxkhpps.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtqlonrdil.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gttiwqbzij.html

[C05] 返回多个值
来源：http://hz.yanxiufei.cn/gtlzrxpgms.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtwzdpcuom.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtpuzxpybx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.quarkkingdee.top/gtarkcwacp.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gtvlmdefhu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtfoiiqekv.html

Go:   return a, b
来源：http://hz.hongshengwenyu.top/gtmzsqflsz.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gtixdgeept.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtqgoiomzb.html

[C06] 匿名函数 / lambda
来源：http://hz.sufxvd.cn/gttqmjxgaq.html

Py:   square = lambda x: x * x
来源：http://hz.ywan-chungtsiang.top/gtueygiuew.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtenjbsaqb.html

JS:   const square = x => x * x;
来源：http://hz.dashuyun.cn/gthryhelmv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jyoumei.cn/gthyxhdxrb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.c1oappe.top/gtvyydmysj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gtsokmqhzz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.andypj.xyz/gtogcvtxxa.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cashguo.top/gtytdvwaop.html

[C07] 把函数作为参数传入
来源：http://hz.yanxiufei.cn/gtozvpparg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jlsjyb.cn/gtdkxvqarl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jyoumei.cn/gtdbuvcnfm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtuqrsbtxj.html

TS:   arr.map(String)
来源：http://hz.havefunace.top/gtkiofbuge.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yanxiufei.cn/gtztwxywrv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sweek.top/gtvrbmzexm.html

Ruby: arr.map(&:upcase)
来源：http://hz.zdqjudy.top/gtcxvtruea.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtzeehdbbq.html

[C08] 闭包
来源：http://hz.bjfxy.top/gtuloqhvrz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtvriztpvs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.iojbl.cn/gtuinxmiro.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtbuhxtuoz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gttdocdolq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jiagoushi.top/gtxfukdytw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxuanxn.top/gtmbezhqkh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aibaodan.cn/gtfqfiasgx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtstvyntny.html

[C09] 递归
来源：http://hz.jqgufenzy.top/gttrqvzljc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtrmrtmigp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.nwbrower.top/gttbgrmenf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gttjvurvtn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtamumkwow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yvedp.cn/gteadmercw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ivvv.top/gtpxydtciz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtfneuipdj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yvedp.cn/gtcrctwdom.html

[C10] 变量作用域
来源：http://hz.0kj1m.cn/gtdkyutvxm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cqqwz.cn/gtdqzrilnx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtytcelgin.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guannengcc.top/gtmuqahebg.html

TS:   同 JS
来源：http://hz.shuidangran.top/gtujaywhnu.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtarovslfs.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtbjrcktvz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhoulong.xyz/gtvtkftaom.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtvuvkmawr.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtyfujwrmw.html

Py:   from module import func
来源：http://hz.zdqjudy.top/gtyblypnnm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zycfv.cn/gtcvobbepo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtzrilwmyn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigfzy.top/gthpcniqku.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gtqfjydgbi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtpikrsfuf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.svipenyu.cn/gttijmsvbu.html

C#:   using System.Text;
来源：http://hz.havefunace.top/gtsdhawvfh.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gtgajnxndf.html

Py:   (lambda: print("run"))()
来源：http://hz.xingfuxueyuan.xyz/gttpkapxib.html

PHP:  (function () { echo "run"; })();
来源：http://hz.bjfxy.top/gtjajnhzls.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtxfxiqsgx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shzxlz.cn/gtwwhhlijg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gtfmtdeuvg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinyuanbaomall.cn/gtnxjmevec.html

Ruby: -> { puts "run" }.call
来源：http://hz.dashuyun.cn/gtqoscijcu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hysaishi.cn/gtjqtqqnbv.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtnwuamdpw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtqnnwmuzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtxponexuy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtolmcywkn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtnupquwdt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtgblloorp.html

Go:   func add(a, b int) int
来源：http://hz.hfpthk.cn/gtpkqjmgfs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangshuangyany.cn/gthzzvaeix.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gtyvkvstnr.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtotlndoco.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gttdhlxabt.html

PHP:  // 无泛型
来源：http://hz.yueranfly.top/gtvfigrfmu.html

JS:   // 无泛型
来源：http://hz.tian-w.cn/gtdfiqayle.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhixingplan.top/gttmbowuuf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtnmvnhjky.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gtudvpwhnh.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtrijxcpox.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gaohongyu789.top/gtdcbnvakz.html

[C15] 解构 / 展开参数
来源：http://hz.xingfuxueyuan.xyz/gtgfkgxzyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtewkobspt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.0kj1m.cn/gtutacmmmq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gtktjxxudp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gaohongyu789.top/gtknlmvpwl.html

Java: // 无解构
来源：http://hz.iojbl.cn/gtwwwrzrvb.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtfvtnqrcg.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gtrvkmdctg.html

C#:   var (a, b) = pair;
来源：http://hz.jinghuilouyu.cn/gtbheitgoq.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtpdwtssmp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xingfuxueyuan.xyz/gtqhpklkby.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtmkuwgrol.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigfzy.top/gtyomphtji.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cdnleiting.top/gthgydzwlm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gthhfwwzhf.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtnqmsnevr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtphdlnvep.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gtyplrrzgk.html

================================================================================
来源：http://hz.cqqwz.cn/gtvtocewlg.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gtwrwopqvv.html

================================================================================
来源：http://hz.svipenyu.cn/gtdkttwdrs.html

[D01] 创建数组 / 列表
来源：http://hz.hongshengwenyu.top/gtzxkywiho.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fzhhl.top/gtmfwcmdnr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtmoxvwnxz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenjidiqi.icu/gtbakkyxex.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gtqcywaizh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shzxlz.cn/gtdimwiomt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtvnllhmgg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtguwhoedk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtctdeimpz.html

[D02] 追加元素到末尾
来源：http://hz.havefunace.top/gtdrssvwok.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtjtemjqtp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtuguyyrxc.html

JS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtypahmugp.html

TS:   arr.push(4);
来源：http://hz.daria6918.cn/gtvqlwftbr.html

Java: list.add(4);
来源：http://hz.zhijiandao.cn/gtvfkvvfpa.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtsdimkoyh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.mhx1999.top/gtubjhxjdn.html

C#:   list.Add(4);
来源：http://hz.iojbl.cn/gtfqotpalu.html

[D03] 在指定位置插入元素
来源：http://hz.hywenlv.cn/gttephswaz.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtmjjvmwty.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gtaqpglogf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xziqi.cn/gtcmzllwnn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.guannengcc.top/gtizfyvzus.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gthmxgnbmi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj202588.top/gtdblnlwdm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtnnplfgpt.html

C#:   list.Insert(0, 0);
来源：http://hz.0kj1m.cn/gttvvkxyyf.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtvabumbps.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258.top/gtzhbypoya.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ybcxt.top/gtgpwwobcz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sxryk.cn/gtcjmdfukq.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gtvxjdnutw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gtmhzqmwwn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gteztvhkag.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gtldsherdm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gtvqsziqrt.html

[D05] 访问与修改元素
来源：http://hz.fengsongda.top/gtfuwlqvmz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtetndxmzz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtcawpnbcq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sxryk.cn/gtdpolwbzd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtumjynout.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.quarkkingdee.top/gtksnlhzry.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtdiiincos.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtpemywclb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gttjuiwoyn.html

[D06] 数组长度
来源：http://hz.daria6918.cn/gtjeivvxfe.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtlmxcmsux.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtnppqqqsw.html

JS:   arr.length
来源：http://hz.chenlongwang.top/gtxhhujaog.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gtwfybpynu.html

Java: list.size();
来源：http://hz.daria6918.cn/gtkpehwntx.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtcyfffnjt.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtorcfcwma.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtvqxqltoq.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigfzy.top/gtsycmxkpa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gtrafrrgki.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gtnmqdelnl.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtmvadpwks.html

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtgxnsakuy.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtpvjeoyoh.html

Go:   arr[1:4]
来源：http://hz.iojbl.cn/gtxetzloqj.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtoevjnawq.html

C#:   list.GetRange(1, 3);
来源：http://hz.havefunace.top/gthsvmbqsy.html

[D08] 合并两个数组
来源：http://hz.dashuyun.cn/gtexghxtrr.html

Py:   a + b;  a.extend(b)
来源：http://hz.mhx1999.top/gthcfamagq.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtomekibgi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigufen.top/gtwofsmjnd.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtxltuxfec.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.wangshuangyany.cn/gtuknuyaem.html

Go:   append(a, b...)
来源：http://hz.zhijiandao.cn/gtzugqglov.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gtjqsqoxah.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgufenzy.top/gtdadpykxc.html

[D09] 排序（升序）
来源：http://hz.hongshengwenyu.top/gtewszplrx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtjniakbmf.html

PHP:  sort($arr);
来源：http://hz.zhaomingkeji.xyz/gtyemtlxwp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.kuanghao11.cn/gtjjulrsqn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtebirbpyp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fengsongda.top/gtkhudutzg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnqzz.top/gtqfqlvjso.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtgmnwkhyg.html

C#:   list.Sort();
来源：http://hz.chenzaomai.com/gtzohowlei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtpmwhucxx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gtiojtknjy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtghrfjagx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtiizflqha.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtykaqgzow.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtqcwchtkv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtseuhizfx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydjk.org.cn/gtiuqyaxlo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gthdvotzzl.html

[D11] 反转数组
来源：http://hz.birdmap.top/gtxarbizgz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hammf.cn/gtyexcqrda.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtxjakpvdi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtfxdhslqq.html

TS:   [...arr].reverse();
来源：http://hz.zycfv.cn/gtafvtaihg.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtqfcfxedp.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtdpoxgtmj.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gtxomhhwhe.html

C#:   list.Reverse();
来源：http://hz.snrcjt.cn/gtzluiixpw.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtksltyemp.html

Py:   arr.index(x);  x in arr
来源：http://hz.iojbl.cn/gtnhpuvnqg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtiblccvnt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtmshaybtm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtlztvwppy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydjk.org.cn/gtexshqywo.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxuanxn.top/gtgjfcozgp.html

Ruby: arr.index(x)
来源：http://hz.yj202588.top/gtbjsyfjhg.html

C#:   list.IndexOf(x);
来源：http://hz.yangfankeji.com/gtnjqervdt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258.top/gtksznoswy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ywan-chungtsiang.top/gtqivteicb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtzhqllegj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtwautdoes.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtgfvyhcym.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtcksjvarg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangshuangyany.cn/gtqogixlyk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtxiyctqzw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydjk.org.cn/gtimcxdwpk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhiwuduotai.top/gtklkcyuzd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gteolryrqg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.52xcode.cn/gtmneelldi.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtjnxbaqke.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtkcglcopl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hammf.cn/gtmqzcaekv.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtxcdwaxjt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.havefunace.top/gtkaoaoxzv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtlzcdbvyq.html

[D15] 去重
来源：http://hz.feifeiyinyue.top/gtznxuuixf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinyuanbaomall.cn/gtqwapolfk.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtbeihakcn.html

JS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtiwreedlp.html

TS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtgrslqrpk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gtnizmxbla.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtywnijaub.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangtech.top/gtrkbogxkn.html

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtxkmsdako.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gtrdmzudtu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gteegwgjyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtbxushcrl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtjuehyshq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtxrcbjxpv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sweek.top/gtwzarybdr.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtbycrjybt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.mhx1999.top/gtrqpuqcde.html

C#:   list.Sum();  list.Average()
来源：http://hz.yongpay.top/gtewojtwkz.html

[D17] 最大值与最小值
来源：http://hz.nanxinkj.top/gtnzibsday.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtcxldctiq.html

PHP:  max($arr);  min($arr);
来源：http://hz.jianghu66.top/gtfewalxlr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtzevlubiq.html

TS:   Math.max(...arr);
来源：http://hz.mhx1999.top/gtvlixnkxd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.316326.xyz/gtknmtnhqu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gthgcxneah.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtcmtcdfni.html

C#:   list.Max();  list.Min()
来源：http://hz.kuanghao11.cn/gtxpulaitu.html

[D18] 扁平化嵌套数组
来源：http://hz.hongshengwenyu.top/gtyzbwhikf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yvedp.cn/gtksldvqsb.html

PHP:  array_merge(...$nested);
来源：http://hz.yanxiufei.cn/gtzivhteom.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cdnleiting.top/gtdrinclmz.html

TS:   nested.flat();
来源：http://hz.jinghuilouyu.cn/gtlgbahmow.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnxiangtu.top/gtbtcaruuj.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtpvxbschb.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtwfwxrhvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhiwuduotai.top/gtpagnbfyc.html

[D19] 按字段分组
来源：http://hz.jianghu66.top/gtzefybdnf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtnpyhrtxv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shzxlz.cn/gtfcawsrvi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhijiandao.cn/gtknrfbimk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtwzwajzam.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtkromfbdx.html

Go:   // 手写 map[string][]T
来源：http://hz.bjfxy.top/gtqzvjjlto.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtxndwitlw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtphjvlyyz.html

[D20] 统计每个元素出现次数
来源：http://hz.316326.xyz/gtpgczhkmo.html

Py:   Counter(arr)
来源：http://hz.chenzaomai.com/gtjoszxwvz.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtenpzsnqz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtsxogpjki.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtdkzgtbmt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangtech.top/gtnfromaed.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtucwsitkr.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtwnocprxv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtwstlilhz.html

[D21] 判断是否包含某元素
来源：http://hz.jyoumei.cn/gttdxgszei.html

Py:   x in arr
来源：http://hz.zdqjudy.top/gtaxdsscab.html


<!-- 参考信息 -->