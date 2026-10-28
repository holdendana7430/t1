代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtrlbxfzwz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.andypj.xyz/gtzxybwhvk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtzvqnrnbb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtubhwkssh.html

[C02] 默认参数
来源：http://hz.shangyingyoupin.top/gtholalgsl.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtzozqyzsu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sweek.top/gtyzyyztcc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tianlin.xyz/gtzmlkxnlw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtjpqijhdt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtudiqobsf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtnkfrjrnn.html

Ruby: def greet(name = "World") = name
来源：http://hz.kuanghao11.cn/gtykmbusdw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhoulong.xyz/gtjayrlzwf.html

[C03] 可变参数
来源：http://hz.hongshengwenyu.top/gthqevqary.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuanzhike.top/gtwiusbtif.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.c1oappe.top/gtefwqkpxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtcvtboavq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtflketgsp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtlennrikf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenjidiqi.icu/gtujubxoyg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.snrcjt.cn/gtyzimiprp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhengqikj.top/gtqxlnejzw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangtech.top/gtfjtwmkhk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gotoacloud.top/gtrnwmylqi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenzaomai.com/gtupsqainr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtrnbbphkt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ehwqpu.com/gttdsumbit.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jiagoushi.top/gtccniieyx.html

Go:   // 无：用配置结构体参数
来源：http://hz.gaohongyu789.top/gtwdapjzwu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtjwlatqtz.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtmdkjxtvq.html

[C05] 返回多个值
来源：http://hz.dashuyun.cn/gthwpntzye.html

Py:   return a, b
来源：http://hz.bjfxy.top/gtdnsawckv.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtfvhjnoql.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yanxiufei.cn/gtcuymplvt.html

TS:   return { a, b };
来源：http://hz.daxiang520.top/gtegmszvwb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinghuilouyu.cn/gttlwilxct.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtzwbemrgm.html

Ruby: return a, b
来源：http://hz.jqgfzy.top/gthqpfearw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtwxzupivp.html

[C06] 匿名函数 / lambda
来源：http://hz.yangfankeji.com/gtzylfgtqp.html

Py:   square = lambda x: x * x
来源：http://hz.haohaochexian.top/gtsndpmctd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.birdmap.top/gtpvfotpgu.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtppmdgiaw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.quarkkingdee.top/gtruhhshlu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yongpay.top/gtdryhbfaw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxinkj.top/gtigayrxuz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gtqqoevmou.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigufen.top/gtshheqohu.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigufen.top/gttndugofl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtterdcphj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxinkj.top/gtdghjmmwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuetiantiany.cn/gtkjjkbhnr.html

TS:   arr.map(String)
来源：http://hz.redwolf501.top/gtyokiuaun.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhongyouzk.top/gttizkpfyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nanxuanxn.top/gtosfplzbd.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtykygfecx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shanyushiyangtech.top/gtcjluznuu.html

[C08] 闭包
来源：http://hz.c1oappe.top/gtctccetmt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtsqqmqdfd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gtodalbljk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtntguhhkv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtlohuzmhm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daxiang520.top/gtimiuptbb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhiwuduotai.top/gtcyfsmghs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gtqjhmlllj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtyhoqqnad.html

[C09] 递归
来源：http://hz.shanyushiyangtech.top/gtrcgfnfko.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtqqmhwuqg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhijiandao.cn/gtqxpwotta.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gtjkqhvmtq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtkuvawjlp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenzaomai.com/gtfbxyktgp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtydnrukjl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gttegssfsm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gtoglxwhmi.html

[C10] 变量作用域
来源：http://hz.chenjidiqi.icu/gtxfklfrzs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dianchejie.cn/gtldslthgx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guowangkeji.top/gtsqoeaejh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.snrcjt.cn/gtpmignunk.html

TS:   同 JS
来源：http://hz.zhaomingkeji.xyz/gtktmhtyte.html

Java: 方法内为块级作用域
来源：http://hz.jinqigfzy.top/gtovzfhgjp.html

Go:   花括号块级作用域
来源：http://hz.tian-w.cn/gtdrmjfjmf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenzaomai.com/gtgfnabiej.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtstieivqx.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gtbadlbuec.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtgcjxetsy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jiagoushi.top/gtzalvkbkb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtosjllauw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtmwuaoscx.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtkqucoezr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.bjfxy.top/gtuuvxsxex.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtpjpcnqqf.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gtkikgpbeb.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxinkj.top/gtpgemxivk.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtvmocrbfl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258.top/gtptrsndxp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtsswfmhrv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtmteqbcir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtmkofardu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cashguo.top/gtnfrpxkhb.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gtfffpozjl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinyuanbaomall.cn/gtyzjbmdbh.html

