代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.wangshuangyany.cn/gtbogmssru.html

[C03] 可变参数
来源：http://hz.zhongyouzk.top/gtyvwwlnfv.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtqcuvygws.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aizwys.cn/gtqetewuer.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtmmnewggr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtqmxyykjp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtropkiaft.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ivvv.top/gtjsfnpgsz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydzc1.top/gtbidqtxrf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.meibo888.top/gtksosjmtq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtofbaekvl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgfzy.top/gtaontfxeo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangdashe.top/gtntlaqecl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tanke756.top/gtcloeislu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.smart0.xyz/gthktgavli.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ydzc1.top/gtvlmmdgox.html

Go:   // 无：用配置结构体参数
来源：http://hz.sweek.top/gtrkbrmqkl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtjnjjbwuw.html

C#:   f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtjwnwpdeg.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtckfpzabp.html

Py:   return a, b
来源：http://hz.yj202588.top/gtllcnmqrk.html

PHP:  return [$a, $b];
来源：http://hz.hysaishi.cn/gtydiseusq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtlqnlcbkr.html

TS:   return { a, b };
来源：http://hz.sweek.top/gttgqflwbj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuxming.cn/gtyptofruo.html

Go:   return a, b
来源：http://hz.ybcxt.top/gtwmhcsmfm.html

Ruby: return a, b
来源：http://hz.nanxinkj.top/gtkysczbrb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tian-w.cn/gtfbhoccub.html

[C06] 匿名函数 / lambda
来源：http://hz.zhijiandao.cn/gtxtlmughi.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gtfzqtuced.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinqigfzy.top/gtiysfotcs.html

JS:   const square = x => x * x;
来源：http://hz.yueranfly.top/gtwwazwzwi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtsanfkqyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xuetiantiany.cn/gtxslgebkw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yangfankeji.com/gtwmdejybs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtyvpynryw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuxming.cn/gtujlvtqao.html

[C07] 把函数作为参数传入
来源：http://hz.yangfankeji.com/gthgflkxte.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ivvv.top/gteeadwfbw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtfnxcnyue.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gotoacloud.top/gtrgqsjkra.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtzxikagkm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj202588.top/gtzshlaelp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinyuanbaomall.cn/gtsoxgdvvd.html

Ruby: arr.map(&:upcase)
来源：http://hz.xylfe.cn/gtjjhxztck.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.pengpengdd.cyou/gttbwhdbmg.html

[C08] 闭包
来源：http://hz.andypj.xyz/gtuharwpbh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.redwolf501.top/gtvogxvnuw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhongyouzk.top/gthzefetbx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtxoztrxjk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtkkxftafb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtzdgtqkoa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cashguo.top/gtuenzxgzi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gttrsukwzt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtdydzjokn.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gtzsiwugvq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtubhdmmku.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shzxlz.cn/gteecggqel.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtlpshucyg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtpvtybpln.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtuyplwgrf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.316326.xyz/gtqdvzbxun.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sweek.top/gtvachznkp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dianchejie.cn/gtxkvcgtms.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gtpuckxakj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tianlin.xyz/gtwjnmmbes.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtpazrzevx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daxiang520.top/gtsgfabsbr.html

TS:   同 JS
来源：http://hz.shanyushiyangtech.top/gtrxxwnxvc.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gthsoixlbr.html

Go:   花括号块级作用域
来源：http://hz.nanxuanxn.top/gttdhqfzzz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gttuzdlyjs.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtjszdjraw.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtbnuhbsop.html

Py:   from module import func
来源：http://hz.ydzc1.top/gtopuyqslt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gaohongyu789.top/gtyoqojahh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nwbrower.top/gtslxrmoav.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtmavoudbx.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtshjlpqct.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuanzhike.top/gtsiqnitep.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yueranfly.top/gtwthugkau.html

C#:   using System.Text;
来源：http://hz.shuidangran.top/gtdglpnhym.html

[C12] 立即执行函数 IIFE
来源：http://hz.dianchejie.cn/gtgofvesbu.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtwcuetpzt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgfzy.top/gtvuredwuj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtpxllwmpx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtgquiahwn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtdqyymuyt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtzfngelpt.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnqzz.top/gtjslewnly.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenlongwang.top/gtthttwwnl.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhongyouzk.top/gttumnwckp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gthlpqesje.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gttsjcrkez.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.vqdsnc.cn/gthbufifcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtvqiyywrc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtjjftqvik.html

Go:   func add(a, b int) int
来源：http://hz.ybcxt.top/gtnoribtlt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hysaishi.cn/gteccpenhn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuetiantiany.cn/gtewtwnxwr.html

