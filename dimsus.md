代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtzcidsnwj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tanke756.top/gtxvbwjkjd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangshuangyany.cn/gtjdtodijz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtxalkgrlx.html

[C02] 默认参数
来源：http://hz.dianchejie.cn/gtmdgpohfo.html

Py:   def greet(name="World"): return name
来源：http://hz.hysaishi.cn/gtasiiqaig.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.quarkkingdee.top/gtbzxdwaco.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.guannengcc.top/gtbmolmzvt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gthlduwcue.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258.top/gttvzpwlcs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.andypj.xyz/gtpitppnix.html

Ruby: def greet(name = "World") = name
来源：http://hz.gzhubu.top/gtkbfwlbxr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ybcxt.top/gtidcskdsz.html

[C03] 可变参数
来源：http://hz.cqqwz.cn/gtmiemydaz.html

Py:   def total(*args): return sum(args)
来源：http://hz.meibo888.top/gtpgwxqptz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtcoghjods.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gttmapwmgl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtvrypweyb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yangfankeji.com/gthxbexuho.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tianlin.xyz/gtfhqgsfax.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jiagoushi.top/gtmnoixepj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenjidiqi.icu/gtmgsqrvfr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guowangkeji.top/gtrmxequws.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtrhvnhyfo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yongpay.top/gtukhmhdhx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtkutanbdd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gtzvssketx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtnqmifopf.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gtgldnksgz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtmlzrncbj.html

C#:   f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtazsfaveg.html

[C05] 返回多个值
来源：http://hz.ybcxt.top/gtpoupiccv.html

Py:   return a, b
来源：http://hz.316326.xyz/gtesvmaqge.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtxomcyoxh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtekajachx.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gtbgwtdzop.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtgzdvutlz.html

Go:   return a, b
来源：http://hz.xinyue.icu/gtzdtxnopb.html

Ruby: return a, b
来源：http://hz.yj20258.top/gtgenvbndf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinghuilouyu.cn/gttlskycnr.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtzjhwifxm.html

Py:   square = lambda x: x * x
来源：http://hz.zhengqikj.top/gttutfxotc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtpgftjoie.html

JS:   const square = x => x * x;
来源：http://hz.feifeiyinyue.top/gtwvctyhgc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hammf.cn/gtrvejbfgw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gtvgfmzfou.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fzhhl.top/gthjjlauqr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenzaomai.com/gtbeyxkbdi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtvrnqxtln.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gtxwpmdvnc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtepgkivce.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.0kj1m.cn/gtbtjufmxu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sxryk.cn/gtrnyfsfpy.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtuflkinao.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtarliykhb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuanzx.com/gtfuaapkiw.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxinkj.top/gtsvadxxgq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtqdhhsylc.html

[C08] 闭包
来源：http://hz.havefunace.top/gtvfznkydt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xinyue.icu/gtlirljsxn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ybcxt.top/gtnmojgqak.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtyybirhsu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtbbjlmsyp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gturodalmg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gtmdncaejr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zycfv.cn/gtvjjoexbd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtvdqsavda.html

[C09] 递归
来源：http://hz.jyoumei.cn/gtbiklamtv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.mhx1999.top/gtvvgcwusf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtoskzwuwn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtpnyfwbcl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtpgaqtmlr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hammf.cn/gteyycjcux.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtkewssfml.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtcfbvomgi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yangfankeji.com/gthotdeebs.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtuydonwhq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhongyouzk.top/gtziuuskwj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtgnoockvj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtedvyotov.html

TS:   同 JS
来源：http://hz.xingfuxueyuan.xyz/gtnlqortpk.html

Java: 方法内为块级作用域
来源：http://hz.vqdsnc.cn/gttzyzvngy.html

Go:   花括号块级作用域
来源：http://hz.guowangkeji.top/gthuzcbpzb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinyuanbaomall.cn/gtmmabmkke.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtmtzskisn.html

[C11] 模块导入与导出
来源：http://hz.xingfuxueyuan.xyz/gtqusiloln.html

Py:   from module import func
来源：http://hz.aibaodan.cn/gtetenkyly.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shangyingyoupin.top/gtxdwszawj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.vqdsnc.cn/gtqeguejno.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtridpeoer.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gtlaodjjrf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sweek.top/gtgiyhjezf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tianlin.xyz/gtpouckbgg.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtdcdrxttz.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhengqikj.top/gthqqoqzob.html

Py:   (lambda: print("run"))()
来源：http://hz.snrcjt.cn/gtitasbgeh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hongshengwenyu.top/gtydgcwfbn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtlkzekcpp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shzxlz.cn/gtwusdxlgj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guowangkeji.top/gtczfyadgr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pengpengdd.cyou/gtvpmlhrgp.html

