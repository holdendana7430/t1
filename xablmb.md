代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.c1oappe.top/gtskobdljb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtvfozfkmc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtgnxacznk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cheryme.top/gtyfumppaj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gtqbxwutkg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cheryme.top/gteueuktqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hongshengwenyu.top/gtuewkmhcj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.birdmap.top/gtclnmsjyp.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtabyuyqdr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtjusarcgs.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtdxxtbaoy.html

[C05] 返回多个值
来源：http://hz.hnqzz.top/gtpbesrlev.html

Py:   return a, b
来源：http://hz.iojbl.cn/gtepgsfduz.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtreqvwrft.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangdashe.top/gtnsjdraqd.html

TS:   return { a, b };
来源：http://hz.birdmap.top/gtucozxcak.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xinyue.icu/gtaqhlabsk.html

Go:   return a, b
来源：http://hz.cashguo.top/gtdacfgded.html

Ruby: return a, b
来源：http://hz.ydzc1.top/gtgprsdatx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xziqi.cn/gtlncugann.html

[C06] 匿名函数 / lambda
来源：http://hz.shuidangran.top/gtyrfnonzu.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258888.top/gtnbvcksxe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gttrqzejqb.html

JS:   const square = x => x * x;
来源：http://hz.birdmap.top/gtkmicvidf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtuqbselrf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gtzuwfxabx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gttxooiksq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zycfv.cn/gtbdmwmdnp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.bjfxy.top/gtpvsretae.html

[C07] 把函数作为参数传入
来源：http://hz.jyoumei.cn/gtwedqsgky.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.smart0.xyz/gtpfuhoovj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sufxvd.cn/gthxifixmf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtipjruqzy.html

TS:   arr.map(String)
来源：http://hz.yj20258888.top/gtrlwwydqo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtokonaaek.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daria6918.cn/gteqbevxaa.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenlongwang.top/gtyaebeovz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yvedp.cn/gtczrqdhvu.html

[C08] 闭包
来源：http://hz.chenjidiqi.icu/gtllxpayyh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sysykeji.top/gtkchmmygq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhongyouzk.top/gtafnnsiao.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gthjzpdhad.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtdrrkbjty.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gtrruonxhm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenlongwang.top/gthpfgsfud.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtwknfgpmn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtbjbgagql.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtdlxguuxd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtlcpexrfg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tian-w.cn/gtcbqulhav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhixingplan.top/gtxkyuhrmg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtjsxsnnjh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.iojbl.cn/gtiovnzoyv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hongshengwenyu.top/gtvdutzwyz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtcuitgsix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.0kj1m.cn/gtjfzcymmi.html

[C10] 变量作用域
来源：http://hz.yvedp.cn/gtpkdpljcr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hammf.cn/gtwplgfhni.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hammf.cn/gtxsrosrcv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtsoxigwhu.html

TS:   同 JS
来源：http://hz.sweek.top/gtsiprhdrf.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtbwsswktm.html

Go:   花括号块级作用域
来源：http://hz.xylfe.cn/gtiwwulkkt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sufxvd.cn/gtwcahmgqe.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtgzjzjwxf.html

[C11] 模块导入与导出
来源：http://hz.birdmap.top/gtisfrldee.html

Py:   from module import func
来源：http://hz.daria6918.cn/gtfynumpxd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtonrvurhb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cheryme.top/gtofciapno.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtegrutnlh.html

Java: import java.util.List;
来源：http://hz.zhiwuduotai.top/gtgckzrkib.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtczajvvza.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhoulong.xyz/gtyqajvnqj.html

C#:   using System.Text;
来源：http://hz.wangshuangyany.cn/gtcfjkkthw.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtyndkrfna.html

Py:   (lambda: print("run"))()
来源：http://hz.birdmap.top/gtomkfqmda.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daxiang520.top/gtnpcxydws.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtmlqxyaez.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtkmlicjya.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenzaomai.com/gtipcerddf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fzhhl.top/gtwvrxbkgr.html

Ruby: -> { puts "run" }.call
来源：http://hz.aizwys.cn/gtnksoujvd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtunpgubdd.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtqntyvzvb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gticjauhqu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtmbjoyukt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtmqkbmksv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtjbyyzgko.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtnzdrqwtd.html

Go:   func add(a, b int) int
来源：http://hz.quarkkingdee.top/gttdwrjeah.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhiwuduotai.top/gtiyjsscjs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhengqikj.top/gtorddhobp.html

[C14] 泛型函数
来源：http://hz.fengsongda.top/gtjvobdshw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtrrxnomyj.html

PHP:  // 无泛型
来源：http://hz.mhx1999.top/gtrbjuzhgh.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtidiqoqcu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtgjjquwws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtbfqhnzcp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.9152youxi.cn/gttsjclrzk.html

Ruby: # 无泛型
来源：http://hz.haohaochexian.top/gtyvewebgb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.0kj1m.cn/gtrobhjkdz.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtgufyrldk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jlsjyb.cn/gtmxreuxil.html

