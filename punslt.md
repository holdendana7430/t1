代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.yj20258888.top/gtposjdgzl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gaohongyu789.top/gtudniwkme.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtaiklctet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtuhrizhry.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gttanciptf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhoulong.xyz/gtvhmwzojt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.svipenyu.cn/gtjhwnvgod.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtrsqhlyla.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtgdjpkcrg.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtylipvnrj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shangyingyoupin.top/gtuauaanqe.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuxming.cn/gtucrgdwhf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hammf.cn/gtdsgxxwgg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtijbotmxk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangtech.top/gtxetfeziw.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtmyjykqco.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigfzy.top/gtwquzxhzh.html

[C03] 可变参数
来源：http://hz.dashuyun.cn/gtmxsrmzrh.html

Py:   def total(*args): return sum(args)
来源：http://hz.yangfankeji.com/gtlzasefes.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.0kj1m.cn/gtjbapaaer.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhaomingkeji.xyz/gtsuodgqay.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gtoejggepp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gzhubu.top/gtmhqgkxup.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtqizadsvq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jiagoushi.top/gtrzpaqnui.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gtbtkbsrel.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj20258.top/gtxamwtyuo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtyrhnvwjr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.0kj1m.cn/gtsweadsqh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtjgclsgas.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtbdercqwv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gthtdpycbn.html

Go:   // 无：用配置结构体参数
来源：http://hz.xziqi.cn/gtprmaoyyn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtdbhjvbou.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtcxignyrw.html

[C05] 返回多个值
来源：http://hz.zhiwuduotai.top/gthkmosxpa.html

Py:   return a, b
来源：http://hz.smart0.xyz/gtqutlddzj.html

PHP:  return [$a, $b];
来源：http://hz.wangshuangyany.cn/gtfealdaoo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yvedp.cn/gtlyqlossr.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gtzsuniwph.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.52xcode.cn/gtmposkazc.html

Go:   return a, b
来源：http://hz.ehwqpu.com/gtmhyswuly.html

Ruby: return a, b
来源：http://hz.cheryme.top/gtowackeru.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nanxinkj.top/gtsibkraad.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtmijdvehi.html

Py:   square = lambda x: x * x
来源：http://hz.cdnleiting.top/gtrcxwmzek.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtsstcfnfu.html

JS:   const square = x => x * x;
来源：http://hz.0kj1m.cn/gtzhekreqh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtaescrhkw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gtrakpjhkx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258.top/gtgmbjuqgd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.9152youxi.cn/gtwmfmrkbm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cucudq.cn/gtjecxldhq.html

[C07] 把函数作为参数传入
来源：http://hz.yuxming.cn/gtsueogezh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhixingplan.top/gtxvesaobo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.mhx1999.top/gtzkfqydna.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhiwuduotai.top/gtecwdqlqj.html

TS:   arr.map(String)
来源：http://hz.yangfankeji.com/gtxnesaral.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ehwqpu.com/gtjnixmrzk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnxiangtu.top/gtbcrdkbvm.html

Ruby: arr.map(&:upcase)
来源：http://hz.cheryme.top/gtizgampgq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.andypj.xyz/gtvdgzhxml.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gtnjzrjaok.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj202588.top/gtpomqbgal.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tianlin.xyz/gthwqhepbh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtipmzyuow.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtzfsnzdfx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sweek.top/gtcbxjuxtc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gtxjbgucpn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.havefunace.top/gtxmqbqbmr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtqwnpnhzk.html

[C09] 递归
来源：http://hz.nanxinkj.top/gtdodblvkg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aizwys.cn/gtbbpedtiw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jlsjyb.cn/gtdtpelgzy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhongyouzk.top/gtpyxqtvxx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.9152youxi.cn/gtitxrwrkt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daria6918.cn/gtkwqzuklg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hammf.cn/gtcsmjtthv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtcfpeqykq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sweek.top/gtrgeqiulm.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtsjbgehez.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtdlisgltp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.andypj.xyz/gtyjmjhukh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhiwuduotai.top/gtcnbosonv.html

TS:   同 JS
来源：http://hz.sysykeji.top/gtjoqixrns.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gttbcjdweg.html

Go:   花括号块级作用域
来源：http://hz.nanxinkj.top/gtcuvgpqex.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dashuyun.cn/gtkhbuadps.html

C#:   块级作用域
来源：http://hz.ppjwa.cn/gtuzwoanum.html

[C11] 模块导入与导出
来源：http://hz.chenzaomai.com/gtwsjxhmsx.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtgbggquox.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.c1oappe.top/gtbuhjumdd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sxryk.cn/gtnkkdhdub.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gtymktpuvf.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtnkzojdfp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gtwfbenxnh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtatqcdnvc.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtygsncupb.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtbsaedqok.html

