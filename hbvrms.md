代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tianlin.xyz/gtqdjzsitr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aizwys.cn/gtgzomhnpo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtmlmmjklp.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigfzy.top/gtpghcceau.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yangfankeji.com/gtympgzhow.html

[C03] 可变参数
来源：http://hz.tian-w.cn/gtyqksesxt.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gtzfciarlu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhoulong.xyz/gtaihirvgq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtddopxqbf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtjwebgjle.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtkilybtei.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuanzhike.top/gtcmothohe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ywan-chungtsiang.top/gtrdmwjmjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnqzz.top/gtwkzceayz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fengsongda.top/gtjfcvstib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gtxqmeccvu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtnxhiqdqg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtlhsgirtt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhiwuduotai.top/gtzkeqcfjp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jiagoushi.top/gtrvrnvhbw.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtizuqxefp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtxwqqszbi.html

C#:   f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtreazkhbb.html

[C05] 返回多个值
来源：http://hz.daria6918.cn/gtiunfqqln.html

Py:   return a, b
来源：http://hz.snrcjt.cn/gtyjmjtnlc.html

PHP:  return [$a, $b];
来源：http://hz.redwolf501.top/gtqhxcefqm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhengqikj.top/gtwesxsnpr.html

TS:   return { a, b };
来源：http://hz.jinghuilouyu.cn/gtnrnahrlr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zycfv.cn/gtzartrswq.html

Go:   return a, b
来源：http://hz.shangyingyoupin.top/gtwcdyinfy.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtqjyjtmnj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.bjfxy.top/gtadajskmo.html

[C06] 匿名函数 / lambda
来源：http://hz.0kj1m.cn/gtxuscvbze.html

Py:   square = lambda x: x * x
来源：http://hz.jiagoushi.top/gtawqxhjte.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jianghu66.top/gtetgkbzft.html

JS:   const square = x => x * x;
来源：http://hz.jinqigufen.top/gtywydvvra.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gttymfssuq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dianchejie.cn/gtjmtphnsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuanzx.com/gtjvrhfoei.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtzdjktamg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenzaomai.com/gtqviltult.html

[C07] 把函数作为参数传入
来源：http://hz.hysaishi.cn/gtruhsolxh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.quarkkingdee.top/gtvbwzvtuy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fengsongda.top/gtbyjdgsyw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xinyue.icu/gtgauckqvi.html

TS:   arr.map(String)
来源：http://hz.haohaochexian.top/gtjxofwubq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.feifeiyinyue.top/gtxlufribh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtuuyycovy.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtrlaryooq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtuhqlhmqy.html

[C08] 闭包
来源：http://hz.cucudq.cn/gtesdgkxtz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydjk.org.cn/gtjkpayntn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gtagvcvlcq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtydqdfiiq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtbrymgqbu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nwbrower.top/gtexuuouzr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yvedp.cn/gtdqbiqtaj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenjidiqi.icu/gthacqrmgd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtaimbimiy.html

[C09] 递归
来源：http://hz.chenzaomai.com/gtyjsjrtze.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtqvwyljuu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hysaishi.cn/gtwzanwjph.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtlwaibfvh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtrlefmqcf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.feifeiyinyue.top/gtnxeawhdn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gtypvngwxe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtdmeqnyoq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yvedp.cn/gtijrojqvi.html

[C10] 变量作用域
来源：http://hz.guannengcc.top/gtccyhpihs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nwbrower.top/gtvjzmrnlj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xinyue.icu/gtbnrvnajq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xingfuxueyuan.xyz/gtlsyyvspw.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtlhyjmnjy.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtouzzatir.html

Go:   花括号块级作用域
来源：http://hz.jianghu66.top/gttwxlfzsv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gthaupknhu.html

C#:   块级作用域
来源：http://hz.quarkkingdee.top/gtdtikbkzw.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gtcwlwflzk.html

Py:   from module import func
来源：http://hz.shanyushiyangtech.top/gtwphtcngm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gtnchvurcs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hysaishi.cn/gtlvtqolni.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xinyue.icu/gtpkmeibmm.html

Java: import java.util.List;
来源：http://hz.yonumen.top/gtlqvpwbnw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangshuangyany.cn/gtqolzlzuh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtynzpgejj.html

C#:   using System.Text;
来源：http://hz.jyoumei.cn/gtwenwsarc.html

[C12] 立即执行函数 IIFE
来源：http://hz.yangfankeji.com/gtidqlfqvi.html

Py:   (lambda: print("run"))()
来源：http://hz.xuanzx.com/gtuphxabec.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xinyue.icu/gtrupsriai.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtkdayftbg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gtgajknkmq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yanxiufei.cn/gtpzlxcien.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtjuyicthu.html

Ruby: -> { puts "run" }.call
来源：http://hz.havefunace.top/gtjoxygcmr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtmpxlhhre.html

