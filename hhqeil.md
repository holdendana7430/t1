代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cashguo.top/gtxmndmxkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuanzx.com/gtjxjltjsa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtekfobzps.html

Ruby: def greet(name = "World") = name
来源：http://hz.cdnleiting.top/gtifltsftb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yueranfly.top/gtgvroaxkt.html

[C03] 可变参数
来源：http://hz.sufxvd.cn/gtkuqileky.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtkrznxjfv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.iojbl.cn/gtzvkhphzr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtgygxhjas.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtdyqsnrkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gttgrjgszp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtcrvueplw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.svipenyu.cn/gtttspzbvc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shangyingyoupin.top/gtwatafvmp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gaohongyu789.top/gtnkfbdebm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.redwolf501.top/gtaixqvklc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ydjk.org.cn/gtrvftxzwg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtsmukrvnp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.c1oappe.top/gtaikzkdzc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.meibo888.top/gthdsidvgd.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gterwzkwza.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jyoumei.cn/gtfvwrhcse.html

C#:   f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtzvblnjlx.html

[C05] 返回多个值
来源：http://hz.ppjwa.cn/gtfkbyyadm.html

Py:   return a, b
来源：http://hz.guowangkeji.top/gtjnqpdpal.html

PHP:  return [$a, $b];
来源：http://hz.zycfv.cn/gtxxjizvmd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.316326.xyz/gtanhgpgws.html

TS:   return { a, b };
来源：http://hz.fengsongda.top/gtlacuiusi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhijiandao.cn/gtjxfmgpmi.html

Go:   return a, b
来源：http://hz.zycfv.cn/gtynxabujd.html

Ruby: return a, b
来源：http://hz.nwbrower.top/gtepolvdyy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.haohaochexian.top/gtnceakjnl.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtecwnexme.html

Py:   square = lambda x: x * x
来源：http://hz.zycfv.cn/gttgkxnqda.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhengqikj.top/gtzpqohbjy.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtlsxwtrtn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gthzmnnbsl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jyoumei.cn/gttvudzxye.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tian-w.cn/gtbvvslorl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtlxcuqjjl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dianchejie.cn/gtjkpdnoiv.html

[C07] 把函数作为参数传入
来源：http://hz.mhx1999.top/gttyvcuosd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xziqi.cn/gtbfxphlry.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hfpthk.cn/gtuscivykv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xingfuxueyuan.xyz/gtdvlwmwzi.html

TS:   arr.map(String)
来源：http://hz.sysykeji.top/gtzaznvnqt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.316326.xyz/gtjpbqtnqx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.snrcjt.cn/gtsiklgbej.html

Ruby: arr.map(&:upcase)
来源：http://hz.jlsjyb.cn/gtbjutojaz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jiagoushi.top/gtxkwblbxa.html

[C08] 闭包
来源：http://hz.meibo888.top/gtkvexlios.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tian-w.cn/gtngwjdjfu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dashuyun.cn/gtucqxqnpa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtlnjjkjoh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtajhxzvfb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gtjpiylooe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cashguo.top/gtrxtulzmx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dashuyun.cn/gtkmafmiwg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtnepgwgie.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtkgocgcyk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtuaodzpwd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhoulong.xyz/gtvllvlwmt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtdaqyuqdb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtgnjfvoyb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtzdikscdr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtfoxtgcjz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gttvmwjbwk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ivvv.top/gtdccpjqke.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtmupstgkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.iojbl.cn/gtefwjevqn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtwkwiznyo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gotoacloud.top/gtgpbqllfr.html

TS:   同 JS
来源：http://hz.shangyingyoupin.top/gtkdfqmahj.html

Java: 方法内为块级作用域
来源：http://hz.ivvv.top/gtuhlfzqmo.html

Go:   花括号块级作用域
来源：http://hz.zhengqikj.top/gtweperilz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtfztpnnxt.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtqnlzehan.html

[C11] 模块导入与导出
来源：http://hz.sweek.top/gtyqzxunsn.html

Py:   from module import func
来源：http://hz.316326.xyz/gtarmzaobo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.316326.xyz/gteynrndbn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gtfmgzquti.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuanzx.com/gtdlchqrah.html

Java: import java.util.List;
来源：http://hz.xuanzx.com/gteuupmudz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangdashe.top/gtvsygkjru.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cdnleiting.top/gtpayflplh.html

C#:   using System.Text;
来源：http://hz.xuetiantiany.cn/gthjjkuzwf.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gtyqbablkm.html

Py:   (lambda: print("run"))()
来源：http://hz.yueranfly.top/gtoovalzei.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtvvsuzujy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.haohaochexian.top/gtcgnekusz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtwthntcer.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.iojbl.cn/gtrlqiectd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hysaishi.cn/gtxewlddkg.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhijiandao.cn/gtdzkplxwk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hywenlv.cn/gtbguikmym.html

