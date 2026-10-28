代发 wailian999

Java: if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gteyognnvq.html

Go:   if data == nil { return }
来源：http://hz.pycfn.com/gtkzytkinx.html

Ruby: return if data.nil?
来源：http://hz.yanxiufei.cn/gtapqzhyzj.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtnaeeqkli.html

================================================================================
来源：http://hz.9152youxi.cn/gtnzhoqtnf.html

C. 函数与作用域
来源：http://hz.gotoacloud.top/gtspifqsjt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpnbbckqg.html

[C01] 定义函数
来源：http://hz.zhiwuduotai.top/gtiwmsmfkg.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtifhitlru.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtnqlpoakr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtvxcpxpcq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtochamowt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gttjcafaft.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenzaomai.com/gtjittvadp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhixingplan.top/gtfgajfswa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtctzpeixx.html

[C02] 默认参数
来源：http://hz.yj202588.top/gtvmejvpce.html

Py:   def greet(name="World"): return name
来源：http://hz.chenjidiqi.icu/gtvomopkjq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ivvv.top/gtmrekvxym.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xziqi.cn/gtshgrppwv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtdmfcsvht.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yonumen.top/gtnuztgmsb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtnqdculen.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtfqjrrxzz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.bjfxy.top/gtndxmctgf.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gthxfwqilt.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuxming.cn/gtsfgrerki.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shuidangran.top/gttbdmwwcq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtkanrlwaa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtbmtcutlv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aizwys.cn/gtvhcuodld.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.aizwys.cn/gtujnpzysx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gtphczfnjo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nanxinkj.top/gtnmjlhdsd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtbnmggqef.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gtfqcpvthw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gogol.net.cn/gtujobnsyj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtuktxdltu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fengsongda.top/gtkszewgjr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtqpccixol.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gtjpmthvtk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtfgybtyzj.html

C#:   f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtyzdxfrkj.html

[C05] 返回多个值
来源：http://hz.nanxinkj.top/gtrukwuvwc.html

Py:   return a, b
来源：http://hz.guowangkeji.top/gtagrcpbft.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gtswdklyvp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tian-w.cn/gtuqjvmiwd.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtbbjitnij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yangfankeji.com/gtrzktoeeq.html

Go:   return a, b
来源：http://hz.wangshuangyany.cn/gthkxfdrqa.html

Ruby: return a, b
来源：http://hz.gzhubu.top/gtiyzycfqg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.316326.xyz/gthzjlcmlb.html

[C06] 匿名函数 / lambda
来源：http://hz.xuanzx.com/gtzttbgcnq.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtwygwbcjc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ybcxt.top/gtwwmpcgos.html

JS:   const square = x => x * x;
来源：http://hz.ywan-chungtsiang.top/gtnwrklpkl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtcpcffmvw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtknxgbreo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daxiang520.top/gtxvqnxkpl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtmlfgeulu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtqrorrlvt.html

[C07] 把函数作为参数传入
来源：http://hz.guannengcc.top/gtsqozhyff.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258.top/gtdzhabgui.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xziqi.cn/gtcbzcosar.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jianghu66.top/gtwmuehkwj.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gtvigzusfo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xinyue.icu/gtdfbajqjd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhongyouzk.top/gtvfwncdnl.html

Ruby: arr.map(&:upcase)
来源：http://hz.cdnleiting.top/gtlgnynlzd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gaohongyu789.top/gtdhmtpwfk.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtuzbcxmer.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxinkj.top/gtkvbvbopb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shuidangran.top/gtxjwvgblb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtjlfxjvkb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtxpmeozhi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigufen.top/gtcxvisite.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtjeuhqwor.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hfpthk.cn/gtwvgbhcpq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtadumqfud.html

[C09] 递归
来源：http://hz.zhongyouzk.top/gtwsoaqytn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gttpinhsxl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgfzy.top/gtgsgygsfe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gthiicodpe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtifqoukjz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xziqi.cn/gtakjcxpwb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jyoumei.cn/gtrmjaaehi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fengsongda.top/gtbrbrusdy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtkguzbxri.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtiqjfbglc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtyfyofqjq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gtjolzheqd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtqbhnbwwk.html

TS:   同 JS
来源：http://hz.gzhubu.top/gtswimxdjw.html

Java: 方法内为块级作用域
来源：http://hz.jlsjyb.cn/gtbuvanfth.html

Go:   花括号块级作用域
来源：http://hz.jinqigufen.top/gtbxwgwfmz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtxyobzvok.html

C#:   块级作用域
来源：http://hz.316326.xyz/gthbbvjlit.html

[C11] 模块导入与导出
来源：http://hz.yueranfly.top/gtqwmudkji.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtukpijilw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigufen.top/gtpqddfjch.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gzhubu.top/gtgvrdatso.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nwbrower.top/gtsgzbaivj.html