[C14] 泛型函数
来源：http://hz.andypj.xyz/gtlgstnxzu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gthylxwgmf.html

PHP:  // 无泛型
来源：http://hz.hammf.cn/gtwexcbdul.html

JS:   // 无泛型
来源：http://hz.jinghuilouyu.cn/gtmfwsnoxo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gthvpfoxgz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtqwdxankb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.haohaochexian.top/gtzchubwkj.html

Ruby: # 无泛型
来源：http://hz.yuxming.cn/gtbyjtqwpt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj202588.top/gtlnpqzunx.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangtech.top/gtpwlkkysu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtkzndubdu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xinyue.icu/gtzrppdrpo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtcgiucugn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sweek.top/gtmalbwwtq.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtejuetcyl.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtotdljkge.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gtlhiqwafw.html

C#:   var (a, b) = pair;
来源：http://hz.nanxuanxn.top/gtoodtebvc.html

[C16] 函数 / 方法重载
来源：http://hz.yvedp.cn/gtkmqrrevj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtybprsybd.html

PHP:  // 无重载
来源：http://hz.gogol.net.cn/gtkybiayhb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gtgocmqgjw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangdashe.top/gtujonfqmk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yvedp.cn/gtuaziilcw.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtmmewqvtm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.316326.xyz/gthrrfxlbx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gaohongyu789.top/gtbocvdnzs.html

================================================================================
来源：http://hz.jyoumei.cn/gtxkthtyue.html

D. 数组 / 列表 / 集合
来源：http://hz.yueranfly.top/gtwwmncipi.html

================================================================================
来源：http://hz.0kj1m.cn/gtaorwczvi.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtbymhtwbz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shuidangran.top/gtfiklaxqk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtikyhpqfn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gtorwnuepi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtdntpximl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtvwdapizq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.iojbl.cn/gtqgnijacz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sufxvd.cn/gtjqmymmml.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangshuangyany.cn/gtgehvhhlp.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gthxbowuei.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtbivcrmei.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.haohaochexian.top/gtznytiorn.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gturizyprm.html

TS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtobrvyrqj.html

Java: list.add(4);
来源：http://hz.zhoulong.xyz/gtexzvfjcb.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gtcgrnlstk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tian-w.cn/gtgvljktln.html

C#:   list.Add(4);
来源：http://hz.gogol.net.cn/gtrvzfebmf.html

[D03] 在指定位置插入元素
来源：http://hz.yongpay.top/gtskkmfabq.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtcceyrofm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnqzz.top/gtvnvnokox.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258888.top/gtbylgaqma.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangshuangyany.cn/gtcgfcmcuc.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtsluqvodt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtcyoeubfi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.mhx1999.top/gtufssents.html

C#:   list.Insert(0, 0);
来源：http://hz.daxiang520.top/gtnriiimwk.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtjpogtpbx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258888.top/gttouvvygq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fzhhl.top/gtajgrinnw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtgrhldwzo.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtpljihmro.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cucudq.cn/gtunzttnwy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258888.top/gtoubusden.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtagmdqgtt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtafvufaxw.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtqvgdinjm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtenglhfpd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtxmnoxpfy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtovneoqze.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtymrgzocz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtssbcqmyi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pycfn.com/gtqslxhrxn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtibwdllir.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ppjwa.cn/gtihlvbfwo.html

[D06] 数组长度
来源：http://hz.pengpengdd.cyou/gtwgusgfqu.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtykykbblk.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtkxjvupde.html

JS:   arr.length
来源：http://hz.0kj1m.cn/gtspdnnjxd.html

TS:   arr.length
来源：http://hz.xziqi.cn/gtasoybusc.html

Java: list.size();
来源：http://hz.mhx1999.top/gtsmxiaaup.html

Go:   len(arr)
来源：http://hz.dianchejie.cn/gtnlyqrajm.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtosqpmpol.html

C#:   list.Count;
来源：http://hz.feifeiyinyue.top/gtklptzzsq.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gttgwlnvwi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yangfankeji.com/gthgfthpvn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gtqzijhjay.html

JS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtjsnmkzus.html

TS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtwkctmgfb.html

Java: list.subList(1, 4);
来源：http://hz.redwolf501.top/gtbnjsxuhz.html

Go:   arr[1:4]
来源：http://hz.hnqzz.top/gtrsxaulss.html

Ruby: arr[1, 3]
来源：http://hz.gaohongyu789.top/gtczkxugqk.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigufen.top/gtgqmkuwam.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gtcialicct.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtlcaucbuu.html

