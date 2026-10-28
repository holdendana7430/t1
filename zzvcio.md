代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnqzz.top/gtlprumwel.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtszldbvba.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtbhwbcgcb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cashguo.top/gtrrieslfs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gttfysjkak.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtlrxxkhgm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gtbgshlahn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shangyingyoupin.top/gtojfzdvqz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sysykeji.top/gtufobqaeu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtenppvwar.html

[C04] 命名参数 / 关键字参数
来源：http://hz.andypj.xyz/gtukuzsfmf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gthncaysiz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shangyingyoupin.top/gtiefgrbql.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj202588.top/gtgfwrrftw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yueranfly.top/gtnksexzai.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.bjfxy.top/gtpkskieig.html

Go:   // 无：用配置结构体参数
来源：http://hz.xingfuxueyuan.xyz/gtwjvbmdez.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtztzkivgy.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtqqsajsva.html

[C05] 返回多个值
来源：http://hz.sweek.top/gtuuhorvrm.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtyvbzsfei.html

PHP:  return [$a, $b];
来源：http://hz.gotoacloud.top/gtpdkjekho.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangshuangyany.cn/gtwhazuocb.html

TS:   return { a, b };
来源：http://hz.hywenlv.cn/gtnvzyfgam.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnxiangtu.top/gtlanpkmxz.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtjropaqeu.html

Ruby: return a, b
来源：http://hz.sxryk.cn/gtlewccasa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xylfe.cn/gthojrtozd.html

[C06] 匿名函数 / lambda
来源：http://hz.hammf.cn/gtytqvnbpt.html

Py:   square = lambda x: x * x
来源：http://hz.jinyuanbaomall.cn/gtpuvscpak.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.mhx1999.top/gterwcncnj.html

JS:   const square = x => x * x;
来源：http://hz.zhongyouzk.top/gtvqdozslh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gtjasucnmc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydjk.org.cn/gtzwnwwehb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pycfn.com/gtueagvjvg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.vqdsnc.cn/gtmnqecces.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.birdmap.top/gtrslfwmzz.html

[C07] 把函数作为参数传入
来源：http://hz.yuxming.cn/gtddwrylep.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gthqpsdsyx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aizwys.cn/gtfskamcdz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xinyue.icu/gtqtzedgkv.html

TS:   arr.map(String)
来源：http://hz.iojbl.cn/gtxdvgxeny.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pengpengdd.cyou/gtollwtfpt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtyamyzpoc.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtqxsuoqau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj202588.top/gttvdwcvoj.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtikhocntk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtepbquzeb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxinkj.top/gtvrevpnxd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gttcykynry.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtjzdkbjhl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gtnrulwcfj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinyuanbaomall.cn/gtnzkwxdmw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.mhx1999.top/gtfembxqyx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtvienqwlu.html

[C09] 递归
来源：http://hz.yuanzhike.top/gtjvdwbwmm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gthhzofjyv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.iojbl.cn/gtbcgeafzm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtxdijpkyi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtqauxrdem.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtusfqykuo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtxaszaqso.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nanxinkj.top/gtkwunoluh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.52xcode.cn/gtvczkegki.html

[C10] 变量作用域
来源：http://hz.meibo888.top/gtppnfkmix.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hnxiangtu.top/gtfmviuchn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gtcwnkibwl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtmsvwpiym.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtrojjgdjz.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gthnrftkqh.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtbrqwrafb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xylfe.cn/gtlbnkjauf.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtkvgjchtc.html

[C11] 模块导入与导出
来源：http://hz.sxryk.cn/gtsyovudrj.html

Py:   from module import func
来源：http://hz.gzhubu.top/gtgvicuvyo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.316326.xyz/gtlcbukkgo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtngouomsy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hysaishi.cn/gtozfesklr.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gtswdnfnlg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gotoacloud.top/gtoyrinroz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhiwuduotai.top/gtjnyirzgw.html

C#:   using System.Text;
来源：http://hz.meibo888.top/gtlpsvneru.html

[C12] 立即执行函数 IIFE
来源：http://hz.hywenlv.cn/gtstrksztb.html

Py:   (lambda: print("run"))()
来源：http://hz.guannengcc.top/gtejuetqpm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ehwqpu.com/gtilzkjrtd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtzwkijmsz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtlreimvsd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgufenzy.top/gtewtmhbik.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xylfe.cn/gtsksbiapo.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtkygkcafd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtqjcrnoow.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtatxdyvzr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtdwqxwwjm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtjdklceps.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.316326.xyz/gtuyzrowbl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtwmwdatba.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtbvxccqdu.html