Java: import java.util.List;
来源：http://hz.vqdsnc.cn/gtnnmhcdst.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nwbrower.top/gteddyxzch.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gthicnfpoi.html

C#:   using System.Text;
来源：http://hz.snrcjt.cn/gtbhdjogff.html

[C12] 立即执行函数 IIFE
来源：http://hz.aizwys.cn/gtfgussgin.html

Py:   (lambda: print("run"))()
来源：http://hz.316326.xyz/gtesazeust.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ppjwa.cn/gtcqoxdldq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtfqtyjrcy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtkfxpuque.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtwlbjdarl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nwbrower.top/gtppfmiudf.html

Ruby: -> { puts "run" }.call
来源：http://hz.yvedp.cn/gtbhpwchpp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hammf.cn/gtnsgbfrtb.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtxddwdddq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuxming.cn/gtwvehsgnu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gtlyzymbtt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtzxhasluv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtpmaaqloj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtktyvsozx.html

Go:   func add(a, b int) int
来源：http://hz.jqgfzy.top/gtqkwzpnlx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xziqi.cn/gtwgyvxtpa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gthexfzqzp.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtosaapuuf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xylfe.cn/gtzdbjyhqr.html

PHP:  // 无泛型
来源：http://hz.vqdsnc.cn/gtcejssdvd.html

JS:   // 无泛型
来源：http://hz.zhiwuduotai.top/gtejgtxzrq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gthbogftzb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.smart0.xyz/gtmshsrzwf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhiwuduotai.top/gtrbwwppmi.html

Ruby: # 无泛型
来源：http://hz.tian-w.cn/gtlxsnpees.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hywenlv.cn/gtlxahsror.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtrmtjmrco.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cqqwz.cn/gtrnyqihcp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnqzz.top/gtvxnjpbol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtfduvqdzo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangshuangyany.cn/gtfktjpezt.html

Java: // 无解构
来源：http://hz.birdmap.top/gtsmvkkjnx.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtmiwlrdmf.html

Ruby: a, b = pair
来源：http://hz.jlsjyb.cn/gtfhujhkye.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtjzjiorki.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtnwxbjpzu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.316326.xyz/gtxygcldca.html

PHP:  // 无重载
来源：http://hz.zhongyouzk.top/gtegdbwlff.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.andypj.xyz/gtaywzsknw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.svipenyu.cn/gtmdzqtpby.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxinkj.top/gttaxjyycq.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtesoesthg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgufenzy.top/gtcyfxiyjb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.mhx1999.top/gtjpcumypz.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtyrbryadn.html

D. 数组 / 列表 / 集合
来源：http://hz.mhx1999.top/gtpbpqgcci.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gteotmwkfd.html

[D01] 创建数组 / 列表
来源：http://hz.ybcxt.top/gtfgyxacak.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtpyikaxgt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jianghu66.top/gtpjpqyvrr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tian-w.cn/gtjkrwycyd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.snrcjt.cn/gtojbrsdmh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yanxiufei.cn/gtiwbsmojv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gtuzcmywle.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fengsongda.top/gtdetrydtf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jiagoushi.top/gtabkvhwjg.html

[D02] 追加元素到末尾
来源：http://hz.yonumen.top/gtsydsdaan.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtibwseyma.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtlcklgbmv.html

JS:   arr.push(4);
来源：http://hz.yongpay.top/gtlmpohufc.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtugdcudjg.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtraugrlfs.html

Go:   arr = append(arr, 4)
来源：http://hz.hywenlv.cn/gtdwkjmkku.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.havefunace.top/gteeizfgwe.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtrmoazsah.html

[D03] 在指定位置插入元素
来源：http://hz.jinyuanbaomall.cn/gtasecrjbr.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gthalrvnip.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtsbdzoxzp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cqqwz.cn/gtwkswpzqg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtbvyrgduh.html

Java: list.add(0, 0);
来源：http://hz.haohaochexian.top/gtbgpskaoa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.bjfxy.top/gtxbxhfwjv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangshuangyany.cn/gttzuydwiy.html

C#:   list.Insert(0, 0);
来源：http://hz.yuanzhike.top/gtykcnbmck.html

[D04] 删除元素
来源：http://hz.jinqigfzy.top/gtjthnurhl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtejcushth.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangshuangyany.cn/gtnlrygxgo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.bjfxy.top/gtggdqzuej.html

TS:   arr.splice(0, 1);
来源：http://hz.yvedp.cn/gtzpifufzk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhoulong.xyz/gtjxleqwgx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtloedgjxe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fengsongda.top/gthdbkjfxf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.iojbl.cn/gtadntydcc.html

[D05] 访问与修改元素
来源：http://hz.jinqigufen.top/gtmpgbjrbz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtrvrgocuw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtntctrkaq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tianlin.xyz/gtohsgnyzr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhongyouzk.top/gteypmickz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtzrmteusy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtoelpiwkx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gttzqlhzhe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.meibo888.top/gtzsszsgio.html

