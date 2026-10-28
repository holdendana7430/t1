代发 wailian999

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtllvtbrym.html

Ruby: a && b || !c
来源：http://hz.tianlin.xyz/gtdocccgdf.html

C#:   a && b || !c
来源：http://hz.hnxiangtu.top/gttuojabmb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnxiangtu.top/gtsoyyqcam.html

Py:   if not data: return
来源：http://hz.hnxiangtu.top/gtkknncrqk.html

PHP:  if (!$data) { return; }
来源：http://hz.daria6918.cn/gttfxbwqjv.html

JS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtkyonfuti.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gtsxmcclrl.html

Java: if (data == null) return;
来源：http://hz.zycfv.cn/gtrwjecqzj.html

Go:   if data == nil { return }
来源：http://hz.yueranfly.top/gtliqcjnaf.html

Ruby: return if data.nil?
来源：http://hz.yongpay.top/gtlywvvssc.html

C#:   if (data == null) return;
来源：http://hz.gogol.net.cn/gttjxnfiiu.html

================================================================================
来源：http://hz.shuidangran.top/gtlgqhsybv.html

C. 函数与作用域
来源：http://hz.hywenlv.cn/gtsvdnyopf.html

================================================================================
来源：http://hz.wangdashe.top/gtzqsectga.html

[C01] 定义函数
来源：http://hz.nwbrower.top/gtlhhcnyax.html

Py:   def add(a, b): return a + b
来源：http://hz.yueranfly.top/gtbetpovfl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtrgqidoyi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtmblbkahp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtacsaquda.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gttrqribmu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtjjpijegv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gtamsfvdaz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtikqgpqxu.html

[C02] 默认参数
来源：http://hz.hammf.cn/gtftdcgulp.html

Py:   def greet(name="World"): return name
来源：http://hz.xuanzx.com/gteoicpmkc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgufenzy.top/gtdlhsfvlp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.snrcjt.cn/gthjexjbjr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtlmnuxqjj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nwbrower.top/gtsqomdpsp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jiagoushi.top/gtkixxjnke.html

Ruby: def greet(name = "World") = name
来源：http://hz.yj20258888.top/gtyrbrvoex.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ydzc1.top/gtxdnqewny.html

[C03] 可变参数
来源：http://hz.guowangkeji.top/gtennzcpev.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtpisnecnm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gtedsmawhg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtyruqawuy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtqjdlrhjj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yueranfly.top/gtdqtfzztk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.9152youxi.cn/gtydndntyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj202588.top/gtymdyjkep.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tanke756.top/gtawhaellr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fzhhl.top/gtepxjomim.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yonumen.top/gtvzzdgpif.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnxiangtu.top/gtqluqjjqq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtqzfljgqs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtmefdfkyb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tanke756.top/gteuhpfxie.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnxiangtu.top/gtudvilhnu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtrritkzoa.html

C#:   f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtvmcqermx.html

[C05] 返回多个值
来源：http://hz.shanyushiyangtech.top/gtaidjzork.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtkycuboqn.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtxdqrjesa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hongshengwenyu.top/gtjhvkxcem.html

TS:   return { a, b };
来源：http://hz.sysykeji.top/gtgqbeiean.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtilcedzyd.html

Go:   return a, b
来源：http://hz.daria6918.cn/gtlklpglqs.html

Ruby: return a, b
来源：http://hz.fzhhl.top/gtewzackbo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtlcvrmsef.html

[C06] 匿名函数 / lambda
来源：http://hz.daria6918.cn/gthicaqbbg.html

Py:   square = lambda x: x * x
来源：http://hz.havefunace.top/gtrusoxduu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.meibo888.top/gtegbxtyvl.html

JS:   const square = x => x * x;
来源：http://hz.svipenyu.cn/gtubcgxvht.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhijiandao.cn/gttuloicsr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtdcmxvbec.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gtotupgpez.html

Ruby: square = ->(x) { x * x }
来源：http://hz.daxiang520.top/gtafbhiegb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aibaodan.cn/gtduxykmyk.html

[C07] 把函数作为参数传入
来源：http://hz.zhijiandao.cn/gtdmgnxmae.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenjidiqi.icu/gtgoayrmuf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.daria6918.cn/gtylddniao.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gaohongyu789.top/gtunocnzwc.html

TS:   arr.map(String)
来源：http://hz.quarkkingdee.top/gtecpdeotg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guowangkeji.top/gtjqtyxbak.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yueranfly.top/gtobpzsoey.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhengqikj.top/gtfolqmzcd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xuetiantiany.cn/gtgvmobyhm.html

[C08] 闭包
来源：http://hz.birdmap.top/gtbvmpnpgb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aibaodan.cn/gtmjrzqmva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydjk.org.cn/gtvuaojpxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtxdjmqxnt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtrhetbkgc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daria6918.cn/gthhftxllu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gttztheskd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jiagoushi.top/gtuqnwzups.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtcpypavtv.html