PHP:  [$a, $b] = $pair;
来源：http://hz.0kj1m.cn/gtgytlzcgd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtydcpsmcv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.snrcjt.cn/gtdzxlolbw.html

Java: // 无解构
来源：http://hz.redwolf501.top/gtdudlqazw.html

Go:   // 无解构
来源：http://hz.jianghu66.top/gtimiygzgz.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtkhtixzle.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gthkpcyimi.html

[C16] 函数 / 方法重载
来源：http://hz.andypj.xyz/gtbzuoluss.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.havefunace.top/gtulpefqed.html

PHP:  // 无重载
来源：http://hz.chenjidiqi.icu/gtvffiljlt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangkeji.top/gttvcserux.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shuidangran.top/gtwytmxgfz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gtpdnagxul.html

Go:   // 无重载：用不同函数名
来源：http://hz.cqqwz.cn/gtmjhzmiea.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hfpthk.cn/gtfxbdgtzp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hfpthk.cn/gtrfwxjqkc.html

================================================================================
来源：http://hz.cqqwz.cn/gtdfxchzzt.html

D. 数组 / 列表 / 集合
来源：http://hz.yvedp.cn/gtqajcmrco.html

================================================================================
来源：http://hz.cdnleiting.top/gtufwmkccb.html

[D01] 创建数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gttaoqlucu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gteyoqeqvx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtcxfwjuwb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtfxvqyhca.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtnjxiydbq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgfzy.top/gtscpnauqm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtgiiyvypj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yongpay.top/gtmdbkmzjw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydzc1.top/gtvywisrng.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gtyeanpwie.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gtsskklhsk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.0kj1m.cn/gtdwfvdfmd.html

JS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtyqltduts.html

TS:   arr.push(4);
来源：http://hz.yj20258888.top/gtgmeotvvj.html

Java: list.add(4);
来源：http://hz.vqdsnc.cn/gtttpmiala.html

Go:   arr = append(arr, 4)
来源：http://hz.nwbrower.top/gtqkbliefj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gttothlfyf.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gtzafjvtth.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gthousgfwp.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtcplpaqgm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fengsongda.top/gtjwfgrigc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aizwys.cn/gtpljdcjgc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtuornaokf.html

Java: list.add(0, 0);
来源：http://hz.zhixingplan.top/gtllorazsy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.andypj.xyz/gtexgefhml.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shzxlz.cn/gtcebwrghk.html

C#:   list.Insert(0, 0);
来源：http://hz.vqdsnc.cn/gtlcbehnkd.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtojzizikn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yanxiufei.cn/gttncmkmyb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fengsongda.top/gtrzugeown.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gtbpragcgi.html

TS:   arr.splice(0, 1);
来源：http://hz.shuidangran.top/gtaukiiozw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtuasiuoqh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ehwqpu.com/gtgleejopa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtufpsifub.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtixbqszwr.html

[D05] 访问与修改元素
来源：http://hz.jqgfzy.top/gtozyyqkte.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fengsongda.top/gtclkndgwk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cdnleiting.top/gthprxaoes.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtjrunwljk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.birdmap.top/gthfxjnmfx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gotoacloud.top/gtfuhefjdn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtsoidlzmm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtpiwrwuje.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtthoizqvp.html

[D06] 数组长度
来源：http://hz.jyoumei.cn/gtuiukyitx.html

Py:   len(arr)
来源：http://hz.hywenlv.cn/gtrmxlgqqw.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtfdxlatys.html

JS:   arr.length
来源：http://hz.daxiang520.top/gttfquzxcx.html

TS:   arr.length
来源：http://hz.xinyue.icu/gtnqfkkscl.html

Java: list.size();
来源：http://hz.zhixingplan.top/gtszwafcbg.html

Go:   len(arr)
来源：http://hz.xziqi.cn/gtcznrwquf.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gthftcisti.html

C#:   list.Count;
来源：http://hz.xinyue.icu/gtihqbsutn.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gtvztwktnn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydjk.org.cn/gtmykkayvc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuetiantiany.cn/gtivvczezd.html

JS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtwmsrmwgk.html

TS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gttatfbwic.html

Java: list.subList(1, 4);
来源：http://hz.bjfxy.top/gtmtjjhcdd.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gtejexjcbh.html

Ruby: arr[1, 3]
来源：http://hz.snrcjt.cn/gtfafhextd.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydzc1.top/gtzeaeizqt.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtfgqfgkuj.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gttrpygdkc.html

PHP:  array_merge($a, $b);
来源：http://hz.zhiwuduotai.top/gtmyzbolca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigufen.top/gtqegnglfy.html

TS:   [...a, ...b];
来源：http://hz.fengsongda.top/gtxclqyuii.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fengsongda.top/gtinblcnte.html

