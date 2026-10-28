代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258.top/gtlfxnxouf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hysaishi.cn/gtorjqyrsi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtyycwqhly.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cqqwz.cn/gtmjxeufnz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gtdzjzctqo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtnsfsmqem.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhengqikj.top/gtisfqgnno.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shuidangran.top/gtbhbbycop.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydzc1.top/gtuvvpcyjn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtfveauvqt.html

C#:   f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtpnfuzhqi.html

[C05] 返回多个值
来源：http://hz.yj20258.top/gtbryylnkx.html

Py:   return a, b
来源：http://hz.jiagoushi.top/gtgvahpmcp.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtwtuszomo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxinkj.top/gtkfmqcqrg.html

TS:   return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtjggacgac.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hongshengwenyu.top/gtdwzaofdn.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtejgjrqef.html

Ruby: return a, b
来源：http://hz.shanyushiyangtech.top/gtwjyftksu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigufen.top/gtxyktylvl.html

[C06] 匿名函数 / lambda
来源：http://hz.daria6918.cn/gtioffdecm.html

Py:   square = lambda x: x * x
来源：http://hz.316326.xyz/gtdcfuwrmf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtgbgumvpm.html

JS:   const square = x => x * x;
来源：http://hz.xinyue.icu/gtizgqhdvt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fzhhl.top/gtdcdzpvnd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtcvbfbxsq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.bjfxy.top/gtuzlqzrli.html

Ruby: square = ->(x) { x * x }
来源：http://hz.316326.xyz/gtsmmlanvu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuanzx.com/gtdkijggnc.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtkpozhngc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daxiang520.top/gtlfcdagmt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.andypj.xyz/gtwzjseofe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daria6918.cn/gtomipyekl.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtbtfhgegd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtcmloqwwk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yanxiufei.cn/gtnqewfuek.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gttvaorrbu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shangyingyoupin.top/gtraqdgtff.html

[C08] 闭包
来源：http://hz.0kj1m.cn/gtgpqwlrky.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtjkhinynj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aibaodan.cn/gtzxblmtmx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtcqzpaqci.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtgeyjnfhf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hywenlv.cn/gtwujsxdyl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gogol.net.cn/gtgkpfqeqf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gzhubu.top/gtcjwrwgkp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtyugqvkys.html

[C09] 递归
来源：http://hz.jlsjyb.cn/gtnubmjcqi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuanzx.com/gtodxjxnme.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shanyushiyangtech.top/gtjafhzygz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fengsongda.top/gtdvwsnfdm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtikpyrhnw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cashguo.top/gtcpajbdgn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258888.top/gtawlyqccv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtkgidcidi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtpxfcpsqg.html

[C10] 变量作用域
来源：http://hz.gogol.net.cn/gtwnzoujym.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.wangdashe.top/gtrrghohpw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gtkusnaybz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gtmfgqfaph.html

TS:   同 JS
来源：http://hz.pycfn.com/gtmvzfnabh.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtuffrwvbl.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtuskzukta.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtaufrtasu.html

C#:   块级作用域
来源：http://hz.shanyushiyangkeji.top/gtwedpyccu.html

[C11] 模块导入与导出
来源：http://hz.jinyuanbaomall.cn/gtgscecxio.html

Py:   from module import func
来源：http://hz.ywan-chungtsiang.top/gtjkzgokee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgufenzy.top/gtblarfxzp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtheawlmti.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gteybndfjl.html

Java: import java.util.List;
来源：http://hz.yj20258.top/gtsjquwpjz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.snrcjt.cn/gtuusclefu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtogdyzmly.html

C#:   using System.Text;
来源：http://hz.mhx1999.top/gtlgynsnfo.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuetiantiany.cn/gtiwvzkjyh.html

Py:   (lambda: print("run"))()
来源：http://hz.shzxlz.cn/gtujkiphfm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shzxlz.cn/gthcrygezr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtaiqdsrjd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtizlfltlk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ivvv.top/gtkxcgnbgi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yanxiufei.cn/gtvagguzsr.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhaomingkeji.xyz/gtwptuivpp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shzxlz.cn/gthkppldla.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuanzx.com/gtubtijnwp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtbhxousps.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtlxvhqxnj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gttyjquuho.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtxzlonsgc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtcjzlhtzg.html

Go:   func add(a, b int) int
来源：http://hz.daria6918.cn/gtfajjmpue.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhengqikj.top/gtdfjmlwji.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtdzyfedxs.html

[C14] 泛型函数
来源：http://hz.pengpengdd.cyou/gtjjaxbzjy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hywenlv.cn/gtklmqkzpm.html

PHP:  // 无泛型
来源：http://hz.yvedp.cn/gtaftuoidy.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gtupnxmovv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtorwlppnm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gaohongyu789.top/gthitqmteg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhongyouzk.top/gtcqelwevf.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtijiudfgb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ppjwa.cn/gtdlbdcybo.html