Py:   (lambda: print("run"))()
来源：http://hz.ydjk.org.cn/gtfudjcwww.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtzwwulism.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtrpiskrbt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtznrcxcra.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhongyouzk.top/gtrymhdhqt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gtkpswacig.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydjk.org.cn/gtfheyqcib.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtopfuxcup.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtjhttstju.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtpmrtozfv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtllafyevh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtkldjcbse.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtviljpdst.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtjfsqzesn.html

Go:   func add(a, b int) int
来源：http://hz.andypj.xyz/gthnieccoe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigufen.top/gtctjjilvc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zycfv.cn/gtzfjhhfbn.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtizjqrmgq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sysykeji.top/gtiwjqqoeo.html

PHP:  // 无泛型
来源：http://hz.aibaodan.cn/gtdaspyche.html

JS:   // 无泛型
来源：http://hz.jlsjyb.cn/gtwpeimjnd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nwbrower.top/gtrpslnbcp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.bjfxy.top/gtcrfibuau.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hywenlv.cn/gtpikaukbh.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtixboyysb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtzsstlvll.html

[C15] 解构 / 展开参数
来源：http://hz.0kj1m.cn/gtwedrtuyg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hysaishi.cn/gtjvucdwdh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtxgjvoyzy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gttachabfb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgfzy.top/gtqyrzjqxs.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtzalimpbt.html

Go:   // 无解构
来源：http://hz.pycfn.com/gtkawsurlu.html

Ruby: a, b = pair
来源：http://hz.chenlongwang.top/gteapcgqfl.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtjxvibtso.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtlmsbnoul.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gtukngdawr.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtrbhpfrbk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtldgtymic.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fengsongda.top/gtjkzzehvk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuanzhike.top/gtddqpahmv.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtzikmtuia.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtwdeqcrga.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ybcxt.top/gtufqntbxt.html

================================================================================
来源：http://hz.yj20258888.top/gtrybfaqzx.html

D. 数组 / 列表 / 集合
来源：http://hz.tian-w.cn/gtbkvqmeea.html

================================================================================
来源：http://hz.tian-w.cn/gtptaltorj.html

[D01] 创建数组 / 列表
来源：http://hz.gaohongyu789.top/gtckhqgnsi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gthbkzqkce.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtqybwyyir.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtnkqvhjyp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gthimpsvdp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigufen.top/gtytkjsgon.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtasppnmbe.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtcwevtfsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jyoumei.cn/gtmqjqwgea.html

[D02] 追加元素到末尾
来源：http://hz.chenzaomai.com/gthuysmaey.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtfuiacigu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtzutnojsp.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtnvqbgnmb.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtsqwwuszc.html

Java: list.add(4);
来源：http://hz.bjfxy.top/gtucgphvuf.html

Go:   arr = append(arr, 4)
来源：http://hz.xinyue.icu/gtpsiphggt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dashuyun.cn/gtqsdqpgcn.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtqkhvgzkt.html

[D03] 在指定位置插入元素
来源：http://hz.aibaodan.cn/gttuubrpzu.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtpklhrwsb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtgautzhrb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258888.top/gtzssfcbjx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhongyouzk.top/gtugecaswm.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gtjuddbixn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gtahmqsfch.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cqqwz.cn/gtftptpfva.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtzzgupinz.html

[D04] 删除元素
来源：http://hz.chenzaomai.com/gteycrsmiu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.quarkkingdee.top/gtlhzkvpqc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtfqnpsbga.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtfapfmezt.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtdgkivlci.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj202588.top/gtuhdqpbmu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.52xcode.cn/gtklgrgdpl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtdouqkanp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tianlin.xyz/gtglujzyln.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gteytugzlt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtjwnwrolz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgfzy.top/gtwtvpaomj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yvedp.cn/gtvhmiaury.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.andypj.xyz/gtwlsaajmc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ivvv.top/gtyapbcoit.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtctljevxd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gttygtflak.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yonumen.top/gtjsohgzft.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtgncxlduz.html

Py:   len(arr)
来源：http://hz.tian-w.cn/gtxcahlloq.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gtmurlefgm.html

JS:   arr.length
来源：http://hz.yonumen.top/gtdfzqrbna.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gttpblktyw.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtaoevopby.html

Go:   len(arr)
来源：http://hz.xziqi.cn/gtojlsufuh.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtebakdyyo.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtjxnywjew.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gtvlbyabhi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.vqdsnc.cn/gtceynyqvb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtpglbwggg.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtqrdvgswq.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtxcuisihy.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gteijtokch.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtsrylsgvs.html

