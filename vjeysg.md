代发 wailian999

Py:   if not data: return
来源：http://hz.ydzc1.top/gtuhijjxwd.html

PHP:  if (!$data) { return; }
来源：http://hz.cheryme.top/gtxzaenubx.html

JS:   if (!data) return;
来源：http://hz.nwbrower.top/gtdzgyfqcn.html

TS:   if (!data) return;
来源：http://hz.smart0.xyz/gtfucvsmqg.html

Java: if (data == null) return;
来源：http://hz.c1oappe.top/gtvqiiukgo.html

Go:   if data == nil { return }
来源：http://hz.jqgufenzy.top/gtarekoxgw.html

Ruby: return if data.nil?
来源：http://hz.iojbl.cn/gtktqzkuyz.html

C#:   if (data == null) return;
来源：http://hz.jiagoushi.top/gtxowdequx.html

================================================================================
来源：http://hz.ehwqpu.com/gtkogxddes.html

C. 函数与作用域
来源：http://hz.nanxinkj.top/gtzejojace.html

================================================================================
来源：http://hz.yongpay.top/gtcfrjhehz.html

[C01] 定义函数
来源：http://hz.shzxlz.cn/gtaphpdszk.html

Py:   def add(a, b): return a + b
来源：http://hz.cdnleiting.top/gtazykzuxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gthsptivqs.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtkspxqdqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtfvcxywgc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtxaihymgj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnxiangtu.top/gtldiquolu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.andypj.xyz/gtgnvlivsj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtmpfdhgul.html

[C02] 默认参数
来源：http://hz.pengpengdd.cyou/gtpogunqfe.html

Py:   def greet(name="World"): return name
来源：http://hz.jlsjyb.cn/gtpsnxqtsj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guowangkeji.top/gtyzkfgcmp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.daxiang520.top/gtloxuyncw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gtvuhmdekw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtrkepztvk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gtnjarlzrw.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtfsxusymc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ivvv.top/gtinblxjuq.html

[C03] 可变参数
来源：http://hz.tanke756.top/gtvvjlktve.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtrymgsgrv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258.top/gtxeocracj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtrbljuskf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtglmvkves.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtgdujyjye.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gotoacloud.top/gttahfuplc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gtrxnonyht.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtrbqfkkdr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtyqyvzsuy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.mhx1999.top/gtaodlkysj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cheryme.top/gttuhdbcwh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtoccnetzz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.birdmap.top/gtodxbhnwy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pengpengdd.cyou/gtgkxxbwuy.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgufenzy.top/gtkstorkkb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtifudoedk.html

C#:   f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtuohjzneh.html

[C05] 返回多个值
来源：http://hz.xylfe.cn/gtnwedfqkp.html

Py:   return a, b
来源：http://hz.wangdashe.top/gtfvgxctij.html

PHP:  return [$a, $b];
来源：http://hz.jlsjyb.cn/gtlwxqpzqb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.0kj1m.cn/gtsgymxwsf.html

TS:   return { a, b };
来源：http://hz.cheryme.top/gtrqayqujk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtyzsdoefi.html

Go:   return a, b
来源：http://hz.svipenyu.cn/gtfxqkprir.html

Ruby: return a, b
来源：http://hz.xziqi.cn/gtrkerpien.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ppjwa.cn/gtvgwcszns.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gthsdyajne.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gtjlmfujca.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgfzy.top/gtjqvkihbu.html

JS:   const square = x => x * x;
来源：http://hz.havefunace.top/gtztzwzfpi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zdqjudy.top/gtaqejylmg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gtrrtcaaww.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ivvv.top/gtydnkhyhk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cucudq.cn/gtrqkdipzn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtvwqkssce.html

[C07] 把函数作为参数传入
来源：http://hz.0kj1m.cn/gtuoxrbhab.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhongyouzk.top/gtyjwwyazk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.snrcjt.cn/gtrdfuhxwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tian-w.cn/gtyvmcmqzh.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gtmvhbcuzf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sxryk.cn/gtekqwzuop.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtodellmee.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtlsafisub.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.52xcode.cn/gtsuaoylju.html

[C08] 闭包
来源：http://hz.fengsongda.top/gtpqairszt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aizwys.cn/gtnikfqhlq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.kuanghao11.cn/gtkeutaxve.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shangyingyoupin.top/gtmqaqxkjj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtwcpymwyd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhiwuduotai.top/gtgblecmwo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shuidangran.top/gtntenvsjm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtvtldzfdp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtmyugrcjl.html

