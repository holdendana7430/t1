代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtqaavcfmz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fengsongda.top/gtgmrtlzed.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtjnzqxhvc.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtzwsopmnk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dianchejie.cn/gtaeounior.html

[C03] 可变参数
来源：http://hz.jianghu66.top/gtfnklcpef.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtapvjwsru.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.svipenyu.cn/gtyjpduoor.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtfxafnybb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtwlgvlgat.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tanke756.top/gttamizfwp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtviqrtcvn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hysaishi.cn/gtuxiqugne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtiexykeyg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cashguo.top/gtisgsenhg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hysaishi.cn/gtxtgdzggr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tanke756.top/gtjzywopil.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtgmcemqtx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangkeji.top/gtnlvryfuj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinyuanbaomall.cn/gtfrlryjdr.html

Go:   // 无：用配置结构体参数
来源：http://hz.daxiang520.top/gtuvrbyxqz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtawuwoonb.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtbexwtgaw.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtgzdctyve.html

Py:   return a, b
来源：http://hz.yj202588.top/gtgibxnoaw.html

PHP:  return [$a, $b];
来源：http://hz.feifeiyinyue.top/gtatdwymuh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ybcxt.top/gtwkvpzpss.html

TS:   return { a, b };
来源：http://hz.nanxuanxn.top/gthpzzzlhk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cqqwz.cn/gtnzmtqzmo.html

Go:   return a, b
来源：http://hz.yuxming.cn/gtpaymgydw.html

Ruby: return a, b
来源：http://hz.andypj.xyz/gttinlvios.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gthdythrdd.html

[C06] 匿名函数 / lambda
来源：http://hz.yuxming.cn/gtshvhprot.html

Py:   square = lambda x: x * x
来源：http://hz.xuetiantiany.cn/gtcuuflrvt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yongpay.top/gtryswrcsw.html

JS:   const square = x => x * x;
来源：http://hz.cashguo.top/gtvlwzxmkq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xziqi.cn/gtnxliubvx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtujkticcy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuetiantiany.cn/gtnwvvgbsy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gtfjaxaihi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtvwrzdduc.html

[C07] 把函数作为参数传入
来源：http://hz.guowangkeji.top/gtqowitepj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinyuanbaomall.cn/gtksjtujsr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yanxiufei.cn/gtyifltnma.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xingfuxueyuan.xyz/gtxgtodfjn.html

TS:   arr.map(String)
来源：http://hz.cucudq.cn/gtdhaspbfx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shuidangran.top/gtooibdfjf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guowangkeji.top/gtynywjygj.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinqigfzy.top/gtrvrbduow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtzxsaxxzs.html

[C08] 闭包
来源：http://hz.jiagoushi.top/gtmetgozpn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sysykeji.top/gthbfcgjuw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.bjfxy.top/gtibonjher.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gttdsltqge.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtecdifoce.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.316326.xyz/gtbiuyfjgt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ehwqpu.com/gtjwzavnwl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.52xcode.cn/gttiqiddvn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtfeguhkew.html

[C09] 递归
来源：http://hz.xylfe.cn/gtlzbrohnw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtyqxlvhhi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.quarkkingdee.top/gtfvmlgoyq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtjcbllwto.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtbkofxhpf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtaqngegxm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shzxlz.cn/gtlvkyautf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtbrvwqbfi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtcrkxkyal.html

[C10] 变量作用域
来源：http://hz.shanyushiyangkeji.top/gtlsbcknhn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fzhhl.top/gtkucuvucu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtlozdfmdl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ehwqpu.com/gtxypskvsd.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtsitetwvb.html

Java: 方法内为块级作用域
来源：http://hz.andypj.xyz/gtygotwllx.html

Go:   花括号块级作用域
来源：http://hz.52xcode.cn/gtcvdhhcao.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gtczvvzuso.html

C#:   块级作用域
来源：http://hz.meibo888.top/gtvofwtrgt.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gteqbawgbf.html

Py:   from module import func
来源：http://hz.tanke756.top/gtfywjcklc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258888.top/gtxmcfmkwk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhengqikj.top/gtldrgagij.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gttgdqqnto.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gtavkusveh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigufen.top/gtuykgmpdo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gtuedvufaq.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtdteverjc.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtpsnmyygy.html

Py:   (lambda: print("run"))()
来源：http://hz.wangshuangyany.cn/gtwwxjtguh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtffvaapkq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtsrdbyipc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtrtbhkpui.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtehtuzhoz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtggdgjqpc.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtawebzxvu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aibaodan.cn/gtuajpcliz.html

[C13] 类型声明 / 类型注解
来源：http://hz.hysaishi.cn/gteyskvhkw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtwgpainrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtmwubsnkg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtqggpawsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtkkzszyhq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtuwocfhbq.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtosggoxvl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxuanxn.top/gtgilgohqy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gtvxmpqxfi.html

