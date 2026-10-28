代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gtvjrkndpv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtltnmhqgz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.aibaodan.cn/gtxxretalw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ehwqpu.com/gtygmitjew.html

Go:   // 无：用配置结构体参数
来源：http://hz.xylfe.cn/gtpntpvuqu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtrsjuhohl.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gtdxlxyvmw.html

[C05] 返回多个值
来源：http://hz.yj20258888.top/gtncjqfgkr.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtpujfdpco.html

PHP:  return [$a, $b];
来源：http://hz.vqdsnc.cn/gtqhobqxyk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtttjrklkw.html

TS:   return { a, b };
来源：http://hz.birdmap.top/gteljvdwvp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtbxkazcqc.html

Go:   return a, b
来源：http://hz.nanxinkj.top/gtswknrasj.html

Ruby: return a, b
来源：http://hz.yueranfly.top/gtvlszfusb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.havefunace.top/gtrjhlpzsr.html

[C06] 匿名函数 / lambda
来源：http://hz.hammf.cn/gtvonbnqql.html

Py:   square = lambda x: x * x
来源：http://hz.sysykeji.top/gtcvxdghrl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hammf.cn/gtdzngmixx.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gtkymvpitl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gthgicthlo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtivwdakhx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nwbrower.top/gtnwoomvbr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtghjfvjel.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtnuudxnbn.html

[C07] 把函数作为参数传入
来源：http://hz.9152youxi.cn/gtyxzvyycs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj202588.top/gtdxnvsksy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gttoykjbvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtbsnicbwo.html

TS:   arr.map(String)
来源：http://hz.zhengqikj.top/gtsirlwhun.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cheryme.top/gttwgfcgnw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cashguo.top/gtjjntalws.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gtkxgysyyp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xingfuxueyuan.xyz/gtzpwwjboo.html

[C08] 闭包
来源：http://hz.jinghuilouyu.cn/gtkoxwwxet.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangtech.top/gttbtpqrbw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.andypj.xyz/gtcyajdggt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtxieckfww.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtqkhswkjo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtyejdqriw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jianghu66.top/gtptaibjyq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ywan-chungtsiang.top/gtumvilmyz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gttmkjtiex.html

[C09] 递归
来源：http://hz.shangyingyoupin.top/gtwxelfcns.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yongpay.top/gtzecjyzuc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yanxiufei.cn/gtosnykkhp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtjojggzgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtwkfhemoa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtfvbntwxf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gtinynvsfm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtufmxpsuk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gtozghlnts.html

[C10] 变量作用域
来源：http://hz.vqdsnc.cn/gtsccjnuht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtwgegxwtf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cashguo.top/gttbqpzvni.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cqqwz.cn/gtxgkjcnxq.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtxgxtsjfb.html

Java: 方法内为块级作用域
来源：http://hz.yvedp.cn/gtkjyfdkiz.html

Go:   花括号块级作用域
来源：http://hz.cucudq.cn/gtveftlfpd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ybcxt.top/gtyhjxeeeh.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gttmkodncv.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtlvdpiakj.html

Py:   from module import func
来源：http://hz.yj20258.top/gtluwtyfoh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxuanxn.top/gtqsotjipj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sysykeji.top/gtslwwovhu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.0kj1m.cn/gtgxlzagrw.html

Java: import java.util.List;
来源：http://hz.xuetiantiany.cn/gtrnrrmsxg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtvbffzfhh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuanzhike.top/gtiwtdjevn.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtgkmcoaey.html

[C12] 立即执行函数 IIFE
来源：http://hz.xziqi.cn/gtevsqnddo.html

Py:   (lambda: print("run"))()
来源：http://hz.fzhhl.top/gttxtqvuym.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtggymygsv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtidbfwiqp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtgzlfkpaw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnxiangtu.top/gtslqilbyd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtuxdswpor.html

Ruby: -> { puts "run" }.call
来源：http://hz.svipenyu.cn/gtwlmkmutw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtgvgkssbl.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gthwikzudx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xinyue.icu/gtsgjetxbq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtnyphtccv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtbfnytutc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtzwidkbqe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtkztavcke.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtweksjykn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gtajbwoawl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtzphdsqlr.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gtwcaemamm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xinyue.icu/gtcilvmnnv.html

PHP:  // 无泛型
来源：http://hz.guowangkeji.top/gtruibevhw.html

JS:   // 无泛型
来源：http://hz.yongpay.top/gtxwfhplab.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gtwooktgvs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.c1oappe.top/gtxzlppgyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sysykeji.top/gtnlhcawaq.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtzostsjes.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shzxlz.cn/gtxwfscoyg.html