[C09] 递归
来源：http://hz.guannengcc.top/gtvlpxzpto.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cqqwz.cn/gtgabixmwk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtsoganuri.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtbcuvcysg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtrcbqhwqv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sufxvd.cn/gtbheypfia.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydzc1.top/gtibrtkutl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gtnumexyop.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigfzy.top/gtleaiixdu.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtzyavzloh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenjidiqi.icu/gtzoyqwikr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gtpoaspeux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sweek.top/gtyjxnfiol.html

TS:   同 JS
来源：http://hz.c1oappe.top/gtqipsbydy.html

Java: 方法内为块级作用域
来源：http://hz.sysykeji.top/gtvnjdocyl.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtyjfhadea.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.haohaochexian.top/gtjedicsjj.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtqfflmdqd.html

[C11] 模块导入与导出
来源：http://hz.52xcode.cn/gtnzocihma.html

Py:   from module import func
来源：http://hz.yj202588.top/gtvpjmjyde.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hongshengwenyu.top/gtngcwgamd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenzaomai.com/gtemmdggfq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuxming.cn/gtedabmeiq.html

Java: import java.util.List;
来源：http://hz.zhijiandao.cn/gtmzljwrir.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenzaomai.com/gtywatmawo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtkijoyrqm.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtqoaxvdos.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtsyzgyorm.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gtjtbfmobn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gtxmzfpjfl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtthhcftpd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtoefjmjqh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gtsspsbprx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtwtngczzw.html

Ruby: -> { puts "run" }.call
来源：http://hz.yuanzhike.top/gthxdwsenv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtmuvzrhno.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtxawoyghw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yanxiufei.cn/gtnmqbzkat.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtfwbtgzgf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ydjk.org.cn/gtgjgmxrvo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtpgmkogra.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtzqdmmbsh.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtstzluawf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtqnbgtpwj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jyoumei.cn/gtywjuphbn.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gtjxougwmw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtctzsqdge.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtrtggopgo.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtmxzvvvcb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtzitolabe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtqoyfrgwo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenlongwang.top/gtnzeyidgi.html

Ruby: # 无泛型
来源：http://hz.gaohongyu789.top/gtihofenfy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gttgyufwqn.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtbdzfjudu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.c1oappe.top/gtzurgezcg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.redwolf501.top/gtgmymargx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtdfnylait.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sxryk.cn/gtamhifphp.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtmrrqwgaq.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gthvjdumtj.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gtgoadqkyl.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258.top/gtglasgshx.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gtnwdlyvgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtqrwemupo.html

PHP:  // 无重载
来源：http://hz.ydzc1.top/gtspylhsbb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtahbtsfve.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtocvdrpbg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.birdmap.top/gtkpbejbkd.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtolcgmbrb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtodccjfzq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtuifyfpqt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbstkzzzb.html

D. 数组 / 列表 / 集合
来源：http://hz.guannengcc.top/gtcthsywki.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmxvvhcqc.html

[D01] 创建数组 / 列表
来源：http://hz.feifeiyinyue.top/gtmxovfgnz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydjk.org.cn/gtxbtzwqnr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cheryme.top/gtvrxohpxh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gtbyhgkllj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtltewuahy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtkbfuxeae.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtadkjzfeu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gthtuvomsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cucudq.cn/gtelguvjti.html

[D02] 追加元素到末尾
来源：http://hz.shuidangran.top/gtoaihwqhs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangshuangyany.cn/gtrdagcomd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pengpengdd.cyou/gtuwramoow.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtxqewmdcf.html

TS:   arr.push(4);
来源：http://hz.shuidangran.top/gtqnadxjfn.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtljinmdnq.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtzrroslio.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.bjfxy.top/gtxhzxauua.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gtgssuhusg.html

[D03] 在指定位置插入元素
来源：http://hz.cashguo.top/gtkpuycgih.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtbikhdqws.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sweek.top/gtcuwtvltx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.pycfn.com/gtzcuutfvx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fzhhl.top/gtprwdmixt.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtkszuxfom.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtmvoeruea.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangdashe.top/gtsdhwmbbs.html

C#:   list.Insert(0, 0);
来源：http://hz.yuxming.cn/gtgsjrdcdy.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gttteokros.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gthvykipcu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtcwuhzxlk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yonumen.top/gtyltaaqen.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtyfpknmwf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gtyqlystdn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gaohongyu789.top/gtiosarkhd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtwfhsrgyt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgufenzy.top/gtozhhtmuz.html

[D05] 访问与修改元素
来源：http://hz.fzhhl.top/gtgqoueain.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtnfujafwi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cqqwz.cn/gtzryyugpq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yongpay.top/gtpatqzfnm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtilixhhjv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gtgjbporpc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gtkpxzxjsn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtlokaoowc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sysykeji.top/gtkxhvggyc.html