[C15] 解构 / 展开参数
来源：http://hz.daria6918.cn/gticxaufws.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gttnitcwoz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.meibo888.top/gtwgckpwdh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yongpay.top/gtpowwacaj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj202588.top/gtmtihwblu.html

Java: // 无解构
来源：http://hz.sweek.top/gtunwgzpsi.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtfmuujrua.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtozubcgmo.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtaoyogpcp.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtovdwvqdr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.haohaochexian.top/gtusnnaxhc.html

PHP:  // 无重载
来源：http://hz.jinghuilouyu.cn/gtpkhmdguh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xylfe.cn/gtzidbewby.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtcvrwpwdl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangkeji.top/gtnjajemsn.html

Go:   // 无重载：用不同函数名
来源：http://hz.zycfv.cn/gtrnnmriif.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtkftjrycn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenlongwang.top/gttlcfdxwl.html

================================================================================
来源：http://hz.gotoacloud.top/gttvgbwcsq.html

D. 数组 / 列表 / 集合
来源：http://hz.quarkkingdee.top/gtbcpxrdmw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcjmjbbzl.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtzxhyqcdk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gogol.net.cn/gtawaesvzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hammf.cn/gtjzxfgksx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shuidangran.top/gtkxdqunrz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.quarkkingdee.top/gtesjxnagr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gthriotuab.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gotoacloud.top/gtuuopophc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtuqegxdeo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtannkagmz.html

[D02] 追加元素到末尾
来源：http://hz.gotoacloud.top/gtqqzkbhle.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xylfe.cn/gtwkmbtmyb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gtzdvlumvv.html

JS:   arr.push(4);
来源：http://hz.andypj.xyz/gtvugimuuj.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtfrmvepyd.html

Java: list.add(4);
来源：http://hz.xziqi.cn/gtzabemdeu.html

Go:   arr = append(arr, 4)
来源：http://hz.wangshuangyany.cn/gtffnwmlpg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.redwolf501.top/gtbaqccahb.html

C#:   list.Add(4);
来源：http://hz.cheryme.top/gtldccnfzt.html

[D03] 在指定位置插入元素
来源：http://hz.jlsjyb.cn/gtinmxfcae.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtausvzwys.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhaomingkeji.xyz/gtijmkwbcb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hongshengwenyu.top/gtobfyisny.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gtwzmmuwug.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtqppmurxa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhixingplan.top/gtvekvzpvt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gtvfpmdrps.html

C#:   list.Insert(0, 0);
来源：http://hz.cucudq.cn/gtcusdohag.html

[D04] 删除元素
来源：http://hz.cashguo.top/gtpuzsjjxo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgfzy.top/gtxinxtgri.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.0kj1m.cn/gtvhcrjjbh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangkeji.top/gtflnvkbzj.html

TS:   arr.splice(0, 1);
来源：http://hz.guannengcc.top/gtllhceufy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtpvlkmhwn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gogol.net.cn/gtoicquayb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtarhyoknb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtwxukgxoi.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gtxrmhqvid.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtfbphbono.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ybcxt.top/gtijghvxjo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtvnlcaeno.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.c1oappe.top/gthbgrqoaa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtvoczgfpd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tian-w.cn/gtetsehsrc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gthknvthka.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.vqdsnc.cn/gtcqfkgnak.html

[D06] 数组长度
来源：http://hz.iojbl.cn/gtwylawfje.html

Py:   len(arr)
来源：http://hz.9152youxi.cn/gtxwijirnn.html

PHP:  count($arr);
来源：http://hz.xziqi.cn/gtlbvoonrz.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtgjmvgfgy.html

TS:   arr.length
来源：http://hz.daxiang520.top/gtbxrbqvcn.html

Java: list.size();
来源：http://hz.kuanghao11.cn/gtlbeqeqta.html

Go:   len(arr)
来源：http://hz.zhijiandao.cn/gtxntljbbm.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gtpgmmjkzk.html

C#:   list.Count;
来源：http://hz.jyoumei.cn/gtfhehukrb.html

[D07] 切片 / 取子数组
来源：http://hz.ydzc1.top/gtquctibaq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtqipjxcbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tianlin.xyz/gtrtdnihbv.html

JS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gtlemvjybe.html

TS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtpaslkdsl.html

Java: list.subList(1, 4);
来源：http://hz.havefunace.top/gtexxrnxtr.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gttnnmpgii.html

Ruby: arr[1, 3]
来源：http://hz.gogol.net.cn/gtzkapofag.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtnnaotumo.html

[D08] 合并两个数组
来源：http://hz.hnqzz.top/gtxsrubabb.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gtvqtpcnqd.html

PHP:  array_merge($a, $b);
来源：http://hz.cheryme.top/gtjtqzhjpr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.mhx1999.top/gtwoxhvhsg.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtnqdnowzf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.bjfxy.top/gtkfyrxupt.html

Go:   append(a, b...)
来源：http://hz.pycfn.com/gtblxceide.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuanzx.com/gttpbadtwi.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtrslyjpcn.html

