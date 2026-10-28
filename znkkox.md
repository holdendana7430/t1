代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.tanke756.top/gtgbiquikg.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtuppvchww.html

Py:   def total(*args): return sum(args)
来源：http://hz.9152youxi.cn/gtwhlbcpeo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtjrwxwtio.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtqizgqryv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtzuiusbas.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtpyegqccz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.0kj1m.cn/gthcneuini.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.redwolf501.top/gteolyktvd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.daxiang520.top/gtqampsveq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dashuyun.cn/gtzngjofwy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.vqdsnc.cn/gtkkukgpje.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ywan-chungtsiang.top/gttbztzulo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtxuslekxo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ydjk.org.cn/gtxsyvgjgo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtswbzasrm.html

Go:   // 无：用配置结构体参数
来源：http://hz.dashuyun.cn/gtekjsiwor.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtfppgffim.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtawofqudp.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtrhgqqlhu.html

Py:   return a, b
来源：http://hz.smart0.xyz/gtctktymlj.html

PHP:  return [$a, $b];
来源：http://hz.sufxvd.cn/gtkxvzkbtl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tian-w.cn/gterallmin.html

TS:   return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtmvxjmegq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenlongwang.top/gtwtdyejbv.html

Go:   return a, b
来源：http://hz.zhongyouzk.top/gtxhcrqdnq.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtyjitmgap.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gaohongyu789.top/gtacljkzdh.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtdzokapaq.html

Py:   square = lambda x: x * x
来源：http://hz.pycfn.com/gteqjzxdhu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhaomingkeji.xyz/gtpjuwhjny.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtahjaqvvk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.iojbl.cn/gttzrislpu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtwzbymslk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xinyue.icu/gtgqrngdfx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dianchejie.cn/gtgmqigazz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtcutscmey.html

[C07] 把函数作为参数传入
来源：http://hz.shzxlz.cn/gtfvufjkck.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tianlin.xyz/gtegpzxsip.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jianghu66.top/gthlfeugfw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtbvktdtgy.html

TS:   arr.map(String)
来源：http://hz.gogol.net.cn/gthwvaayrz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yueranfly.top/gtpkautzuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuanzx.com/gtmqkibrhn.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtifhyflch.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hysaishi.cn/gtqpdmpowq.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtwgpuzmpg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cqqwz.cn/gtqkwuoszb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj202588.top/gtlofazrqi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtmtfsbssc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gthrsbvqlq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.svipenyu.cn/gtcudftbjc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cheryme.top/gtgopqwxty.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gtkhasroiq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtdxdbyjvs.html

[C09] 递归
来源：http://hz.yvedp.cn/gtecpulzvb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtewtrflhh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hysaishi.cn/gtpakkdfcx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtoqvzfojt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtsumlspmg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.52xcode.cn/gtxducztyv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hammf.cn/gtvqxsjsrd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtpuglukrj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jqgfzy.top/gtiichvfkz.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtfflqoqwu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shuidangran.top/gtdwhcsqyt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuanzhike.top/gttyxjazxm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gtigzlllqb.html

TS:   同 JS
来源：http://hz.316326.xyz/gtufqjuxnn.html

Java: 方法内为块级作用域
来源：http://hz.andypj.xyz/gtoqljhghw.html

Go:   花括号块级作用域
来源：http://hz.yj20258888.top/gtadersdss.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.c1oappe.top/gtgwhbajix.html

C#:   块级作用域
来源：http://hz.jqgufenzy.top/gtqmotirpn.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtakwjxcpj.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtlnjzlolk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinghuilouyu.cn/gtvelxeadp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenzaomai.com/gtnmaevgau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gtrxkrfvae.html

Java: import java.util.List;
来源：http://hz.yuanzhike.top/gtqddyalli.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sufxvd.cn/gtwhazwont.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtoloogcfu.html

C#:   using System.Text;
来源：http://hz.cashguo.top/gtqxhzioab.html

[C12] 立即执行函数 IIFE
来源：http://hz.ppjwa.cn/gtupbsnpew.html

Py:   (lambda: print("run"))()
来源：http://hz.xuanzx.com/gtegkozwgz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtpwuuaoth.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtjixvicnz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gteikypiok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ivvv.top/gtcrddtvuy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gaohongyu789.top/gtbbbjlhgh.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtarmqpdsr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigfzy.top/gttdvugqik.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuanzx.com/gtdkmrigbe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.feifeiyinyue.top/gtyesmnnrd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtsclbhawe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtndihhmjc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtxwdabogb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtqwekkzsy.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gttqjraujf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtmasobkcn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangkeji.top/gtexgebrjb.html