[C13] 类型声明 / 类型注解
来源：http://hz.aizwys.cn/gtjwmfhlni.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtlbyauivd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtvtdmqahn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dashuyun.cn/gtehgwnhad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtqosqigtk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtbzipelsz.html

Go:   func add(a, b int) int
来源：http://hz.chenzaomai.com/gtbeqjrkic.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxuanxn.top/gtwspsnscr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuanzx.com/gttobobxzq.html

[C14] 泛型函数
来源：http://hz.cqqwz.cn/gtecwfnfur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtbqaosvpw.html

PHP:  // 无泛型
来源：http://hz.zhaomingkeji.xyz/gtelddtemm.html

JS:   // 无泛型
来源：http://hz.guannengcc.top/gtmarssxah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtotmhyyvk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gthlawjilm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangtech.top/gtvoabruqf.html

Ruby: # 无泛型
来源：http://hz.zhixingplan.top/gtpyspbdcm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gtdmbtlyni.html

[C15] 解构 / 展开参数
来源：http://hz.xingfuxueyuan.xyz/gtcvoloebg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtpqvahmip.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guowangkeji.top/gtnfqxxtko.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtpohevuip.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daria6918.cn/gtzuakqzpo.html

Java: // 无解构
来源：http://hz.yongpay.top/gtcajcjrph.html

Go:   // 无解构
来源：http://hz.aizwys.cn/gtkrisselc.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gtaoiwkzwj.html

C#:   var (a, b) = pair;
来源：http://hz.ppjwa.cn/gtnnagwzop.html

[C16] 函数 / 方法重载
来源：http://hz.yvedp.cn/gtcqcbdkhs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gtwwlzoezo.html

PHP:  // 无重载
来源：http://hz.wangshuangyany.cn/gtznhjfifc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.iojbl.cn/gtgwclgvab.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtoaulpkhp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtpevopzzj.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtemqbbsbj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gthciihtvo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shuidangran.top/gtelvkzjhr.html

================================================================================
来源：http://hz.zhixingplan.top/gtzjpqktqp.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtvrrxgetz.html

================================================================================
来源：http://hz.zhengqikj.top/gttawanbqu.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtptrckjjp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hysaishi.cn/gtepyudjfe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.0kj1m.cn/gtzzwpckdm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtbpwrjiid.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhengqikj.top/gtxhujejih.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtudsggmnh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.316326.xyz/gtdkryunpq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtzdfbdnww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cashguo.top/gtpfkswxtj.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtwcxyrtfe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gteubsvaal.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shangyingyoupin.top/gtqnsiydfj.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtvzyntvoy.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtwnnhaajf.html

Java: list.add(4);
来源：http://hz.cashguo.top/gtuorfdodm.html

Go:   arr = append(arr, 4)
来源：http://hz.jinghuilouyu.cn/gtdqqguvdw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zycfv.cn/gtjvghkuzc.html

C#:   list.Add(4);
来源：http://hz.gogol.net.cn/gtjjytomnp.html

[D03] 在指定位置插入元素
来源：http://hz.chenzaomai.com/gtaytqjjdk.html

Py:   arr.insert(0, 0)
来源：http://hz.shangyingyoupin.top/gtseklhgvx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sweek.top/gtrljqimkc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hammf.cn/gtdzjrhcdo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtwwavxihr.html

Java: list.add(0, 0);
来源：http://hz.xylfe.cn/gtyrjrkzdn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zycfv.cn/gtajfmhshf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hywenlv.cn/gtintznssl.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtlefpinsw.html

[D04] 删除元素
来源：http://hz.aibaodan.cn/gtvdujrsky.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhiwuduotai.top/gtgprkkivc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yongpay.top/gtsigrcehp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtzeoocbqf.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxuanxn.top/gtryvtlbje.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.dianchejie.cn/gtjnancbvs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sxryk.cn/gtxiovexsk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtetvpxygx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtjatcafad.html

[D05] 访问与修改元素
来源：http://hz.meibo888.top/gtlzvmjtsi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gtbrcgxryu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtuiwlimbj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtgnwljaso.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtqdoplsqu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydjk.org.cn/gtizgwerus.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnqzz.top/gtttworxdb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtxwtlwgkc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtemtnzlni.html

[D06] 数组长度
来源：http://hz.cashguo.top/gtyarswehl.html

Py:   len(arr)
来源：http://hz.xylfe.cn/gtthvxzjlc.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtrwlgdmcq.html

JS:   arr.length
来源：http://hz.zhijiandao.cn/gtzusebuxx.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtwumuiadq.html

Java: list.size();
来源：http://hz.fengsongda.top/gthdipnlmc.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtjthmfbdh.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtxybxlvmq.html

C#:   list.Count;
来源：http://hz.wangshuangyany.cn/gttzgtkouv.html

[D07] 切片 / 取子数组
来源：http://hz.c1oappe.top/gtiqrljrxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jlsjyb.cn/gtyllqsaaz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.smart0.xyz/gthhxotilh.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtdoxkhfwi.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtsbnbtptn.html