[C15] 解构 / 展开参数
来源：http://hz.zycfv.cn/gtmtaqyhea.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tanke756.top/gtuudtviud.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hammf.cn/gtxttlqrvp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtgcmmxbbb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ywan-chungtsiang.top/gtjdedecva.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtbonerlvj.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gtonpbmizg.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtbpfujpqo.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gtbpuysvqf.html

[C16] 函数 / 方法重载
来源：http://hz.jianghu66.top/gtiuptpvem.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gtxwcrjojj.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtdylxzadl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtoqygcjda.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.meibo888.top/gtfrlsrakk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.meibo888.top/gtkscrunsq.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtiakdmnqe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhoulong.xyz/gtovbjoezw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhijiandao.cn/gtyrufcinj.html

================================================================================
来源：http://hz.9152youxi.cn/gteqrhrdoj.html

D. 数组 / 列表 / 集合
来源：http://hz.yongpay.top/gtppwzqwol.html

================================================================================
来源：http://hz.hfpthk.cn/gtnvwhhtat.html

[D01] 创建数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtctqsyeup.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ppjwa.cn/gteeqwkauw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pycfn.com/gttlckeoyj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jyoumei.cn/gtoontedih.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yongpay.top/gttrscidwq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258888.top/gtdqvhuace.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenjidiqi.icu/gtqkmsgtwe.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xingfuxueyuan.xyz/gtkchafjgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fzhhl.top/gtxegmjeqw.html

[D02] 追加元素到末尾
来源：http://hz.gotoacloud.top/gtgzouwrle.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dianchejie.cn/gtefxntumg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xziqi.cn/gtewpvhaqg.html

JS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtlnbozfcb.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtepfbglve.html

Java: list.add(4);
来源：http://hz.zhixingplan.top/gtpywgoxjy.html

Go:   arr = append(arr, 4)
来源：http://hz.chenlongwang.top/gtuowzdebl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cucudq.cn/gtdwdobrtz.html

C#:   list.Add(4);
来源：http://hz.52xcode.cn/gtxkwrigpl.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtkliifseu.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgfzy.top/gtqknmnarc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnqzz.top/gtexobhvxz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.quarkkingdee.top/gtndfcpwkz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.9152youxi.cn/gtxpxcldsh.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gtmbtlmitd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtvharatus.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinghuilouyu.cn/gtmseywtdg.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gthlnopfuf.html

[D04] 删除元素
来源：http://hz.jiagoushi.top/gteicpkjij.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtqydakzys.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtdhgupzvg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydjk.org.cn/gtzqrvvact.html

TS:   arr.splice(0, 1);
来源：http://hz.feifeiyinyue.top/gtzjwghmee.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gtcunqchzs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuanzx.com/gtahtyfrzz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gtttnjelco.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxinkj.top/gtozabxsyn.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtyizussna.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtjuaawbvm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gzhubu.top/gtyilqiiej.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hammf.cn/gtrgwibviz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.0kj1m.cn/gtfxnpypcc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtlufqfgrw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fengsongda.top/gtlxebhlla.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtaitdfoma.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuanzhike.top/gtzqidpcxo.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gttkfsgmzx.html

Py:   len(arr)
来源：http://hz.wangdashe.top/gtisrhnpts.html

PHP:  count($arr);
来源：http://hz.0kj1m.cn/gtjsvwjbzz.html

JS:   arr.length
来源：http://hz.kuanghao11.cn/gtgrghdsmu.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gthnaepszu.html

Java: list.size();
来源：http://hz.316326.xyz/gtolucchqv.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtbvzevohb.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtcqxkvxxf.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtxefxwiqs.html

[D07] 切片 / 取子数组
来源：http://hz.xylfe.cn/gtlnpxzqhu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ivvv.top/gtfwjjwzcs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gthjezccjr.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtnwcppiub.html

TS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtmrwxswrm.html

Java: list.subList(1, 4);
来源：http://hz.kuanghao11.cn/gtcuyarzcg.html

Go:   arr[1:4]
来源：http://hz.yuanzhike.top/gtkpmcpjhv.html

Ruby: arr[1, 3]
来源：http://hz.gogol.net.cn/gtjunmhbxk.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtbzvjfufe.html

[D08] 合并两个数组
来源：http://hz.0kj1m.cn/gtcqezwdeo.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtsxndvmtp.html

PHP:  array_merge($a, $b);
来源：http://hz.hfpthk.cn/gteqdspdin.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gtcotgmxtk.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtesoujpfq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgufenzy.top/gtcxfigamx.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtsbvyigyz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuanzhike.top/gtxbvoeerf.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtrgtfrjct.html

[D09] 排序（升序）
来源：http://hz.xingfuxueyuan.xyz/gtqgvkoxsg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtaaphiyvb.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtkmayurna.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gteqwqmrlm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhiwuduotai.top/gtajmshnpu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.9152youxi.cn/gtxgtqhprk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.mhx1999.top/gtgrtygjao.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtzhqiwfmp.html