[C13] 类型声明 / 类型注解
来源：http://hz.svipenyu.cn/gtfcmciiwu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtozzkyksp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtsptpkngf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gttjaugtyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtqietytyq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtvfhhwuhs.html

Go:   func add(a, b int) int
来源：http://hz.yuanzhike.top/gtwqiknghq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gthvziinzt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hysaishi.cn/gtzsmutkef.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gtyecsbnhp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtspyhmgcr.html

PHP:  // 无泛型
来源：http://hz.nwbrower.top/gtwngsikjv.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gtgdlroxol.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gtiwvhxonv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zycfv.cn/gtowychand.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daxiang520.top/gtlxwgurpm.html

Ruby: # 无泛型
来源：http://hz.yj202588.top/gtuzqhcpdo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gtcemcsmms.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtktobhcgt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zdqjudy.top/gtcvmikxbi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daria6918.cn/gtmaqtjxom.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtlvpwiihk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tianlin.xyz/gtqoubswqo.html

Java: // 无解构
来源：http://hz.birdmap.top/gtuylktpzw.html

Go:   // 无解构
来源：http://hz.cashguo.top/gteiyzdgzm.html

Ruby: a, b = pair
来源：http://hz.chenzaomai.com/gtbqlqizva.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtjofdtask.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtyhwthzah.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtqajwqqno.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtyufbeemg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guannengcc.top/gtouftwvsq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jiagoushi.top/gtcnlcosms.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.haohaochexian.top/gtivejthrz.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258.top/gtrxzwqetp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guannengcc.top/gteovezgxu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtqnrvhhxn.html

================================================================================
来源：http://hz.xziqi.cn/gtiqmwdiej.html

D. 数组 / 列表 / 集合
来源：http://hz.jinghuilouyu.cn/gtlnttuzxq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjthbkonu.html

[D01] 创建数组 / 列表
来源：http://hz.yvedp.cn/gtxeadaujn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtxmyirwan.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtyrkbjflx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gthqrkctvw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gttgjltqdn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtufxbbyxw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuxming.cn/gtdzkarciw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sweek.top/gtrrgnhakt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jyoumei.cn/gtiucqmydf.html

[D02] 追加元素到末尾
来源：http://hz.ehwqpu.com/gtjpuamqyd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtvgyoxifp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gtrrykcats.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtqdggivcd.html

TS:   arr.push(4);
来源：http://hz.sysykeji.top/gtczbmckpk.html

Java: list.add(4);
来源：http://hz.dashuyun.cn/gtbrbuyshg.html

Go:   arr = append(arr, 4)
来源：http://hz.tian-w.cn/gtlmaxwstz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtczrummfp.html

C#:   list.Add(4);
来源：http://hz.c1oappe.top/gtnedbnsyb.html

[D03] 在指定位置插入元素
来源：http://hz.zhongyouzk.top/gtwwipaisu.html

Py:   arr.insert(0, 0)
来源：http://hz.zdqjudy.top/gtipfyxisn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtxernzoia.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ywan-chungtsiang.top/gtzeycvshy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtqacivjvj.html