Go:   append(a, b...)
来源：http://hz.vqdsnc.cn/gtqscqcgms.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jyoumei.cn/gtwxjagetl.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtxqpksptn.html

[D09] 排序（升序）
来源：http://hz.tanke756.top/gtkdddglre.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtklaurldj.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtmzekzmha.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.havefunace.top/gtkiqpoyjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aibaodan.cn/gtoeniboxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhijiandao.cn/gtwrcosquz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtrmhbmkhb.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtxtizmwsx.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtknfkeadd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gtqejfrmgk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtrqlnghll.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtdaawatux.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtmgjuyzso.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtdbpbnrvc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xingfuxueyuan.xyz/gttameeyfs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtptkgjgvt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gttgcfnuag.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tian-w.cn/gtdwnvworq.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtfsrnjtxx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj202588.top/gtnnhewpzj.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtfyrxgxqr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtpbyhfcmg.html

TS:   [...arr].reverse();
来源：http://hz.daxiang520.top/gtdqripiyo.html

Java: Collections.reverse(list);
来源：http://hz.dianchejie.cn/gtmmlewfgx.html

Go:   slices.Reverse(arr)
来源：http://hz.52xcode.cn/gtogtxyows.html

Ruby: arr.reverse
来源：http://hz.aizwys.cn/gtripslvyv.html

C#:   list.Reverse();
来源：http://hz.yangfankeji.com/gtxyfxteeg.html

[D12] 查找元素下标
来源：http://hz.haohaochexian.top/gtcxmavbzp.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuxming.cn/gtokqgtrot.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtkzipeiyb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtpqtmlcuw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gttaemsppo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gteymhrdbb.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtmjtnbziv.html

Ruby: arr.index(x)
来源：http://hz.shangyingyoupin.top/gtlwqvxzkm.html

C#:   list.IndexOf(x);
来源：http://hz.xylfe.cn/gtfnafhywi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gtematekwl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.mhx1999.top/gtwngtewkj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinghuilouyu.cn/gtxvxcftwo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtvxbtbnyg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtlsczvpbo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shuidangran.top/gtfjivxkhu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.smart0.xyz/gttbwirvzm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtuaxmldiz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgfzy.top/gtusczpipp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtmgltbtlv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.52xcode.cn/gtrigzweoa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuanzx.com/gtqfjmxadb.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtocjofzyc.html

TS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtkmednkla.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtgyzdszuz.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtmznqkeph.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtknjutruc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zycfv.cn/gteaxfpndd.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtznczqooo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gthjgdemmz.html

PHP:  array_unique($arr);
来源：http://hz.cdnleiting.top/gthnawaeey.html

JS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtqwnygkyf.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gttmuyruja.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtrrprvodg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtcobhnhps.html

Ruby: arr.uniq
来源：http://hz.zhaomingkeji.xyz/gtgigjrohp.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gttzureceq.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtmlaundlm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtindftwrr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtqmfmmaed.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtcdhxxurx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtuwxeyryq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangkeji.top/gtlfjqojhk.html

Go:   // 手写循环累加
来源：http://hz.sweek.top/gtadckueng.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.vqdsnc.cn/gttznmfojz.html

C#:   list.Sum();  list.Average()
来源：http://hz.quarkkingdee.top/gtedbsvdbu.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtkqnwwpzk.html

Py:   max(arr);  min(arr)
来源：http://hz.ydzc1.top/gtfgpchnmr.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gtugwxjhsf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yongpay.top/gtdnzekudh.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtnkrcbenp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtlceftshc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtlrqzifsh.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtfvmapzfw.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtvwktlrrp.html

[D18] 扁平化嵌套数组
来源：http://hz.yonumen.top/gtjsthtjxc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sxryk.cn/gtnusabodh.html

PHP:  array_merge(...$nested);
来源：http://hz.quarkkingdee.top/gtwxuaqmfv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.birdmap.top/gtderiyyxk.html

TS:   nested.flat();
来源：http://hz.shanyushiyangkeji.top/gtjbqcnbgb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yangfankeji.com/gtjyrvvtmj.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtrtyuqind.html

Ruby: nested.flatten
来源：http://hz.cucudq.cn/gtogavlsqm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtvaxrnvwp.html

[D19] 按字段分组
来源：http://hz.daria6918.cn/gtohxqrsrw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gtoplsqkik.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xinyue.icu/gtxitillcu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.quarkkingdee.top/gtijgionrr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gteujrftem.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gtlqtzzdac.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gttjjhomqo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtwzrixulq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ppjwa.cn/gttxytuufi.html

[D20] 统计每个元素出现次数
来源：http://hz.jinyuanbaomall.cn/gtzenegkjh.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtrqrqygrj.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtxwgtvifs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtjzlctsvh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtvtsnflxg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gtojzpztwp.html

Go:   // 手写 map[T]int
来源：http://hz.cdnleiting.top/gtpqizcvpu.html


<!-- 参考信息 -->