Go:   func add(a, b int) int
来源：http://hz.andypj.xyz/gtupbvxliv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zdqjudy.top/gtsscdymle.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtwezagozz.html

[C14] 泛型函数
来源：http://hz.yuanzhike.top/gtdtrkrfry.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangshuangyany.cn/gtzbadsfgy.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gtrhmicoqm.html

JS:   // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtgppdcqrq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhiwuduotai.top/gtmlcmxjsb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fzhhl.top/gteiprnyjb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhixingplan.top/gtcjwkyujd.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtukbkjqtt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxinkj.top/gtnqqxtibv.html

[C15] 解构 / 展开参数
来源：http://hz.zhijiandao.cn/gtdhvovfoj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.52xcode.cn/gtknoryltu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtbxvrnren.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtigbizlqp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gteckwomll.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtetzgylij.html

Go:   // 无解构
来源：http://hz.tian-w.cn/gtqpbgymji.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtdzwpanni.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gtbxmmawzi.html

[C16] 函数 / 方法重载
来源：http://hz.ybcxt.top/gthioydbxj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.c1oappe.top/gtpeyoayft.html

PHP:  // 无重载
来源：http://hz.yanxiufei.cn/gtokboudlb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.smart0.xyz/gtqqhkllmx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jyoumei.cn/gtcerbchjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtctugcijk.html

Go:   // 无重载：用不同函数名
来源：http://hz.zycfv.cn/gtgludbivy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ivvv.top/gtbyrwwcvr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sxryk.cn/gtpkqfkjcu.html

================================================================================
来源：http://hz.yueranfly.top/gtcesyidew.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtycvdslka.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcatmxscd.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtljysrhte.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigufen.top/gtidqifsgk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinyuanbaomall.cn/gtbuiqpgsp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.9152youxi.cn/gthyzekkjp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.snrcjt.cn/gtwmpryjte.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pengpengdd.cyou/gtdgvhiuum.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yueranfly.top/gtqjrmcuej.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gtbndmmmsn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtrgknehfi.html

[D02] 追加元素到末尾
来源：http://hz.tanke756.top/gtvkcgxccx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aibaodan.cn/gtmfuqcslb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.mhx1999.top/gtzgfjldds.html

JS:   arr.push(4);
来源：http://hz.tanke756.top/gtdfjyhezl.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gtnqvjbuvp.html

Java: list.add(4);
来源：http://hz.yongpay.top/gtgovepruw.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtktxsiyxo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydzc1.top/gtrxddlunp.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtvbvovldd.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtonttgyzo.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtolpyxwnl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258888.top/gtkgmmulvo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhaomingkeji.xyz/gtjtjmgdpx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.svipenyu.cn/gtwzuxiirj.html

Java: list.add(0, 0);
来源：http://hz.jqgfzy.top/gtihfwzjli.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dashuyun.cn/gtjhajcyxa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtgoiqehax.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtoimdwjfu.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtmynitvqi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shuidangran.top/gtwmynfspv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guowangkeji.top/gtpkbwlfgz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhiwuduotai.top/gtpsgkrgka.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gtczbamcyz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.meibo888.top/gttvvkkfsh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.meibo888.top/gtjgfkousa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtyrpwqjxk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtegiiphvr.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gtnpqvaaci.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtwypcybwt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtmfkvhxwg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhongyouzk.top/gtskcmhlmg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhoulong.xyz/gtefjlbzpz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cheryme.top/gtlqozocff.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daxiang520.top/gtzewpaqks.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtmxnjnemi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtgqqgcdns.html

[D06] 数组长度
来源：http://hz.cheryme.top/gtugdgbxyi.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtwisvdvnu.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtkeacyolz.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtfqkygobg.html

TS:   arr.length
来源：http://hz.tian-w.cn/gtapxudsmz.html

Java: list.size();
来源：http://hz.jqgufenzy.top/gtcgoovfya.html

Go:   len(arr)
来源：http://hz.svipenyu.cn/gthhfduusv.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtpbazjsoe.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gthekbshmf.html

[D07] 切片 / 取子数组
来源：http://hz.sysykeji.top/gtqbcuzmry.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gtaonfvlfd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tian-w.cn/gttgoizkjd.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gttbxasoai.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtgytrzxxr.html

Java: list.subList(1, 4);
来源：http://hz.vqdsnc.cn/gtxeoztxie.html

Go:   arr[1:4]
来源：http://hz.gaohongyu789.top/gttbdjwmuk.html

Ruby: arr[1, 3]
来源：http://hz.sweek.top/gtjkeugoul.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gtjjrfcvch.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtzhnahfke.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gtgewhgxuu.html