[C09] 递归
来源：http://hz.smart0.xyz/gtttlsevfu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gtoynqahoe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ppjwa.cn/gtlixkaenw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtlfwbyetl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtweaevygy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pengpengdd.cyou/gtncpimbtm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtyuupffab.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aizwys.cn/gtzabomvxy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ybcxt.top/gtkopvwkoy.html

[C10] 变量作用域
来源：http://hz.bjfxy.top/gtryimolsq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gthpmhxrsl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tian-w.cn/gtavebytys.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtarjmvnxr.html

TS:   同 JS
来源：http://hz.zhaomingkeji.xyz/gtuoyowhxe.html

Java: 方法内为块级作用域
来源：http://hz.zhiwuduotai.top/gtrsldlbie.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtlxqzykna.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtrqkodfmz.html

C#:   块级作用域
来源：http://hz.zhixingplan.top/gtmccdvywn.html

[C11] 模块导入与导出
来源：http://hz.guowangkeji.top/gtggnmbhuq.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtfyshvmon.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydjk.org.cn/gtfqvwqvcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.snrcjt.cn/gtopgnxpqr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.wangdashe.top/gtfnmfrots.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtmnrdjosh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gttqeaotvq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gtoziflgsx.html

C#:   using System.Text;
来源：http://hz.yj202588.top/gtpazbizqd.html

[C12] 立即执行函数 IIFE
来源：http://hz.shanyushiyangtech.top/gtwzkrnegs.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtddxfnxwk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fengsongda.top/gthmtvaoaf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtdlapiqep.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtggpnozjl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fzhhl.top/gtrekkayof.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zdqjudy.top/gtxvtgdpjm.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtpxbqkjkj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cashguo.top/gtkfugemxy.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhoulong.xyz/gtixowrnqc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sxryk.cn/gtmdvuvysb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtavxhgvvq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtpwpwsrth.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtropdebvq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtqwkxhcqu.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtsmupkbkr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtlvljbvvh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxinkj.top/gtrbathodl.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtrhgmtfyl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tanke756.top/gtpdrldfrb.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtsyxclbyx.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtgxpxqbte.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtmbxdkjqf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtfxcqmmww.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.birdmap.top/gtgjqjfltr.html

Ruby: # 无泛型
来源：http://hz.smart0.xyz/gtbwkwydww.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtezdevypz.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gttgvfbuet.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cucudq.cn/gtygbxdppu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tian-w.cn/gtvvhdlslc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtwegztuet.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtnfgmggbk.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtknavtuut.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtbvfqusnz.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtfdfcuqxa.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtkytxvgot.html

[C16] 函数 / 方法重载
来源：http://hz.shuidangran.top/gtvvjdbfyf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtcobkmmbk.html

PHP:  // 无重载
来源：http://hz.ybcxt.top/gtoykpikug.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gttylksxme.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gtiwxnzbfs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jiagoushi.top/gtsmmidcpv.html

Go:   // 无重载：用不同函数名
来源：http://hz.yueranfly.top/gtjihwzbdi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gzhubu.top/gtfirktwgs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.havefunace.top/gtfkdtlcgr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwlbsfrma.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtebegpcpb.html

================================================================================
来源：http://hz.cdnleiting.top/gtsjxcjykj.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtbxhwrriw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhijiandao.cn/gtgmthtihd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pycfn.com/gtinxiziys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenzaomai.com/gthgugypjs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xinyue.icu/gtcysxavgs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gtqmllvlzb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ppjwa.cn/gtigzogynv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtvfacbgwg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydzc1.top/gtidtikcke.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gtbdtpeueu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daxiang520.top/gtqoxxhrnp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtajjuzixa.html

JS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gttlrimrzw.html

TS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtmirhxlra.html

Java: list.add(4);
来源：http://hz.jianghu66.top/gttlsvjbjv.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtkogziswo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtqmecovdo.html

C#:   list.Add(4);
来源：http://hz.nanxuanxn.top/gtjrlighag.html

[D03] 在指定位置插入元素
来源：http://hz.zdqjudy.top/gtjlfepdrr.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtxmndwizp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yongpay.top/gthfjdnijs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.pycfn.com/gtrnwlnsrp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtlkasbtie.html

Java: list.add(0, 0);
来源：http://hz.yueranfly.top/gtioxsxwbl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtlosuskhf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtraglsgzm.html

C#:   list.Insert(0, 0);
来源：http://hz.ydzc1.top/gtayvgzzyg.html