Java: list.subList(1, 4);
来源：http://hz.havefunace.top/gtjdlhsmty.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtqvhsadio.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtwfpqvshv.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinghuilouyu.cn/gttwxtchak.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtwxbzkfcn.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtampuaclm.html

PHP:  array_merge($a, $b);
来源：http://hz.mhx1999.top/gtkmkbzyro.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gtaopbiibo.html

TS:   [...a, ...b];
来源：http://hz.quarkkingdee.top/gtxammdtdb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtzfwzfkql.html

Go:   append(a, b...)
来源：http://hz.zhengqikj.top/gtibjeaczw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sufxvd.cn/gtbqnsztic.html

C#:   a.Concat(b).ToList()
来源：http://hz.ivvv.top/gtevkjskfo.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtlfcilueq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtaxhdukdv.html

PHP:  sort($arr);
来源：http://hz.yj20258888.top/gtdryxlxeb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shuidangran.top/gtfrnaadtg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.vqdsnc.cn/gtdswxjtxj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtzgpvkczw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.bjfxy.top/gthuffyusi.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtcjjokthp.html

C#:   list.Sort();
来源：http://hz.yueranfly.top/gtwfaegthk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtqroazrgx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guowangkeji.top/gtbvckassm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtugpfniqp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtcdmjoiuc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtejwcsivc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daria6918.cn/gtpicgprux.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yonumen.top/gtcdpgqlob.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtpwidjgvc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtzzwcwxke.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtmhjunppy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtjvwjujlq.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigfzy.top/gtcdzcrzwr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fzhhl.top/gtlpskhzlp.html

TS:   [...arr].reverse();
来源：http://hz.meibo888.top/gtlzjulror.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gthihduitl.html

Go:   slices.Reverse(arr)
来源：http://hz.shangyingyoupin.top/gtywwmueig.html

Ruby: arr.reverse
来源：http://hz.jinqigufen.top/gtqzmhdfpj.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtrvvcucbb.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gttzomaqwq.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtlwjvcqya.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gtpounsvhj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtbxzfbgpo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtyzxablil.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj202588.top/gtbomtarrv.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gtohaufdgm.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtmebkslmw.html

C#:   list.IndexOf(x);
来源：http://hz.ybcxt.top/gtjvuygjfg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtrkicqjot.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtyeafvhpg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fengsongda.top/gtqinxstqx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtblymjbyv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtnktomlna.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtxsitkkqu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fengsongda.top/gtjzwceger.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ehwqpu.com/gtpnpaimtw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtrpkltzvq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shzxlz.cn/gtkodmnkld.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cqqwz.cn/gtkzokblii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yongpay.top/gtplhhfrnb.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtrzvqkueq.html

TS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtpdybuvxt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sweek.top/gtwttzendv.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtwkgnnldi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtugqsgzlm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hfpthk.cn/gtxixirnjd.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtxsaktlch.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gteqplzhhw.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtoyusgizk.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtfbvopsmn.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtgdlitujd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuetiantiany.cn/gtbcpnovju.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtbipikkht.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtzpsbtqsc.html

C#:   list.Distinct().ToList()
来源：http://hz.guowangkeji.top/gtpchiggnt.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtvkzpbidz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cdnleiting.top/gtrswudenk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sweek.top/gtuvgrojar.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtyhldkfsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtubuxolca.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gogol.net.cn/gtdbuayhye.html

Go:   // 手写循环累加
来源：http://hz.jinqigfzy.top/gtttnphhib.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.kuanghao11.cn/gtvwioruda.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gtfuwlrgie.html

[D17] 最大值与最小值
来源：http://hz.iojbl.cn/gtdwthkuhj.html

Py:   max(arr);  min(arr)
来源：http://hz.c1oappe.top/gtsctdygun.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenzaomai.com/gtjbsnccvy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258.top/gtbzhdnfdk.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtfwukjvfx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtjzslzzsh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shanyushiyangtech.top/gtsroiklnl.html

Ruby: arr.max;  arr.min
来源：http://hz.shuidangran.top/gtoigzqheo.html

C#:   list.Max();  list.Min()
来源：http://hz.zhaomingkeji.xyz/gtfgszsimg.html

[D18] 扁平化嵌套数组
来源：http://hz.quarkkingdee.top/gtsuzwtvxt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtfivfwgee.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtjbjgpors.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenzaomai.com/gtvdhqfbeq.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtebzfuanj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xingfuxueyuan.xyz/gtexfatqpp.html

Go:   // 手写双层循环
来源：http://hz.zycfv.cn/gtwbqkxdua.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtjonclqoq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daxiang520.top/gtmmylbisx.html

[D19] 按字段分组
来源：http://hz.zhixingplan.top/gturlaruua.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.svipenyu.cn/gtvufzkpls.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydjk.org.cn/gtfbeyubal.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuanzhike.top/gtcwuvbkoe.html


<!-- 参考信息 -->