Java: list.add(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtzdvzwlsx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.316326.xyz/gtyykehnav.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhoulong.xyz/gtwpupemuh.html

C#:   list.Insert(0, 0);
来源：http://hz.52xcode.cn/gtxkmhwfsl.html

[D04] 删除元素
来源：http://hz.zhiwuduotai.top/gtzubexjgp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gtouqxppeb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtimsstezq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yvedp.cn/gtzbimdyvx.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gtluxgfvua.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gogol.net.cn/gtnftwgynv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydzc1.top/gthiaujeop.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gtmomkumgk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnxiangtu.top/gtnvrnmwkj.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtqthifhnh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtqjksthwq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtvqpxvyfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtsbccisub.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gtecqrrjua.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtmgskbaof.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtmkmtecyy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtngwdumqk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.0kj1m.cn/gtxwtrsghg.html

[D06] 数组长度
来源：http://hz.hnqzz.top/gtzhcntxnp.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtlhpaitby.html

PHP:  count($arr);
来源：http://hz.jinyuanbaomall.cn/gtfwwramlg.html

JS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtykgzotmt.html

TS:   arr.length
来源：http://hz.jiagoushi.top/gtjzlsroic.html

Java: list.size();
来源：http://hz.yonumen.top/gtcxeaolld.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gtkkchrruy.html

Ruby: arr.length; arr.size
来源：http://hz.ydjk.org.cn/gtebxsaehl.html

C#:   list.Count;
来源：http://hz.chenzaomai.com/gtxmlcalfv.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtlamrljbx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuanzx.com/gtttbehsln.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtkiwlxfxh.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtsdjhjhvg.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtfwkxzodf.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtpxslhkcj.html

Go:   arr[1:4]
来源：http://hz.yueranfly.top/gtaezraasq.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtmkncywdv.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenzaomai.com/gtgxxkdxmr.html

[D08] 合并两个数组
来源：http://hz.yuanzhike.top/gteazqcttl.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtcximvpip.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtcmyasigw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtemxnkbtf.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtouqidxsb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cheryme.top/gtqikguexs.html

Go:   append(a, b...)
来源：http://hz.zhijiandao.cn/gtfngrxher.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangkeji.top/gtgkflzxvd.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtpdtsklwo.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtxkhzffgm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtslebwhtg.html

PHP:  sort($arr);
来源：http://hz.feifeiyinyue.top/gtgbosmgqk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtaencwmaa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtgvkscuxm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gzhubu.top/gtytngpook.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtfmwhkdrw.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtjahkicbp.html

C#:   list.Sort();
来源：http://hz.redwolf501.top/gtollvbbrg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtmcfutcim.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gtdcjyretc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtnadmpnci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtbiqisvkk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtebdorpnb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gtqzzppyis.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtqbzguyns.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtgqmhryzn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtawmqqsex.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtlgujyqby.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yuanzhike.top/gtrmyzwogy.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtbkdqiizy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.52xcode.cn/gtbcnqknmd.html

TS:   [...arr].reverse();
来源：http://hz.fzhhl.top/gtuxlhupdn.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gtjplswjoc.html

Go:   slices.Reverse(arr)
来源：http://hz.kuanghao11.cn/gtypkadouy.html

Ruby: arr.reverse
来源：http://hz.pycfn.com/gtfvrmlzkt.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtngzlvgdd.html

[D12] 查找元素下标
来源：http://hz.gzhubu.top/gtgicezmwl.html

Py:   arr.index(x);  x in arr
来源：http://hz.redwolf501.top/gtiibamekd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.havefunace.top/gtbbydelat.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtuflxectg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtnjmisvje.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jianghu66.top/gtqsnwzkaq.html

Go:   slices.Index(arr, x)
来源：http://hz.wangdashe.top/gtxvmsqczx.html

Ruby: arr.index(x)
来源：http://hz.ybcxt.top/gtmgtodmav.html

C#:   list.IndexOf(x);
来源：http://hz.ehwqpu.com/gtbxuqjhdu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gtgmbiymsh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtowrhopmx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgufenzy.top/gtbsjmazyc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtrzufmuri.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtftatdrhf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtrfycvncq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xinyue.icu/gtkykcvwwe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtuevctcrv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ybcxt.top/gthwiiszmt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gtmvyquqmu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhijiandao.cn/gtgyzidzlh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtghocxhzy.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtwsjwuhnh.html

TS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtyzaxsblv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtaenbmtdx.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtteuqmlhn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtmonqjcgk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtgualbzaa.html

[D15] 去重
来源：http://hz.cucudq.cn/gtvmvnitep.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtfnmptyjo.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtpsbrxmcy.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtmcqugpcq.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtxnqfmwfp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxinkj.top/gtqkmkdhnf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtknijwtut.html

Ruby: arr.uniq
来源：http://hz.dashuyun.cn/gtirmarezi.html

C#:   list.Distinct().ToList()
来源：http://hz.guannengcc.top/gtzmjqdebo.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gttfvgewai.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxuanxn.top/gtxrojyssm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aibaodan.cn/gtxirpmycj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtooptgvay.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtpvrvohuu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258.top/gtizkvuzqq.html

Go:   // 手写循环累加
来源：http://hz.yj20258.top/gtcginwvra.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gttlrkzvuk.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gttapkeban.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtmfuzvtop.html

Py:   max(arr);  min(arr)
来源：http://hz.shzxlz.cn/gtbogpjada.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gtukgsiiro.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj202588.top/gtjsnakoxc.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtmmcwzyms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtqhuzprke.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtckqzlxfg.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtpyaarpdu.html

C#:   list.Max();  list.Min()
来源：http://hz.xylfe.cn/gtmuqwpcvs.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtbngpsjyx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cucudq.cn/gtlsybsrke.html

PHP:  array_merge(...$nested);
来源：http://hz.pycfn.com/gtxorhgpzx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.vqdsnc.cn/gttqccbjug.html

TS:   nested.flat();
来源：http://hz.kuanghao11.cn/gtsrkviahz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtjxxskoot.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtcalpswyv.html

Ruby: nested.flatten
来源：http://hz.snrcjt.cn/gtegpxtcjs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtoxcqxfnt.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtfndhifyq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hfpthk.cn/gtxuiftqcm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cheryme.top/gtnsrdusul.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuanzx.com/gtikbpsmkv.html


<!-- 参考信息 -->