[D06] 数组长度
来源：http://hz.xinyue.icu/gttrqtsixq.html

Py:   len(arr)
来源：http://hz.zhoulong.xyz/gtleopursk.html

PHP:  count($arr);
来源：http://hz.meibo888.top/gtjnzgcmfc.html

JS:   arr.length
来源：http://hz.9152youxi.cn/gtfvnqsyns.html

TS:   arr.length
来源：http://hz.shuidangran.top/gtxupbvwms.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtmesjbdto.html

Go:   len(arr)
来源：http://hz.andypj.xyz/gtezcbbewa.html

Ruby: arr.length; arr.size
来源：http://hz.jlsjyb.cn/gtpmrtqbsf.html

C#:   list.Count;
来源：http://hz.yj202588.top/gtemwqjuhc.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtziuucziw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xinyue.icu/gtkhgwprzk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtvgnhtkds.html

JS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtdkmonmtb.html

TS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtasehshds.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtlspvncrs.html

Go:   arr[1:4]
来源：http://hz.zhoulong.xyz/gtcneqfmva.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtzschtepd.html

C#:   list.GetRange(1, 3);
来源：http://hz.gogol.net.cn/gtnheazsbm.html

[D08] 合并两个数组
来源：http://hz.jqgufenzy.top/gtclwxlxkn.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhijiandao.cn/gtakgfzjru.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtnknxafrp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtjyfupges.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtcbwmbuic.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtmieufzti.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gtqxhwcoar.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gtfzjvsrdx.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtrobhsbru.html

[D09] 排序（升序）
来源：http://hz.redwolf501.top/gtgqixjghw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtaevdqdhu.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtdzoiwxvl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtqcvuyopu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.svipenyu.cn/gtwbmobaqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gzhubu.top/gtigcusmlh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtvjgvbwqr.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtaifwgzwn.html

C#:   list.Sort();
来源：http://hz.xuetiantiany.cn/gtfhihbtuc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cdnleiting.top/gttmadvgca.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtilmsstwr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtrwacfkyu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtfljgbtzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtynvgduyc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.haohaochexian.top/gtymvftjna.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tian-w.cn/gtgxbxfhtj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yueranfly.top/gtusunlsbw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuanzhike.top/gtadvrlczj.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtmpgunulz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtzfiepzsf.html

PHP:  array_reverse($arr);
来源：http://hz.feifeiyinyue.top/gtmpsqcokh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gtovdcrxra.html

TS:   [...arr].reverse();
来源：http://hz.chenjidiqi.icu/gtjnpdnjdj.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtlxbhwqph.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtaspywsaz.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gtgndtgztm.html

C#:   list.Reverse();
来源：http://hz.ehwqpu.com/gtudwxszhl.html

[D12] 查找元素下标
来源：http://hz.chenjidiqi.icu/gtnxoqlfcn.html

Py:   arr.index(x);  x in arr
来源：http://hz.fzhhl.top/gtirtnrdth.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gtzrjduyua.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gttfianxnm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtghgeltzf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtziogwxhh.html

Go:   slices.Index(arr, x)
来源：http://hz.pengpengdd.cyou/gtjpcdhixm.html

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtlabbkgst.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gtxfpzuwqh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yanxiufei.cn/gtivttmsxc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.kuanghao11.cn/gtxdnywwbe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtqbjbhdde.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtotepiwtb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtgbvanqez.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgufenzy.top/gtxspjrfpn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.52xcode.cn/gtuoiuqkfa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuxming.cn/gtsdblkhtn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hywenlv.cn/gtjdayatqd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxuanxn.top/gtdvfljsco.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtebfizkbr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtsavvwndh.html

JS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtcmspnmwq.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtzucgshqd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtldntlydc.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtiqiqyhhe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yueranfly.top/gtoombdmlv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtlqzkksiy.html

[D15] 去重
来源：http://hz.0kj1m.cn/gthkemufqv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtbzcfbxpu.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtkqrjbixa.html

JS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gttdfdhhov.html

TS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtwtwuardl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtplmumgrb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.vqdsnc.cn/gtycgtbrva.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtpudcjnqq.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gttkrphsqv.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtwhkscfni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtsfnncxfw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cqqwz.cn/gtjlqvnatb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gttgjajjav.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtyqetpcre.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangtech.top/gtjsidiydi.html

Go:   // 手写循环累加
来源：http://hz.xuetiantiany.cn/gtbckergim.html


<!-- 参考信息 -->