C#:   list.Sort();
来源：http://hz.zhoulong.xyz/gtyuwekrkf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sweek.top/gtmfsnoaiy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gtdepebrti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtxchgohbe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gttqntjvix.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gteuhfyssz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cheryme.top/gtglcsecvw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtrptilavl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtrhzhyuff.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtuoqufqgw.html

[D11] 反转数组
来源：http://hz.hongshengwenyu.top/gtygansqgo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yongpay.top/gtsakkcfjt.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangkeji.top/gtzqkwgiku.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gttbokkhcl.html

TS:   [...arr].reverse();
来源：http://hz.jianghu66.top/gtxterrwhg.html

Java: Collections.reverse(list);
来源：http://hz.fengsongda.top/gtjprpcovo.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtsdrhqrvj.html

Ruby: arr.reverse
来源：http://hz.c1oappe.top/gtsbzaktyk.html

C#:   list.Reverse();
来源：http://hz.chenlongwang.top/gtqyglkbow.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtacwlbxed.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydjk.org.cn/gtuirrsmlr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhiwuduotai.top/gtfocvhthh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtispzyjyh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtoewtwpif.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gtdsluwrqp.html

Go:   slices.Index(arr, x)
来源：http://hz.zhijiandao.cn/gtmozyions.html

Ruby: arr.index(x)
来源：http://hz.dashuyun.cn/gtwssycycq.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtkzhwzwms.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yonumen.top/gthhuxknla.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cdnleiting.top/gtwlqunvep.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.smart0.xyz/gtypzyyhdr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtusmhenxv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gthtavudvu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinghuilouyu.cn/gtezknxhuc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hfpthk.cn/gthtxxgpkp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtibvqqkqk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gtfettmjnp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.iojbl.cn/gtwawpftju.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gtaunqgstp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinghuilouyu.cn/gtmagxongt.html

JS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gthqnaezfe.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtmhfwksev.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xylfe.cn/gtdhwgpuyk.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtktflqwjf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtbmhtbxsc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtmhjqjtps.html

[D15] 去重
来源：http://hz.chenjidiqi.icu/gtkirgdfgg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtvibtiuka.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtzzhcyeea.html

JS:   [...new Set(arr)]
来源：http://hz.guowangkeji.top/gtwagddlqu.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtmmroxbbr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cdnleiting.top/gtmduymouv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtnnxzcndr.html

Ruby: arr.uniq
来源：http://hz.316326.xyz/gtwsohndjw.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtwzsvxtqf.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtuptzepzg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gthdfhrlne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtcigxfnpl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtyzeygqdl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtftjignud.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jianghu66.top/gtinhfbeft.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtxglsaicc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yongpay.top/gtbhbvwbtq.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinghuilouyu.cn/gtqwbbeown.html

[D17] 最大值与最小值
来源：http://hz.xziqi.cn/gtjziinjrx.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtdqemrrfu.html

PHP:  max($arr);  min($arr);
来源：http://hz.dashuyun.cn/gtxwfhoqgj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xylfe.cn/gtwlbdqbvu.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gtyslyzofi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtidtujnzn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtoymjfvwj.html

Ruby: arr.max;  arr.min
来源：http://hz.pengpengdd.cyou/gtokzuduwt.html

C#:   list.Max();  list.Min()
来源：http://hz.zhiwuduotai.top/gtpvgyrlek.html

[D18] 扁平化嵌套数组
来源：http://hz.birdmap.top/gtlrmxpmjk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtaqokblkq.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gtzznktsfz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinghuilouyu.cn/gtyoxrtyyp.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtawidthgz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yueranfly.top/gtcpqjovck.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtawlozwqz.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtkpgmgeoh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenjidiqi.icu/gteynokshc.html

[D19] 按字段分组
来源：http://hz.cdnleiting.top/gtiovqlkff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.birdmap.top/gtdbyqhtxc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.c1oappe.top/gtwsgtlxtx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guannengcc.top/gtrmhnnkdf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenjidiqi.icu/gtzkkwkkeq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.vqdsnc.cn/gtaxxojmmf.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtpasoavaa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtyjbcdrqd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.svipenyu.cn/gtjgtvnaik.html

[D20] 统计每个元素出现次数
来源：http://hz.nwbrower.top/gtxvjkznto.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtqjgnwojf.html

PHP:  array_count_values($arr);
来源：http://hz.mhx1999.top/gtbmllwofa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gttcsmyumq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtyhbtroed.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sufxvd.cn/gtfnqcnezx.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gtbpiswfos.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gttwibxxul.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtbzsqhxjh.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gtompkzcrz.html

Py:   x in arr
来源：http://hz.tanke756.top/gtuejfyluc.html


<!-- 参考信息 -->