[C13] 类型声明 / 类型注解
来源：http://hz.pengpengdd.cyou/gtfhvquflm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yueranfly.top/gtfrgkvydp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtyvntihzx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gtvxdgkmvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtmozehafv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtjasucbyz.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gtcwzypqdt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtgpusydky.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.svipenyu.cn/gtffcueegq.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtauyqqeua.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhoulong.xyz/gtpytllvkv.html

PHP:  // 无泛型
来源：http://hz.sufxvd.cn/gtnnwagnxh.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtstvnmbyj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pycfn.com/gttugtczut.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jlsjyb.cn/gtdnkofvrq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gtpxxnbdbb.html

Ruby: # 无泛型
来源：http://hz.vqdsnc.cn/gtfoxcyewm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtjwpgmwbf.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gtvtpxpclm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenlongwang.top/gtdwmfmntq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtlaeqxvpo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtkgkhnxip.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pycfn.com/gtorsswbsd.html

Java: // 无解构
来源：http://hz.gzhubu.top/gttoofcsif.html

Go:   // 无解构
来源：http://hz.gotoacloud.top/gthauxtsob.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtjneivpyu.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtqvndcqsd.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtgaozbxgj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daria6918.cn/gtfbfawecx.html

PHP:  // 无重载
来源：http://hz.mhx1999.top/gtejghlvbd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtjqcfezld.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yueranfly.top/gtjphkfscf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhongyouzk.top/gtawcqegyi.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhijiandao.cn/gtdcxpffyn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gtgjolhekf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenjidiqi.icu/gtdldapfdf.html

================================================================================
来源：http://hz.wangdashe.top/gtejuchjgs.html

D. 数组 / 列表 / 集合
来源：http://hz.chenlongwang.top/gthlvhssby.html

================================================================================
来源：http://hz.yuxming.cn/gtzkguwdyu.html

[D01] 创建数组 / 列表
来源：http://hz.yuanzhike.top/gtsmhnjmyn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtpcvkyzsk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pycfn.com/gtojjywjbx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gzhubu.top/gtvdadnpgf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.quarkkingdee.top/gtvenlegxb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuxming.cn/gtnhkbjpfc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gtqqwonvzs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtrabkxhcg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dianchejie.cn/gtalbalnzs.html

[D02] 追加元素到末尾
来源：http://hz.meibo888.top/gtqiylqwuh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtvnupqbwq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtxqykcdlz.html

JS:   arr.push(4);
来源：http://hz.hnqzz.top/gtzxrvubjl.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtilbiegkv.html

Java: list.add(4);
来源：http://hz.birdmap.top/gtptkihqdb.html

Go:   arr = append(arr, 4)
来源：http://hz.iojbl.cn/gtagqcfcgy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtapzfuuvp.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtwhjrojtu.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtkglgcmcm.html

Py:   arr.insert(0, 0)
来源：http://hz.cashguo.top/gtfzwzgrcr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.wangdashe.top/gtiuncojan.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydzc1.top/gtfgxwcfss.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtdhjxduux.html

Java: list.add(0, 0);
来源：http://hz.guannengcc.top/gttibxxcqo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gttpqkocmi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gthwtwbfqh.html

C#:   list.Insert(0, 0);
来源：http://hz.chenlongwang.top/gtxfpujhzm.html

[D04] 删除元素
来源：http://hz.zhiwuduotai.top/gtycryigpw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtgwgnuhts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zycfv.cn/gtjhmvwkio.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.havefunace.top/gtdzsnbvhr.html

TS:   arr.splice(0, 1);
来源：http://hz.zhijiandao.cn/gtqmztflfu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtmbfoukrt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tian-w.cn/gtokarzttp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gtrhzgftci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gtqxerokni.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtnznxjqhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtfxlczyfq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gteudbnrpw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.meibo888.top/gtynbdxbwq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nwbrower.top/gtvphgnqwn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtlyjuthoi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fengsongda.top/gtgbmelyht.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtvoijqymg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtzbgiuhcb.html

[D06] 数组长度
来源：http://hz.shangyingyoupin.top/gtnbhtwlpl.html

Py:   len(arr)
来源：http://hz.sxryk.cn/gthtkuwzfa.html

PHP:  count($arr);
来源：http://hz.cqqwz.cn/gtaqtvmkld.html

JS:   arr.length
来源：http://hz.ehwqpu.com/gtdvkymowk.html

TS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gtytkuygvi.html

Java: list.size();
来源：http://hz.jinghuilouyu.cn/gtyiuadhtd.html