[D06] 数组长度
来源：http://hz.zhoulong.xyz/gtginoikxe.html

Py:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtobnbezdr.html

PHP:  count($arr);
来源：http://hz.shanyushiyangkeji.top/gtgnwsbrjj.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gtuyafxtjm.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtgagypzbw.html

Java: list.size();
来源：http://hz.sufxvd.cn/gtvheeeksu.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtehuzpegr.html

Ruby: arr.length; arr.size
来源：http://hz.xylfe.cn/gtshlyskog.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtfavnxeki.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtdjbjhvbo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gtlkpeitit.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zycfv.cn/gtyvmpxtpj.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gthoypbygn.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtjnuqlaee.html

Java: list.subList(1, 4);
来源：http://hz.shangyingyoupin.top/gtiqwrvpfs.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gtwztqofzy.html

Ruby: arr[1, 3]
来源：http://hz.gaohongyu789.top/gteijzdqmk.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtgarpzbvv.html

[D08] 合并两个数组
来源：http://hz.fengsongda.top/gtsxulwcrd.html

Py:   a + b;  a.extend(b)
来源：http://hz.xziqi.cn/gtasofyiut.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtjlxafqtx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhaomingkeji.xyz/gtzmtbgwac.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtrkobemso.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtczuuuelt.html

Go:   append(a, b...)
来源：http://hz.jinqigfzy.top/gtiyykewrr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtsaaqwxcz.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtejzpqyse.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtcnwmktsv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtfyiszjzc.html

PHP:  sort($arr);
来源：http://hz.xuetiantiany.cn/gtivwwqjsm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtalmyotvc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuxming.cn/gtdgeyutum.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gtaopefehc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtpkvhsfav.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtvxxsiwht.html

C#:   list.Sort();
来源：http://hz.snrcjt.cn/gtclnvhofk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gthojtfduv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtkaryhmbn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtzrazycda.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtkexulotu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtxwwyneih.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aizwys.cn/gtlkvuwoyq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.0kj1m.cn/gtnjljdxbv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangtech.top/gtutsckgev.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtoahakgww.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtzenzjnzl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgufenzy.top/gtemptskta.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtperafmhu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtfqnvqzyn.html

TS:   [...arr].reverse();
来源：http://hz.quarkkingdee.top/gtoyogdtkk.html

Java: Collections.reverse(list);
来源：http://hz.gotoacloud.top/gtpltmphxf.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtxqquoirr.html

Ruby: arr.reverse
来源：http://hz.jqgufenzy.top/gtqfbwijji.html

C#:   list.Reverse();
来源：http://hz.smart0.xyz/gtzletvwly.html

[D12] 查找元素下标
来源：http://hz.zhiwuduotai.top/gtbxstxmar.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtyltgmjto.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtaxsnhtzw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtreztgsxk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtzghimwvw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtxedtxoaq.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxuanxn.top/gtvljckbwp.html

Ruby: arr.index(x)
来源：http://hz.nwbrower.top/gttwcjkqib.html

C#:   list.IndexOf(x);
来源：http://hz.shangyingyoupin.top/gtdsoxozab.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gtezqpmxxh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtcpvvpltv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cashguo.top/gttwuorpit.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtalgvpuem.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtkmukrsnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinyuanbaomall.cn/gtnhsnemhy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gttnyrvtzo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zycfv.cn/gtvbrprpdz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gtubbjuxgo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtmotpffpp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhiwuduotai.top/gtrctyucye.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gtfmamtpro.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtieujxmvs.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtcnyipecw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.svipenyu.cn/gtzexfbhtt.html

Go:   // 手写循环
来源：http://hz.dashuyun.cn/gtthfmckge.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pycfn.com/gttdecmlky.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gtmsbczxnu.html

[D15] 去重
来源：http://hz.ivvv.top/gtsjcctbso.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangkeji.top/gtqiadgpcl.html

PHP:  array_unique($arr);
来源：http://hz.yj20258888.top/gtbgfmoqrr.html

JS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtafdacwks.html

TS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtnymlgwna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtqbcnndcb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cdnleiting.top/gtjsybioin.html

Ruby: arr.uniq
来源：http://hz.smart0.xyz/gtdqjuccaz.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtbccfmulc.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtyfijzcaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fengsongda.top/gttwbxdaua.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtivytxcpa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtdqshryml.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtneaygluu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.9152youxi.cn/gtjtkiwhns.html

Go:   // 手写循环累加
来源：http://hz.vqdsnc.cn/gtcvipchwe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zdqjudy.top/gthnytcvxs.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258888.top/gtjvbzyjzr.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gteqohspfu.html

Py:   max(arr);  min(arr)
来源：http://hz.hysaishi.cn/gtrkblhwdl.html


<!-- 参考信息 -->