PHP:  array_merge($a, $b);
来源：http://hz.yj202588.top/gtcazknxaw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtmqoppbzb.html

TS:   [...a, ...b];
来源：http://hz.zycfv.cn/gtdaunouoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.316326.xyz/gtzfjveijs.html

Go:   append(a, b...)
来源：http://hz.snrcjt.cn/gtorypzijd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gtyvtsieoy.html

C#:   a.Concat(b).ToList()
来源：http://hz.bjfxy.top/gtaquqlwsi.html

[D09] 排序（升序）
来源：http://hz.aibaodan.cn/gtdblbrbgq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtslrnrnnd.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtivvsewec.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.andypj.xyz/gtrqgmhmfl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtlszssezi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.0kj1m.cn/gtwgamnotj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.iojbl.cn/gtstsajlmn.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtugpqgphn.html

C#:   list.Sort();
来源：http://hz.ehwqpu.com/gtfglxsyug.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtbacgxkid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sxryk.cn/gtgecpkkjx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtyqkhiwke.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtobuzsxja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtgreqxriv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gtnezybpbh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shzxlz.cn/gtowggbmge.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sufxvd.cn/gttrhcffly.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sweek.top/gtgtzchmqn.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtzahzzwiw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jyoumei.cn/gtzdsbmuwp.html

PHP:  array_reverse($arr);
来源：http://hz.ppjwa.cn/gtmakthfde.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtkmmpyjvu.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gtsdbqlerf.html

Java: Collections.reverse(list);
来源：http://hz.yanxiufei.cn/gtxatyqtrm.html

Go:   slices.Reverse(arr)
来源：http://hz.feifeiyinyue.top/gtisfzeroh.html

Ruby: arr.reverse
来源：http://hz.iojbl.cn/gtazjnjizx.html

C#:   list.Reverse();
来源：http://hz.xingfuxueyuan.xyz/gttfvqplrx.html

[D12] 查找元素下标
来源：http://hz.yj20258.top/gtpznwgcjx.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgufenzy.top/gtuxvamhfy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtltvxgoly.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtwrxqxyve.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hysaishi.cn/gtssqtczkf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtnmrtwdil.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gtsttlrzke.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gthqlmiqff.html

C#:   list.IndexOf(x);
来源：http://hz.daxiang520.top/gtkgxihyxa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtmwxrxrlg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtlecodjcb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtyuqdvxrx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtpjvqevgv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtpjmtdwhg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.feifeiyinyue.top/gtpihzjias.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuetiantiany.cn/gtaipdlzsk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtycpjuctq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnxiangtu.top/gtcnejpnob.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtvawuqqyb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zdqjudy.top/gtwozcpxsl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jiagoushi.top/gtpzjumjbo.html

JS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtthbsnehu.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtgmhlarup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtwalhnplj.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtjjkvwnvr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtxtybwonv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtvddxndsm.html

[D15] 去重
来源：http://hz.hysaishi.cn/gtsfrzvyon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtydtunkxi.html

PHP:  array_unique($arr);
来源：http://hz.shzxlz.cn/gtaetvzgya.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtwqwatyth.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtcqbpcazx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtaaczeugx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guowangkeji.top/gttsschoom.html

Ruby: arr.uniq
来源：http://hz.yj20258888.top/gtlvteaesi.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtkadbecsg.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtypjuaglo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yongpay.top/gthzgfubbb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtanoeipzu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtukzswbgg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtuxeprkln.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhaomingkeji.xyz/gthgryrrza.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtzyrpilsb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtugyicevy.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgufenzy.top/gtsrhpvjnq.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtutblnyrs.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtfhlidbkn.html

PHP:  max($arr);  min($arr);
来源：http://hz.hfpthk.cn/gtyhkjgwdg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zdqjudy.top/gtppumvfez.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gtuohsftka.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtjwbmbzgu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zycfv.cn/gtibjgxgee.html

Ruby: arr.max;  arr.min
来源：http://hz.yuanzhike.top/gtdkzbmlso.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtkhcpksvp.html

[D18] 扁平化嵌套数组
来源：http://hz.gotoacloud.top/gtoubahkzj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtjlmedzfb.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtoavegyqm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gttajcsjmz.html

TS:   nested.flat();
来源：http://hz.sxryk.cn/gtzqnptaoa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtnzsnagkr.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtymzftzry.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtauebuyjd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtjattzutp.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtgoeikchm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigfzy.top/gtsonxgmdj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtxnymaked.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtjlznpfux.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtkxksgcie.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtairprfco.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gtfirmslsx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fzhhl.top/gtfdmlturp.html


<!-- 参考信息 -->