[D04] 删除元素
来源：http://hz.tian-w.cn/gtpisqwycp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gtlukomiqa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sxryk.cn/gtpzwlxcvg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.snrcjt.cn/gtmswzkptz.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtbaisqlim.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenjidiqi.icu/gtkrzjmkav.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gotoacloud.top/gtrcjwrxzm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xylfe.cn/gtcijnjhfs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.meibo888.top/gtwynrqjxl.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gtbcmhpyxq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtaadvgnfc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nwbrower.top/gtsckyymmk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yangfankeji.com/gtmrstcxxr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtbvlfdjmv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtxjtkixkf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sxryk.cn/gtwlgrvhow.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtwmcljgjn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.snrcjt.cn/gtqegdcxcn.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtsrzbjkyn.html

Py:   len(arr)
来源：http://hz.316326.xyz/gtlcwhmwbr.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtoevpnfin.html

JS:   arr.length
来源：http://hz.meibo888.top/gtmjuwsrkb.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtmguncufp.html

Java: list.size();
来源：http://hz.xuetiantiany.cn/gttqpxnzrs.html

Go:   len(arr)
来源：http://hz.yj20258888.top/gtawzpqxki.html

Ruby: arr.length; arr.size
来源：http://hz.hnqzz.top/gtnaxzzdfo.html

C#:   list.Count;
来源：http://hz.ehwqpu.com/gtyazjeutg.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtkpoxssty.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gteoqjnehi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtdymifdtb.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtormtjead.html

TS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtwqeoqdej.html

Java: list.subList(1, 4);
来源：http://hz.hfpthk.cn/gtdeqfjful.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtohjdtpth.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtdimdjukq.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtmbxoxwed.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtogllovav.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtvcgohsli.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtarmosaet.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtkcehdmpm.html

TS:   [...a, ...b];
来源：http://hz.aizwys.cn/gtbqlvhmtv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtvxucblwz.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gtlpyoidlu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtyfsvjcxx.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtwqbrpbuc.html

[D09] 排序（升序）
来源：http://hz.tianlin.xyz/gtzdkksbvm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtqrghjqsh.html

PHP:  sort($arr);
来源：http://hz.ehwqpu.com/gtixmrsbcc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daria6918.cn/gtvmvnygtt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhiwuduotai.top/gtavclcrgu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guannengcc.top/gtsdqakqkg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtdjtajrqs.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtabgfxgtm.html

C#:   list.Sort();
来源：http://hz.jinghuilouyu.cn/gtbrggjupt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj20258888.top/gtabfkyruh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuanzx.com/gtvrujvrth.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gzhubu.top/gtyavjnfzp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtoswjrlhi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtdgcfieoq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gogol.net.cn/gtjdejiiie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangkeji.top/gtfcybdjxw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gtugsbpnkw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.bjfxy.top/gtjdgkjcwu.html

[D11] 反转数组
来源：http://hz.jinqigufen.top/gtuoszxlfs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tanke756.top/gtqeaaxguc.html

PHP:  array_reverse($arr);
来源：http://hz.sysykeji.top/gtsrgfuddk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ywan-chungtsiang.top/gtghfjtwzl.html

TS:   [...arr].reverse();
来源：http://hz.yuxming.cn/gtdvmfmcqi.html

Java: Collections.reverse(list);
来源：http://hz.yj20258.top/gtgkyyxuet.html

Go:   slices.Reverse(arr)
来源：http://hz.guowangkeji.top/gtdcacjlfk.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gtkvtnpfub.html

C#:   list.Reverse();
来源：http://hz.yangfankeji.com/gtzthfmsxc.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtnivsrmnz.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtltqijuvt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtfkahhjvx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtkibqqcjs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtpzpuwthq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtkjxhxbft.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gtqalenesv.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gtaiycimba.html

C#:   list.IndexOf(x);
来源：http://hz.wangdashe.top/gtnfbeneje.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtlhivmmvv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgfzy.top/gthgqqgjzt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtonvdjekg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258888.top/gtvtlypjho.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtrhwdthkm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtvnffofgp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dashuyun.cn/gtgytahxta.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yangfankeji.com/gtqpjgylnn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtsjcyysnz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tanke756.top/gtrhtvhhvb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtlwrlswbk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtoyacerea.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtrwmndenn.html

TS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtstbwsnog.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtcjwxzhwm.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtdyxqpwdw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.birdmap.top/gttpdpmhvf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guowangkeji.top/gtkyrrobvn.html

[D15] 去重
来源：http://hz.zhaomingkeji.xyz/gtioxmeldj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gteqizixtd.html

PHP:  array_unique($arr);
来源：http://hz.zhiwuduotai.top/gtsfyemfow.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtyoczvybw.html

TS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gtqjvqqjwr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hammf.cn/gtsdnekawa.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.kuanghao11.cn/gtfwqabzvf.html

Ruby: arr.uniq
来源：http://hz.316326.xyz/gtudcuqdhg.html

C#:   list.Distinct().ToList()
来源：http://hz.zhiwuduotai.top/gthcqdvzmx.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtjccylink.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gtyqarnfic.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtwstajaqj.html


<!-- 参考信息 -->