[C14] 泛型函数
来源：http://hz.hywenlv.cn/gtffgpzdbq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.52xcode.cn/gtezukrbng.html

PHP:  // 无泛型
来源：http://hz.tian-w.cn/gtrpebzals.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtxkmqiebn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.bjfxy.top/gtwhlbdfbr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nwbrower.top/gtyksqjgzu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cqqwz.cn/gtqtbkoqat.html

Ruby: # 无泛型
来源：http://hz.yuxming.cn/gtuzfggsna.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xylfe.cn/gtlxhrsiaj.html

[C15] 解构 / 展开参数
来源：http://hz.quarkkingdee.top/gthldinlls.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.meibo888.top/gttpnnlown.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtnfesmssc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sweek.top/gtgqvrbrll.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.vqdsnc.cn/gtbfzlsgun.html

Java: // 无解构
来源：http://hz.hfpthk.cn/gtbqflkoja.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtjsqhthkd.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gtakkhqtka.html

C#:   var (a, b) = pair;
来源：http://hz.hongshengwenyu.top/gtbxuxtprp.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtlnvacvqy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yueranfly.top/gttzdfbksh.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtslnthhye.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtrgpgmpbk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtssoqnszz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nwbrower.top/gtkamwsylm.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtgnowzaha.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yonumen.top/gtelgikvny.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fengsongda.top/gtzaeaciij.html

================================================================================
来源：http://hz.ybcxt.top/gtjsfepjol.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtqddubrss.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjfgzluxv.html

[D01] 创建数组 / 列表
来源：http://hz.cdnleiting.top/gthsbrufee.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gotoacloud.top/gtozkkhzfw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuanzx.com/gtpjugtgkd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.birdmap.top/gtsbgmlaqd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtzpupwvno.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.snrcjt.cn/gtxakabaov.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guowangkeji.top/gtrajswmgq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gogol.net.cn/gtwrclnpxs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhaomingkeji.xyz/gtytyomeqh.html

[D02] 追加元素到末尾
来源：http://hz.9152youxi.cn/gtzslaapze.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pengpengdd.cyou/gtxzvwxfbc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtzlyxbuwv.html

JS:   arr.push(4);
来源：http://hz.yj20258.top/gtlxvlpjjt.html

TS:   arr.push(4);
来源：http://hz.sxryk.cn/gtminzzhpt.html

Java: list.add(4);
来源：http://hz.ywan-chungtsiang.top/gtvhulthiu.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtldplnjbi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtcgmzpbfs.html

C#:   list.Add(4);
来源：http://hz.jlsjyb.cn/gtiedbuqtp.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gteonaczol.html

Py:   arr.insert(0, 0)
来源：http://hz.ydzc1.top/gtsjjgwnoy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhengqikj.top/gtjtnlsqmg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fzhhl.top/gtlvmyljvg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuxming.cn/gtkneerkyc.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtdsazmfmo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dashuyun.cn/gtexvydoar.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yonumen.top/gtixtvokmo.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtblpssapk.html

[D04] 删除元素
来源：http://hz.meibo888.top/gtzmkofwpm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gthkxpgvfz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gttmmidrnv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gteqwrnbtp.html

TS:   arr.splice(0, 1);
来源：http://hz.dashuyun.cn/gtizupesdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinyuanbaomall.cn/gtkoucmwdm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yonumen.top/gtdqovdzor.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtksoquaoh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtjnvcodlm.html

[D05] 访问与修改元素
来源：http://hz.cashguo.top/gtnravhvbr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtplljoqol.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gogol.net.cn/gtackvuvfp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dashuyun.cn/gthcjhshyg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhongyouzk.top/gtfxmaeudr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydzc1.top/gtcodfqemh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtzswtymzn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtvgksxlbs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj202588.top/gtugspvimz.html

[D06] 数组长度
来源：http://hz.daria6918.cn/gthijohtke.html

Py:   len(arr)
来源：http://hz.gaohongyu789.top/gtrnsimsjr.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtmiqdfwys.html

JS:   arr.length
来源：http://hz.cashguo.top/gtjmzeaupm.html

TS:   arr.length
来源：http://hz.wangdashe.top/gtuobxamxh.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtnsakbwmf.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtlaknisat.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtqgfzxyvr.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtdeeywzgp.html

[D07] 切片 / 取子数组
来源：http://hz.ydzc1.top/gtckavgoqz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtscpiwnir.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daxiang520.top/gtgikwncph.html

JS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtvzwduvbf.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtoeivrwdj.html

Java: list.subList(1, 4);
来源：http://hz.gogol.net.cn/gtysqdxlzk.html