[C14] 泛型函数
来源：http://hz.pengpengdd.cyou/gtbpsqtiwz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tanke756.top/gtufesknpl.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtargbbbhf.html

JS:   // 无泛型
来源：http://hz.xylfe.cn/gtwkpujvqe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtacvlfehb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yongpay.top/gtiboddvts.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gttivdwcwe.html

Ruby: # 无泛型
来源：http://hz.316326.xyz/gtjftetbig.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xziqi.cn/gtsiibywyg.html

[C15] 解构 / 展开参数
来源：http://hz.yueranfly.top/gtmimxptgw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gttsmpvkex.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gtjlljiefq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtpkcagajq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tianlin.xyz/gtdnbetpyc.html

Java: // 无解构
来源：http://hz.daxiang520.top/gtdmxldnjr.html

Go:   // 无解构
来源：http://hz.yj202588.top/gtyohxbxcd.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtvvanthvk.html

C#:   var (a, b) = pair;
来源：http://hz.dashuyun.cn/gtlarxyxfq.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtgdmzykjj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.smart0.xyz/gtxzomofeb.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtjitirhjz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenjidiqi.icu/gtcffsbjbm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gtbzoocsuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xziqi.cn/gtdsvvkqxb.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtjkfbfjia.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhongyouzk.top/gtrxcabjmr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangkeji.top/gtgafzyrhy.html

================================================================================
来源：http://hz.zycfv.cn/gtqojrbirh.html

D. 数组 / 列表 / 集合
来源：http://hz.shuidangran.top/gtfjmavaul.html

================================================================================
来源：http://hz.aibaodan.cn/gtxnnqwdrz.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtyrkbpruy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fengsongda.top/gtueogdnvq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtdvudccei.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gzhubu.top/gtgubigksu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ybcxt.top/gtunadvuwm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtlfqacwnn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hysaishi.cn/gtzttyuaju.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtzjhxmkib.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtxefqbgry.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtorrjtbvz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gtmvsdwzlm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtfjgdbsoc.html

JS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtrfufamce.html

TS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtumqshxus.html

Java: list.add(4);
来源：http://hz.gotoacloud.top/gtrzetqlsu.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtznxxniiu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxinkj.top/gtzfwujrpx.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gttoyqgldc.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtqbznkpnj.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigfzy.top/gtqxtpgwio.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cashguo.top/gttrjluzqf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuanzx.com/gtmnybwbym.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtxnkuqbjs.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtkkcswyzr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sxryk.cn/gtivaihiym.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtdxmweelh.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgufenzy.top/gtjvmwdyrt.html

[D04] 删除元素
来源：http://hz.wangdashe.top/gtlavkhiic.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtfnlmeffi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtbqctlnml.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xingfuxueyuan.xyz/gttqienpnj.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258.top/gtqysnldcr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnqzz.top/gtnnarymme.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gthcsoslsx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.316326.xyz/gtcdqzfexp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cashguo.top/gtffsblmgh.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gtbuqztmpj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yonumen.top/gtrgxlpcro.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtajewaxoj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.andypj.xyz/gtqjpabxgf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtwvnmodsh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.meibo888.top/gtveljkoig.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xinyue.icu/gttcxphotv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtytqdnhvy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtziahovjg.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtkvwjasez.html

Py:   len(arr)
来源：http://hz.yj202588.top/gtlfabjnvd.html

PHP:  count($arr);
来源：http://hz.jinyuanbaomall.cn/gtoplstoyv.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtejjcyglw.html

TS:   arr.length
来源：http://hz.hnqzz.top/gtvtevksmu.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtdmvpirjy.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gtpbeszkpk.html

Ruby: arr.length; arr.size
来源：http://hz.zhaomingkeji.xyz/gtepepurcl.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtogulyntx.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtvnqazvdk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydzc1.top/gtoyrzaquj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.52xcode.cn/gtxzccfego.html

JS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtmcqkpslf.html

TS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gtnnvowmib.html

Java: list.subList(1, 4);
来源：http://hz.gzhubu.top/gtnuwpiqzf.html

Go:   arr[1:4]
来源：http://hz.shzxlz.cn/gtvemxftux.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtcdncznyb.html

C#:   list.GetRange(1, 3);
来源：http://hz.ppjwa.cn/gtscjxbqci.html

[D08] 合并两个数组
来源：http://hz.chenzaomai.com/gttfvtauyf.html

Py:   a + b;  a.extend(b)
来源：http://hz.cucudq.cn/gtpmlzvoyl.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtnuceqpjv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shangyingyoupin.top/gtmgurstsp.html