Ruby: -> { puts "run" }.call
来源：http://hz.zycfv.cn/gtwxsfpzcu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cdnleiting.top/gtuayzylxm.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxinkj.top/gttjyifvpx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shuidangran.top/gtqhugbhdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gthqupgkfv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhoulong.xyz/gtmfnkogxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtiqcvfyps.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtvloqamog.html

Go:   func add(a, b int) int
来源：http://hz.hnqzz.top/gtxcfcqhxc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtqhesqznh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sysykeji.top/gtszfrqemb.html

[C14] 泛型函数
来源：http://hz.aibaodan.cn/gthrsdwfzu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daria6918.cn/gthacuhjve.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtapvuodqa.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtnbsqtedc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtlmhralor.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj202588.top/gtnmncmuor.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.pengpengdd.cyou/gtowoxfkvx.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtbrpktnsn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.redwolf501.top/gtwarmbjof.html

[C15] 解构 / 展开参数
来源：http://hz.zdqjudy.top/gtgcenioys.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigfzy.top/gtbuugwnba.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuanzhike.top/gtvgymltlv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gtgshgdhpk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gtiwrueusg.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtxtzonhku.html

Go:   // 无解构
来源：http://hz.yj202588.top/gtjgtviadw.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtzuhhkhgu.html

C#:   var (a, b) = pair;
来源：http://hz.daxiang520.top/gtutnomsol.html

[C16] 函数 / 方法重载
来源：http://hz.bjfxy.top/gtmnuijvjq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.smart0.xyz/gtfdbrtjmw.html

PHP:  // 无重载
来源：http://hz.yvedp.cn/gtxzujseon.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangkeji.top/gtiyzgrcnd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sweek.top/gtkkyajryn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydjk.org.cn/gtorgduapb.html

Go:   // 无重载：用不同函数名
来源：http://hz.cdnleiting.top/gtlwxqylde.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydzc1.top/gtbpsxsedg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gthtlnurhf.html

================================================================================
来源：http://hz.meibo888.top/gtgdthuime.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtjpyehdom.html

================================================================================
来源：http://hz.9152youxi.cn/gttxznsmca.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gtsvsqeoei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yangfankeji.com/gtsduuaoij.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gtocxmdqwr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gtvbcshkgg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangshuangyany.cn/gtycxbjwbe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuxming.cn/gtoaqrugzs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.quarkkingdee.top/gtccsetgkk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtqwucbbfa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtlsmkhijo.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtanzekaed.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.birdmap.top/gtfosjircg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhoulong.xyz/gttadqauer.html

JS:   arr.push(4);
来源：http://hz.xylfe.cn/gtejwtosru.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtjmkpqlbk.html

Java: list.add(4);
来源：http://hz.ehwqpu.com/gtunefceho.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtibmalbdx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gtiejibbap.html

C#:   list.Add(4);
来源：http://hz.tanke756.top/gtfjmwxddo.html

[D03] 在指定位置插入元素
来源：http://hz.wangdashe.top/gtpvbwlwpx.html

Py:   arr.insert(0, 0)
来源：http://hz.zhongyouzk.top/gtnutnlrid.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ywan-chungtsiang.top/gtbtnztrbu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtpsejxocf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.c1oappe.top/gtyxzifsvs.html

Java: list.add(0, 0);
来源：http://hz.xingfuxueyuan.xyz/gthzqdlqxn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jianghu66.top/gtueekfpyu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ehwqpu.com/gtmcexlfmy.html

C#:   list.Insert(0, 0);
来源：http://hz.yonumen.top/gtoackzxif.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtgslgitpu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtgwopwbfq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtgvtrqmvu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtwzoobiit.html

TS:   arr.splice(0, 1);
来源：http://hz.daria6918.cn/gtccfmbrha.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenzaomai.com/gtrqkdsoyu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtutwwtavc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jlsjyb.cn/gtvvtnzlws.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cheryme.top/gtoklvfezo.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gtrfewslxp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.birdmap.top/gtvlbmlqcv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aizwys.cn/gtxzxhywjz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtsetkqzbx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtdtwxqllq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gtzqhwymqe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtqikwjhbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gttpemdveu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cashguo.top/gthkrjqlci.html

[D06] 数组长度
来源：http://hz.shanyushiyangkeji.top/gtviqijctp.html

Py:   len(arr)
来源：http://hz.zhiwuduotai.top/gtphmfgpko.html

PHP:  count($arr);
来源：http://hz.yongpay.top/gtmxifmqim.html

JS:   arr.length
来源：http://hz.hammf.cn/gtfnyqpday.html

TS:   arr.length
来源：http://hz.c1oappe.top/gtjlwrrdec.html