Go:   len(arr)
来源：http://hz.jinqigufen.top/gtarufdywu.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtcblicpul.html

C#:   list.Count;
来源：http://hz.gaohongyu789.top/gtxuirltdc.html

[D07] 切片 / 取子数组
来源：http://hz.xinyue.icu/gtgrdlnubx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fzhhl.top/gtfhlrbhvi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtwlelcmud.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtjcpzokzi.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtkwbpwgnq.html

Java: list.subList(1, 4);
来源：http://hz.snrcjt.cn/gtuofeqpgy.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gteaizhgal.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gtlcankfbn.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhengqikj.top/gtdzajjljp.html

[D08] 合并两个数组
来源：http://hz.yuanzhike.top/gtbvquxbgl.html

Py:   a + b;  a.extend(b)
来源：http://hz.feifeiyinyue.top/gtmdoyezzo.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gttswepraj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenlongwang.top/gtdrpackfd.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtgaitjidn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtvexaajos.html

Go:   append(a, b...)
来源：http://hz.cqqwz.cn/gttderxnpr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gthkxkdqgk.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhijiandao.cn/gtdyhsybrk.html

[D09] 排序（升序）
来源：http://hz.tian-w.cn/gtaozmozrp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtqeojxzmu.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtqdmbmllo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gtbaqzyanz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtnzcozuex.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gtuakugbjk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtwqcpenhp.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtrwaasixf.html

C#:   list.Sort();
来源：http://hz.cashguo.top/gtaueswrjz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yanxiufei.cn/gtkiksjchd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dianchejie.cn/gtimgovzqk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtxblfhtqc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtsivwvnny.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtbxqmlluo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangdashe.top/gtfxwvvpsk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtghnmtxkf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.haohaochexian.top/gteqqtjfxj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gogol.net.cn/gtlqccojmv.html

[D11] 反转数组
来源：http://hz.hywenlv.cn/gtplrrecpj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.vqdsnc.cn/gtgpepdszj.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gtnyvxnqts.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.9152youxi.cn/gthgvhfdyc.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtgvlinfyo.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gtzzmfuefy.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtfbqvzvly.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtrulutrhh.html

C#:   list.Reverse();
来源：http://hz.gotoacloud.top/gtwfimrecu.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtpscihqih.html

Py:   arr.index(x);  x in arr
来源：http://hz.xingfuxueyuan.xyz/gthsrvjwhe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtknzpgzsv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtedyjzkdi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtttmpkzqn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gzhubu.top/gtvlwnxkxz.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gtqjvfjsrr.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtkdblhwnf.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtfzwakfix.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtullvccsp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangshuangyany.cn/gtinrpzpbw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtbsrducmm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtqvicvfvp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtgdcgserl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ivvv.top/gtvdlclbva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gttoxdcfnh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dashuyun.cn/gtrklztggv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.guowangkeji.top/gtkayopkrn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtrtecgvfn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenlongwang.top/gtffkwzypa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtvfibopge.html

JS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtanrisces.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtoynpdlfg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtaleuchyp.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtfbgobedp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aibaodan.cn/gtciozcxvf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.redwolf501.top/gtpirhhsjo.html

[D15] 去重
来源：http://hz.svipenyu.cn/gtbdxuftql.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtufilceeg.html

PHP:  array_unique($arr);
来源：http://hz.sweek.top/gtgdkpbgem.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtvmngfyjd.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtyvrrtbby.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jlsjyb.cn/gtetdaaenw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtrzodbnli.html

Ruby: arr.uniq
来源：http://hz.sxryk.cn/gtpesgfchy.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtgtshkadm.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtdgdvvsux.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtoqrjnyvf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shzxlz.cn/gtjplkwxjy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtzatvuntm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtwntfopui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtrypnlqox.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtjmionslr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dashuyun.cn/gthfaluuma.html

C#:   list.Sum();  list.Average()
来源：http://hz.sysykeji.top/gtrweswtwm.html

[D17] 最大值与最小值
来源：http://hz.xuetiantiany.cn/gtwpxgfvpv.html

Py:   max(arr);  min(arr)
来源：http://hz.cdnleiting.top/gtrcelkyqz.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtpvvfavbm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gthzdhzmfm.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtmkyilkrj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jlsjyb.cn/gtcbzsfyzu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtgdjkwgnd.html

Ruby: arr.max;  arr.min
来源：http://hz.cheryme.top/gthucifsfs.html

C#:   list.Max();  list.Min()
来源：http://hz.xinyue.icu/gtkapaybuw.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtzudtkitx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtgptzppzj.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtiwdgbgqz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.haohaochexian.top/gtmgiizqhr.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gthjyvjzze.html


<!-- 参考信息 -->