PHP:  array_merge($a, $b);
来源：http://hz.ivvv.top/gtxepdapqe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guannengcc.top/gtfcrhupjk.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtbzdtmxso.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sysykeji.top/gtigjabyaz.html

Go:   append(a, b...)
来源：http://hz.yvedp.cn/gtwocpkysx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtnscaztww.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtatpwigcc.html

[D09] 排序（升序）
来源：http://hz.fzhhl.top/gtbzvbvzdr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtxjsdymch.html

PHP:  sort($arr);
来源：http://hz.gogol.net.cn/gtmffqanjy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.9152youxi.cn/gtktwycwfg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gthphmvdue.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtedcvbdlh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtgftobouj.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtrgpgubjg.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtjukkxzqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhengqikj.top/gtpbccacyo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pycfn.com/gtkdabeomo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gotoacloud.top/gtziejlbrj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtdrqeohgr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jlsjyb.cn/gtoghpvjgm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sxryk.cn/gtifvuxlbt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gaohongyu789.top/gtwvhnyfny.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.svipenyu.cn/gtrcmavzcn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aizwys.cn/gtmcrcjnje.html

[D11] 反转数组
来源：http://hz.zhongyouzk.top/gtqryexjww.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guannengcc.top/gtobacseqk.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gtgympkkar.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gotoacloud.top/gtsuedcndh.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtduocsxpd.html

Java: Collections.reverse(list);
来源：http://hz.ehwqpu.com/gtqhhgxdby.html

Go:   slices.Reverse(arr)
来源：http://hz.c1oappe.top/gtnzdtogdy.html

Ruby: arr.reverse
来源：http://hz.havefunace.top/gttpjfuvss.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtlykwpklb.html

[D12] 查找元素下标
来源：http://hz.ywan-chungtsiang.top/gtpxfpvcei.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtguckbpew.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtrcsubyby.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtilyxctfz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtlhchkldd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cucudq.cn/gtnheqzogf.html

Go:   slices.Index(arr, x)
来源：http://hz.fzhhl.top/gtmfoqcbnl.html

Ruby: arr.index(x)
来源：http://hz.redwolf501.top/gtytevohvn.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtcwgxmdek.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gtvthuuvmn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtpxshwxxu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtnsowozjp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtdkxuglae.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtbilhiwwb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yvedp.cn/gtjdfouatm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gtkoieiess.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.andypj.xyz/gtohlqfzxk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxuanxn.top/gtmecasjrh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtptauqsiq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtdqlsqfmz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj202588.top/gtnixwpfym.html

JS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtzdkmxsth.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtprbpyyof.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yangfankeji.com/gtayfumwrv.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtsyiihisx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.andypj.xyz/gtalfiatyf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtidjxhtgh.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtosvvmmyw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtxjldjmll.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtsypsfijn.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtxahwgybt.html

TS:   [...new Set(arr)]
来源：http://hz.guowangkeji.top/gtzaixcbnk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtgkgwzgub.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.mhx1999.top/gtdkjahgyj.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtxgqpeozc.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtwcznmmxe.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtuxoziiqt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jlsjyb.cn/gtcwnenfbo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtcweafkax.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtnfoegkmv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtagkjwguj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtjyskirll.html

Go:   // 手写循环累加
来源：http://hz.xziqi.cn/gtkuvjtijo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gtladejevj.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtgglydcqp.html

[D17] 最大值与最小值
来源：http://hz.aibaodan.cn/gtbmowzill.html

Py:   max(arr);  min(arr)
来源：http://hz.hongshengwenyu.top/gtqyrwzich.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtduqlgrtj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtlqewncie.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtziohvttq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ybcxt.top/gtultpdmzr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtkodharwt.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtxfbdxvza.html

C#:   list.Max();  list.Min()
来源：http://hz.zhijiandao.cn/gtwkioacdv.html

[D18] 扁平化嵌套数组
来源：http://hz.xingfuxueyuan.xyz/gthbsfzssm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yanxiufei.cn/gtjkprxhrn.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258.top/gtfdetlrwf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtuhwkzynt.html

TS:   nested.flat();
来源：http://hz.ivvv.top/gtphcvhyei.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnxiangtu.top/gtmfegkkmc.html

Go:   // 手写双层循环
来源：http://hz.zhijiandao.cn/gtjqyiiuxd.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtsmoodpwh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtfclqsfzd.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtuolpopuy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenlongwang.top/gtliyplfia.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtzdhgtjnx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtbazqrtvu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtnehqcscs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtnylhwzxp.html

Go:   // 手写 map[string][]T
来源：http://hz.quarkkingdee.top/gtmdsxstld.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.vqdsnc.cn/gtuwzfycbf.html


<!-- 参考信息 -->