Java: list.size();
来源：http://hz.zycfv.cn/gtortzvnnk.html

Go:   len(arr)
来源：http://hz.tianlin.xyz/gtykflorbo.html

Ruby: arr.length; arr.size
来源：http://hz.svipenyu.cn/gticgyfwli.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtmujbggko.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtjrdpvkst.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cucudq.cn/gtalnibkef.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yueranfly.top/gtoixxpxda.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtttphbssp.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtlwiabtni.html

Java: list.subList(1, 4);
来源：http://hz.yvedp.cn/gtzeyxnktr.html

Go:   arr[1:4]
来源：http://hz.sweek.top/gteomfbhfl.html

Ruby: arr[1, 3]
来源：http://hz.zycfv.cn/gtbloipbjj.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gtmadoulzs.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtdusxpuyp.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtnyheques.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtrtrhmtxr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydzc1.top/gtpyxbplvf.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gtkoelgwab.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daria6918.cn/gtwlfdreum.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtjleqdiji.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtayhjfksz.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtzkyhvbjx.html

[D09] 排序（升序）
来源：http://hz.tanke756.top/gtfytwtksg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtvppvmxca.html

PHP:  sort($arr);
来源：http://hz.jiagoushi.top/gtnnngazjl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtvvhdypsy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hysaishi.cn/gtrdtqejpo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtxeulvlgr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtxaydfwoj.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtzktdgjzv.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtfcssewbl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtlxygpsvb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tian-w.cn/gtbhzyalbx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtzkcgtsgc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gthbpjdyio.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtocuzjmua.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gthlwzfvtu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtsvwjvuht.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtgrvddpgb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ivvv.top/gtbwxkltlq.html

[D11] 反转数组
来源：http://hz.nwbrower.top/gtriijhnrk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.316326.xyz/gtqfrumfvo.html

PHP:  array_reverse($arr);
来源：http://hz.redwolf501.top/gtbjhyiqth.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gttsldyjwt.html

TS:   [...arr].reverse();
来源：http://hz.cdnleiting.top/gtaisohatb.html

Java: Collections.reverse(list);
来源：http://hz.ybcxt.top/gtfivcteee.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtjogfryjd.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtnkindkna.html

C#:   list.Reverse();
来源：http://hz.vqdsnc.cn/gtkbxlrnzp.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtqyytxgur.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtolpoqova.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtvopgaqrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtkxdijomk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtudtwmkfu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gogol.net.cn/gtvejcdbnh.html

Go:   slices.Index(arr, x)
来源：http://hz.yj202588.top/gtrbijzciv.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtbmcemcjk.html

C#:   list.IndexOf(x);
来源：http://hz.ybcxt.top/gtnozkslgy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gtutxiwpqc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuetiantiany.cn/gtupwthkrl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yvedp.cn/gtywotoyfa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtoukppzbf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtbgioavoo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtliubzdcu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtrireijxa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aibaodan.cn/gttdluqnbf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtlbnlvnkv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fzhhl.top/gtslnhaddc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhoulong.xyz/gtsfnvfrht.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sysykeji.top/gtgjkgqfrh.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtendjsiiv.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtnzlihfgl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ppjwa.cn/gtpphxlmjh.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtaslnrdci.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xinyue.icu/gtxxwdjfax.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hammf.cn/gthdxwuydz.html

[D15] 去重
来源：http://hz.ydzc1.top/gtyefgvjsj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtnchkromo.html

PHP:  array_unique($arr);
来源：http://hz.cucudq.cn/gtziozlmix.html

JS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtmidrwwgd.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtdaltprjv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtxcfdzebb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xinyue.icu/gtzncaczwq.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtcfigikyg.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtjmlhbjwr.html

[D16] 求和与平均值
来源：http://hz.hfpthk.cn/gtnyvvqahk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daria6918.cn/gticksokng.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sxryk.cn/gtfmtuzlwb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtgkdfdbll.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtlphfgoni.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtewijkzni.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtewynzqjw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gttqiqjvca.html

C#:   list.Sum();  list.Average()
来源：http://hz.hammf.cn/gtvtijdkvl.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtkzowrasv.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtfcunfiwl.html

PHP:  max($arr);  min($arr);
来源：http://hz.gotoacloud.top/gtdnnpfkft.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gtzekvpnuv.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtdxkafoda.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtoxpeghxh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtpyesbigj.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtvbsczazq.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtmiykofpp.html

[D18] 扁平化嵌套数组
来源：http://hz.zdqjudy.top/gtqcasvfjp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.0kj1m.cn/gterlnfbjn.html

PHP:  array_merge(...$nested);
来源：http://hz.shzxlz.cn/gtygzlxawf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnqzz.top/gtqgeytgka.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtgmgeoqxa.html


<!-- 参考信息 -->