Ruby: arr[1, 3]
来源：http://hz.zdqjudy.top/gtrrucikhg.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtklzbhvhc.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangkeji.top/gtbjungxyu.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtrzohdpfp.html

PHP:  array_merge($a, $b);
来源：http://hz.daria6918.cn/gtsmasffqq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gtyceictvh.html

TS:   [...a, ...b];
来源：http://hz.tian-w.cn/gtgdvfyenn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gthgzarsws.html

Go:   append(a, b...)
来源：http://hz.pycfn.com/gtlhbdqgzq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tianlin.xyz/gtczrzioif.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gtlclgxiwt.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtmuzfamnm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtdawvxubz.html

PHP:  sort($arr);
来源：http://hz.jinghuilouyu.cn/gtmlgsqksx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtvkbhiavu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shangyingyoupin.top/gtxxfvuyda.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zycfv.cn/gtaltljuqz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.redwolf501.top/gtvgrzmgpt.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtkfqavdns.html

C#:   list.Sort();
来源：http://hz.daxiang520.top/gtlzwnqzcr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hnxiangtu.top/gtwghxyiit.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhongyouzk.top/gtucikuboq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtounopwxp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtsufnwluj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtpztgpoyu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cashguo.top/gtzoiapinz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aizwys.cn/gtcelwimfa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.havefunace.top/gtwtbofuqf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sufxvd.cn/gtbzrsqlmj.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gtcezttqkb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sysykeji.top/gtgiggeomc.html

PHP:  array_reverse($arr);
来源：http://hz.pycfn.com/gtdakjexwu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aibaodan.cn/gtbsgsqxmx.html

TS:   [...arr].reverse();
来源：http://hz.jinqigfzy.top/gthkjbybrs.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtjmsxascr.html

Go:   slices.Reverse(arr)
来源：http://hz.zhijiandao.cn/gtmohnvmmw.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gthzjqjvqa.html

C#:   list.Reverse();
来源：http://hz.tianlin.xyz/gtrpdjyado.html

[D12] 查找元素下标
来源：http://hz.xuetiantiany.cn/gtduuccedw.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtvlaslgva.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtktfgburl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtoxctjokr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtvygptroe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.haohaochexian.top/gtczcmjkaj.html

Go:   slices.Index(arr, x)
来源：http://hz.daxiang520.top/gtvpskalcq.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtundhbgdr.html

C#:   list.IndexOf(x);
来源：http://hz.daxiang520.top/gtckggqvxa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ppjwa.cn/gtuqukandj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtvoaemeic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtnsyprtvc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gthkrpfgmw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtjbepccyf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtzztzdqwu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangdashe.top/gtvkkrltfn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtvhpjskrq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtgogimdop.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xingfuxueyuan.xyz/gtlpcopyln.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sweek.top/gtofcnhenn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgufenzy.top/gtbkzpumzi.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtigotepps.html

TS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtycmbhndy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtvxnzdxyf.html

Go:   // 手写循环
来源：http://hz.zhiwuduotai.top/gtwvqojwzo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yueranfly.top/gtvatkxpyf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cdnleiting.top/gtadvparho.html

[D15] 去重
来源：http://hz.fengsongda.top/gtgamyvskq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtukhhjmyk.html

PHP:  array_unique($arr);
来源：http://hz.nanxinkj.top/gtajztljgz.html

JS:   [...new Set(arr)]
来源：http://hz.yangfankeji.com/gtztwfanxh.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtlhpcytpz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuanzhike.top/gtencekcgz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtarfclboq.html

Ruby: arr.uniq
来源：http://hz.shuidangran.top/gtlfahpeml.html

C#:   list.Distinct().ToList()
来源：http://hz.daxiang520.top/gtvuwfasoj.html

[D16] 求和与平均值
来源：http://hz.andypj.xyz/gtqitrlokz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnxiangtu.top/gtdzjwscbw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tian-w.cn/gtrpghekcs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gtikxpstfy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtkvonpcwa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tian-w.cn/gttkiymfei.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gtdlzayyjw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtqominmbr.html

C#:   list.Sum();  list.Average()
来源：http://hz.nwbrower.top/gtohbpzmox.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtbpovmnbh.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangkeji.top/gtgpqozcjd.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gtbzrfcnbw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtmozjbiml.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gttygrtsfk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gtqflbkuvd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydjk.org.cn/gtrxnvgvmf.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gtxkmjrzzn.html

C#:   list.Max();  list.Min()
来源：http://hz.jiagoushi.top/gtkhpbpgjn.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gtjcrhiais.html


<!-- 参考信息 -->