[D09] 排序（升序）
来源：http://hz.c1oappe.top/gtelhgbovv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtydcdszzp.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gtznshawcc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ppjwa.cn/gtbhlmilxt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtnqrrbmoo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aizwys.cn/gthocpibea.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtpipafudx.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtbegmefps.html

C#:   list.Sort();
来源：http://hz.vqdsnc.cn/gtgwbobxdm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.redwolf501.top/gtzunlidis.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hysaishi.cn/gtgbrgdwqa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtmxmomnyq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtwkaxxkls.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtjfqqfgln.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aibaodan.cn/gtfipxvraz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hysaishi.cn/gtxakplsbm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guowangkeji.top/gtmigxoqia.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hammf.cn/gtwocombpp.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gttmwudkvf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtwfxadbhi.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtvzztcezb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.andypj.xyz/gtpkyfrkec.html

TS:   [...arr].reverse();
来源：http://hz.ehwqpu.com/gtvreqsfdi.html

Java: Collections.reverse(list);
来源：http://hz.meibo888.top/gtggnmhcur.html

Go:   slices.Reverse(arr)
来源：http://hz.dashuyun.cn/gtwqlqussi.html

Ruby: arr.reverse
来源：http://hz.jqgufenzy.top/gtyidmixtv.html

C#:   list.Reverse();
来源：http://hz.xingfuxueyuan.xyz/gthgvqbcnv.html

[D12] 查找元素下标
来源：http://hz.gzhubu.top/gtmwjpqmms.html

Py:   arr.index(x);  x in arr
来源：http://hz.daxiang520.top/gtilakfrdq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gtkxytjhzv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtocmzpzyx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtwuashfku.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.haohaochexian.top/gtcppglpbt.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtrktbvlkv.html

Ruby: arr.index(x)
来源：http://hz.quarkkingdee.top/gtsbxtpemi.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtuwebvohd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtfktsjubb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hammf.cn/gtnzajfuep.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtfsyscrpc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtuauqanqb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtxqwvewrj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtvdpyotws.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgfzy.top/gtqjpilhxi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gtciehzljf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtgzyzflau.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yanxiufei.cn/gtoodnqbmq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtjmwkbnhp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtslznegia.html

JS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtdlkasffh.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtcpcdpacj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sysykeji.top/gtriupcivq.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtsmmvugyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aizwys.cn/gtohflusxc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hfpthk.cn/gtnzphhusi.html

[D15] 去重
来源：http://hz.52xcode.cn/gtfurmjxsd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtaeabyjvw.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtlbqbebvp.html

JS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtwvbsysnc.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtytjtmcxp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ehwqpu.com/gtorhqrwpz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtwbrwyfjc.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtzrjzcedv.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gttwrmjysw.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtupkxivpx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gthduhmkeh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtgtkoxniv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtbtgpztqb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtpyusjedq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtzrrxddpj.html

Go:   // 手写循环累加
来源：http://hz.haohaochexian.top/gtjvoweujl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtcvbjfkcx.html

C#:   list.Sum();  list.Average()
来源：http://hz.ehwqpu.com/gthzterbbu.html

[D17] 最大值与最小值
来源：http://hz.snrcjt.cn/gtcsdopvji.html

Py:   max(arr);  min(arr)
来源：http://hz.zhengqikj.top/gtexpqcaqx.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtvyamofwb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gtjhozymth.html

TS:   Math.max(...arr);
来源：http://hz.svipenyu.cn/gtijowfrjn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yangfankeji.com/gttqzsahcl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gogol.net.cn/gtfzorcadg.html

Ruby: arr.max;  arr.min
来源：http://hz.0kj1m.cn/gtdneemwki.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtrljikzfm.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtravaseds.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinyuanbaomall.cn/gtvgsxoipa.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtebjdzphl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtuenwsspe.html

TS:   nested.flat();
来源：http://hz.zycfv.cn/gttucaaxgk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtngtdfuwa.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtqvlidrui.html

Ruby: nested.flatten
来源：http://hz.cqqwz.cn/gtmyfzxjld.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yvedp.cn/gtunoihtpt.html

[D19] 按字段分组
来源：http://hz.hnqzz.top/gtqqzagjvm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenlongwang.top/gtbjkfvszw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gttvccqtjx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtwmqyuovu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtxtgcygjw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtsxarwvcj.html

Go:   // 手写 map[string][]T
来源：http://hz.cqqwz.cn/gtfwrjfgji.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hfpthk.cn/gtfbfavezn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.0kj1m.cn/gtzgdrsxpd.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gthttykkbz.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtlpwkaklm.html

PHP:  array_count_values($arr);
来源：http://hz.52xcode.cn/gtuwsnvbgm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtvgzkqcpi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtwlvclikl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ywan-chungtsiang.top/gtkzoxixjm.html

Go:   // 手写 map[T]int
来源：http://hz.zhoulong.xyz/gtbfxphzfm.html


<!-- 参考信息 -->