TS:   [...a, ...b];
来源：http://hz.zhijiandao.cn/gtxaqbhvwl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jyoumei.cn/gtjdgojhhy.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gtzwrrntza.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gthubbvuty.html

C#:   a.Concat(b).ToList()
来源：http://hz.ppjwa.cn/gtithipuue.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtwvrofzfv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtgnawhkqu.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtzqffzxrn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhijiandao.cn/gtnhmoomly.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gtsdrognsu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnxiangtu.top/gtmbuajffp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtsmrnexdi.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gthvajbffb.html

C#:   list.Sort();
来源：http://hz.andypj.xyz/gtuznwzemj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hongshengwenyu.top/gtrqsdsmhi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shuidangran.top/gtkefebiha.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.havefunace.top/gtoboephdv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dianchejie.cn/gtylbijqwo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtutdplniy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangkeji.top/gtdxzmspyx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yongpay.top/gtqfaauydk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.birdmap.top/gtibyaxuej.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtwbndydgk.html

[D11] 反转数组
来源：http://hz.hysaishi.cn/gtbwohyfir.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.quarkkingdee.top/gtdxfgslfc.html

PHP:  array_reverse($arr);
来源：http://hz.snrcjt.cn/gtjiqaorvk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.snrcjt.cn/gtpzhodfgp.html

TS:   [...arr].reverse();
来源：http://hz.xylfe.cn/gtmizoiawq.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gtwpxlklvx.html

Go:   slices.Reverse(arr)
来源：http://hz.yongpay.top/gteobpjgvc.html

Ruby: arr.reverse
来源：http://hz.xingfuxueyuan.xyz/gtemkhmkxx.html

C#:   list.Reverse();
来源：http://hz.quarkkingdee.top/gtchsubhzq.html

[D12] 查找元素下标
来源：http://hz.guannengcc.top/gtdjefestb.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtzsnwcduf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhoulong.xyz/gturacsvwu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtwsildjdr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gterzysqaz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtxlpkrmuf.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtjvchzied.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtoqgkrvxb.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtdxobfinf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtccuqjgpz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.haohaochexian.top/gtyxuxwfkt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xziqi.cn/gtjudiuydu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtdyczazea.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtzhvlhpnf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhengqikj.top/gtjvldcfau.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangdashe.top/gtuozyiukk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtejcjalas.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.havefunace.top/gthfjepxau.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtowwgmlno.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtyviwzvvn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtaumpcavb.html

JS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtntpbonyg.html

TS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtjehkugal.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gtksrcjzml.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtndsbwkuc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtoxvgyksi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gticnhkkye.html

[D15] 去重
来源：http://hz.shzxlz.cn/gtywtkfghn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aizwys.cn/gtuiewfdig.html

PHP:  array_unique($arr);
来源：http://hz.aibaodan.cn/gtxybirkyj.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtvlnjcchn.html

TS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtfujjylug.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.mhx1999.top/gthwarglrs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.smart0.xyz/gtnkcczxyu.html

Ruby: arr.uniq
来源：http://hz.jlsjyb.cn/gtwzjvnkyr.html

C#:   list.Distinct().ToList()
来源：http://hz.c1oappe.top/gtqnjomctd.html

[D16] 求和与平均值
来源：http://hz.haohaochexian.top/gteziponvh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xylfe.cn/gtxofqutjb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cqqwz.cn/gtoblygcil.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtstsltoii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtfhmueocw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cucudq.cn/gtmvkwktlh.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtxpgixmup.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shuidangran.top/gtqwpqcuso.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangdashe.top/gtxmuaufpo.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtscvhsrqu.html

Py:   max(arr);  min(arr)
来源：http://hz.gaohongyu789.top/gtejfmvazt.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhaomingkeji.xyz/gtnasslpwt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gtmomycezn.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtuaeflrgj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtfwkofhnd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.iojbl.cn/gtrjrslocq.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgfzy.top/gtfxtutqhj.html

C#:   list.Max();  list.Min()
来源：http://hz.chenlongwang.top/gthkuchpqw.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtcoslxytj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gogol.net.cn/gtpaouvbqq.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtxmvzljaa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigufen.top/gtxfttszwz.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gthiobugmt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtctrlmzid.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtxdbiiyic.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtbxqavdws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gtcffdzygn.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtndpxinna.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinyuanbaomall.cn/gtmdbrwvok.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cheryme.top/gtlszwbcvo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtotarlvee.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hfpthk.cn/gtvozmqknr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.9152youxi.cn/gtmdicvwws.html

Go:   // 手写 map[string][]T
来源：http://hz.pengpengdd.cyou/gtejzaeyoc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtlfxancma.html


<!-- 参考信息 -->