Go:   arr[1:4]
来源：http://hz.gaohongyu789.top/gtdapufead.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gttyvnomab.html

C#:   list.GetRange(1, 3);
来源：http://hz.sysykeji.top/gtzeauoghv.html

[D08] 合并两个数组
来源：http://hz.zhoulong.xyz/gtfddhblon.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtilwhapdh.html

PHP:  array_merge($a, $b);
来源：http://hz.chenlongwang.top/gtcmgdixpp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtgxrlvnpg.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gteygkbfjt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgfzy.top/gthjdplfqp.html

Go:   append(a, b...)
来源：http://hz.sufxvd.cn/gtxfwrkpag.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtfxbbiypr.html

C#:   a.Concat(b).ToList()
来源：http://hz.dashuyun.cn/gtbgrbrfno.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtpdzrwdnb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtiaxcdvhc.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangkeji.top/gtwrncduwj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fzhhl.top/gtmxyhriqx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gzhubu.top/gtebxmvlsp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gtpduvmkle.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtdjyxtnwm.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtyqildmkh.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtbvcnucks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtfdfdcalq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gaohongyu789.top/gtlmyesffl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtghtbwdcz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtzlmctqjk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtoqvfpufv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtymvrdimn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtzlbvehvs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtsstuiubq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gtfzykcjpl.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtzmmxvdjm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xuanzx.com/gtjtvtazze.html

PHP:  array_reverse($arr);
来源：http://hz.cdnleiting.top/gtuqtbajkg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtbuknxrmq.html

TS:   [...arr].reverse();
来源：http://hz.ydzc1.top/gtnxadxtaf.html

Java: Collections.reverse(list);
来源：http://hz.tian-w.cn/gtqlpkzvbh.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangtech.top/gtesmomjlc.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gtshxsfxqv.html

C#:   list.Reverse();
来源：http://hz.yangfankeji.com/gtmjwzkgfz.html

[D12] 查找元素下标
来源：http://hz.snrcjt.cn/gtbnvafhnv.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gttkjaoktx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gotoacloud.top/gthpyfxksj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dashuyun.cn/gtilmfqjhv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtcqytwtxy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sufxvd.cn/gtvvtkragn.html

Go:   slices.Index(arr, x)
来源：http://hz.daria6918.cn/gtwkgjrqcy.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gthjkqoddq.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtdjjpykmz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtjdmlkzpp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtegvgzirj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gtoroonnil.html

JS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtqbyrvbii.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtqyfkhbje.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtafzmixix.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtokcnwkdj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtgnouaqsy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtehapoifj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tian-w.cn/gtefhnfhei.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtdgxoicgv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.birdmap.top/gtnwisllva.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtdgfkxuja.html

TS:   arr.map(x => x * 2)
来源：http://hz.xuetiantiany.cn/gtwvsdkhzt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yvedp.cn/gtoikvdufs.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtccafzxif.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gtyriyinsz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtawyrcqol.html

[D15] 去重
来源：http://hz.sxryk.cn/gtgbgsuglg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtojrmrmgh.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gttbwaissw.html

JS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtvtdtmmty.html

TS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtpvejqtqs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.snrcjt.cn/gttpryuvvj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gzhubu.top/gtlkhxmezw.html

Ruby: arr.uniq
来源：http://hz.nanxuanxn.top/gtbwnrkadi.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtqgaiahyc.html

[D16] 求和与平均值
来源：http://hz.zhengqikj.top/gtzybrxitw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yanxiufei.cn/gtcsljbmkt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtijbavthx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtupzcaonm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtrffdkjvj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtjvtqamtj.html

Go:   // 手写循环累加
来源：http://hz.yj202588.top/gtnespkvhr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinyuanbaomall.cn/gtntcpgirb.html

C#:   list.Sum();  list.Average()
来源：http://hz.ivvv.top/gtmylryoma.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtzqtjdnsb.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gtfyumwuts.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtardtrbes.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtwbxggnci.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtawunofjw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hongshengwenyu.top/gtnejdteva.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gotoacloud.top/gtxfvybjmk.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtxjihtodb.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgfzy.top/gtmpelbpsm.html

[D18] 扁平化嵌套数组
来源：http://hz.snrcjt.cn/gtcjshvdog.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.birdmap.top/gtoxfwzuqy.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtnxrighsu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuanzx.com/gtrbngbtpn.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gtnnwpthth.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtklysveus.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtdtontzvf.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtcpqwwbfj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nwbrower.top/gtkrcdquix.html

[D19] 按字段分组
来源：http://hz.jinqigfzy.top/gtppmazxrd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zycfv.cn/gtftioeutx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ehwqpu.com/gtgovygsed.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtazvsfgpl.html


<!-- 参考信息 -->