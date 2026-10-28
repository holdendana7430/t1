代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ivvv.top/gtmfyerkzh.html

Java: x instanceof Number
来源：http://hz.chenzaomai.com/gtuxikkded.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhiwuduotai.top/gtnycexnxv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ivvv.top/gtmnppayhs.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gturfaxqtm.html

[B14] 判断值是否在集合内
来源：http://hz.nanxuanxn.top/gtzhhvvpcw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dianchejie.cn/gtqekacjjv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zycfv.cn/gtlesmbuat.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtntzppgcb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtegioyahj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zycfv.cn/gtrsrxaruk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuanzx.com/gtsltyruhc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cucudq.cn/gtgelmvbqu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigfzy.top/gtprurjxka.html

[B15] 布尔运算与取反
来源：http://hz.tanke756.top/gtnyhysnkn.html

Py:   a and b or not c
来源：http://hz.yvedp.cn/gtdgeuouwx.html

PHP:  $a && $b || !$c
来源：http://hz.havefunace.top/gtpjpkvukf.html

JS:   a && b || !c
来源：http://hz.cdnleiting.top/gtlhcsuwtb.html

TS:   a && b || !c
来源：http://hz.cheryme.top/gtczfhpqxo.html

Java: a && b || !c
来源：http://hz.yj202588.top/gtsqgvnapi.html

Go:   a && b || !c
来源：http://hz.52xcode.cn/gtrpxodjdp.html

Ruby: a && b || !c
来源：http://hz.hywenlv.cn/gtmktslrye.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtqzazirpq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sweek.top/gtrvcgqgtz.html

Py:   if not data: return
来源：http://hz.cashguo.top/gtadyhzllr.html

PHP:  if (!$data) { return; }
来源：http://hz.tanke756.top/gtleqkthwd.html

JS:   if (!data) return;
来源：http://hz.daria6918.cn/gtanknilou.html

TS:   if (!data) return;
来源：http://hz.xylfe.cn/gtxmxpbpfy.html

Java: if (data == null) return;
来源：http://hz.tian-w.cn/gtmgebsfvj.html

Go:   if data == nil { return }
来源：http://hz.gzhubu.top/gtavpxwsyp.html

Ruby: return if data.nil?
来源：http://hz.haohaochexian.top/gtayfxggss.html

C#:   if (data == null) return;
来源：http://hz.zhijiandao.cn/gtbngkzmgt.html

================================================================================
来源：http://hz.hnqzz.top/gtznsfbptx.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gttyehahzr.html

================================================================================
来源：http://hz.ydzc1.top/gtsfoptero.html

[C01] 定义函数
来源：http://hz.aizwys.cn/gtrathnvep.html

Py:   def add(a, b): return a + b
来源：http://hz.yj202588.top/gtemtwmhnp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtrghaxsbj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yueranfly.top/gtakdcldsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtrbolfpai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtuqhrdteg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtpmckkdas.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuanzx.com/gtolphqaxk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtzviejoyi.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtcuqmamkc.html

Py:   def greet(name="World"): return name
来源：http://hz.xziqi.cn/gtqnrcjadm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gtfdjwwmrd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtnpvrkbrz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhengqikj.top/gtzhxnpkzr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.kuanghao11.cn/gtfxicinzq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangkeji.top/gtjyjxvbvs.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenzaomai.com/gteydlipay.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yueranfly.top/gtqxwfotey.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtgwxoroei.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydjk.org.cn/gtjmwidvdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yanxiufei.cn/gtxqkrpyhy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtpwufubxz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigufen.top/gtbijvlein.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sweek.top/gtrnzvsqkh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sysykeji.top/gtqkyzjccb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtjwsnolea.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhiwuduotai.top/gtaxsfbyhw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtcjhtpmjr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gtirrxseii.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtmsqrejzc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtvfqjilwi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gaohongyu789.top/gtyeerbqlu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pengpengdd.cyou/gtllcrtbim.html

Go:   // 无：用配置结构体参数
来源：http://hz.daria6918.cn/gtixpovkfv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtegqtxfuc.html

C#:   f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtwqejzgpa.html

[C05] 返回多个值
来源：http://hz.zhaomingkeji.xyz/gtfmnjaaly.html

Py:   return a, b
来源：http://hz.xinyue.icu/gtokvoxugi.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtitmuhwja.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yangfankeji.com/gtqdeimkis.html

TS:   return { a, b };
来源：http://hz.yuanzhike.top/gtaeebsojl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.c1oappe.top/gtlncjjgoj.html

Go:   return a, b
来源：http://hz.hysaishi.cn/gtatdavqgw.html

Ruby: return a, b
来源：http://hz.hysaishi.cn/gtmmjklpnc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hywenlv.cn/gtlefmrxdo.html

[C06] 匿名函数 / lambda
来源：http://hz.c1oappe.top/gtztktgdzl.html

Py:   square = lambda x: x * x
来源：http://hz.cheryme.top/gtkxozlluk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xylfe.cn/gtywpfdpwv.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtnytjxhso.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenjidiqi.icu/gtnkhxlbaz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gthfhjplxf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gtfyvyeseq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gtcjbpurjm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhoulong.xyz/gtnlakyugi.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtvsiljffk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.vqdsnc.cn/gtlinfdxka.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.smart0.xyz/gtszfnpbkc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtahjxffed.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtnfnmtkmq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtgiklgagv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.316326.xyz/gtacmidway.html

Ruby: arr.map(&:upcase)
来源：http://hz.kuanghao11.cn/gtwptmbfcj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenzaomai.com/gtzqhdyhpq.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtxzwhcedo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hongshengwenyu.top/gtgiavoxxs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jiagoushi.top/gtxpefiyhm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtujxsjihn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtribcvhgt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yangfankeji.com/gtdfdmukdc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenlongwang.top/gtpdauluul.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtzcenhpyj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtvyephmuo.html

[C09] 递归
来源：http://hz.tanke756.top/gtbjyertcr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtycrjmwrh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daria6918.cn/gtvinrjlyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtyyxzdhqi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtroygoqgp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtkyamjsnq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtfqpvakas.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtvbeblmvr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dashuyun.cn/gtqywcknik.html

[C10] 变量作用域
来源：http://hz.jinyuanbaomall.cn/gtpmttjosd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guowangkeji.top/gtpqfbyhvd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtrofztagd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.9152youxi.cn/gtdznlayxn.html

TS:   同 JS
来源：http://hz.bjfxy.top/gtuzalzrew.html

Java: 方法内为块级作用域
来源：http://hz.jinqigufen.top/gtigancofm.html

Go:   花括号块级作用域
来源：http://hz.zhijiandao.cn/gtjqelznwh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnxiangtu.top/gtuilbdlhs.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtdoucrvdb.html

[C11] 模块导入与导出
来源：http://hz.zhaomingkeji.xyz/gtcmhubgpu.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtoxeeucdf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinyuanbaomall.cn/gtdvtoziqk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gtveuaffnj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtvhpjgyhm.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gtqvlajovk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxinkj.top/gtlnkdprig.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtcmelgksc.html

C#:   using System.Text;
来源：http://hz.xinyue.icu/gtbhszqczs.html

[C12] 立即执行函数 IIFE
来源：http://hz.sysykeji.top/gtosoinuwm.html

Py:   (lambda: print("run"))()
来源：http://hz.meibo888.top/gtlmrosvua.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtnhinlsky.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtkbrlbbxw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtyfpdoypb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jlsjyb.cn/gtjhtjggez.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ehwqpu.com/gtbvcfetkl.html

Ruby: -> { puts "run" }.call
来源：http://hz.zycfv.cn/gtaqgejccy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtlpooffjs.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtbdjskwzo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.bjfxy.top/gtongsucfj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtklodfzwf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gogol.net.cn/gtttlniyrt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtuahdbrnd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtpkesuffp.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gtoqoeeazx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtrrwgdkgs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ppjwa.cn/gtfxfgeclx.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtafswnpbd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtjofmvpyc.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtvbzqsgkh.html

JS:   // 无泛型
来源：http://hz.chenjidiqi.icu/gtrrhrpseh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtucalixea.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenjidiqi.icu/gtgropdqai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtordgldix.html

Ruby: # 无泛型
来源：http://hz.c1oappe.top/gtsnjecttl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gthpfptjvk.html

[C15] 解构 / 展开参数
来源：http://hz.kuanghao11.cn/gtpjiorjpp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gzhubu.top/gtmzcjvaju.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtchdtluuc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtquigrybk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxinkj.top/gtytdlpfyv.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gtehklqhlq.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtvsdjpubi.html

Ruby: a, b = pair
来源：http://hz.nwbrower.top/gtxaehgdwo.html

C#:   var (a, b) = pair;
来源：http://hz.yuxming.cn/gtipupdosb.html

[C16] 函数 / 方法重载
来源：http://hz.gzhubu.top/gtiiownpyz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtcocazysi.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtiblyogam.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tanke756.top/gtpospjfjb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuanzhike.top/gtnwbupyod.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtsdpzscob.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhaomingkeji.xyz/gtfnjvnwzo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.svipenyu.cn/gtiwgzxuyl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.iojbl.cn/gtxkvpyksd.html

================================================================================
来源：http://hz.guannengcc.top/gtlvhvyqai.html

D. 数组 / 列表 / 集合
来源：http://hz.cqqwz.cn/gtcbesnrac.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtuwekdcqd.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtkrsmqcdw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtrgjdeckq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtmtlgidef.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinyuanbaomall.cn/gtgcqrtvds.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.aizwys.cn/gtsxznehdf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtzrhfaxho.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gthoduhwjn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhongyouzk.top/gtobelntkh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtzjvtgmkg.html

[D02] 追加元素到末尾
来源：http://hz.jinqigufen.top/gtxuqlylvh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxinkj.top/gtcmwvrlhf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtdxonmyeg.html

JS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtofwosnnb.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtnhpxwfyr.html

Java: list.add(4);
来源：http://hz.meibo888.top/gtgriokonx.html

Go:   arr = append(arr, 4)
来源：http://hz.cdnleiting.top/gtmgnahggk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtccurrxxv.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtqvmaibio.html

[D03] 在指定位置插入元素
来源：http://hz.sweek.top/gtbmvdqznx.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtoxxaxyds.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuanzx.com/gtroekmvru.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gtbhgzfvqu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jianghu66.top/gtuloprfaz.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gtajelwxzy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sysykeji.top/gtbyauswjn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ivvv.top/gtkktfenuq.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtdqvmfnob.html

[D04] 删除元素
来源：http://hz.yj20258888.top/gtdykaqsia.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gtqqkwzwqb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuxming.cn/gtplukufgs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gogol.net.cn/gtvavjdpfr.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtxocdgzzs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtbckznzsh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtlblahblc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhixingplan.top/gtjysqudwh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nwbrower.top/gtfuyizafk.html

[D05] 访问与修改元素
来源：http://hz.birdmap.top/gtfykuncmg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtarccdccm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgfzy.top/gtfhwawbpo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtaynqyyiv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtxxedfgqk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daxiang520.top/gtofgghxch.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtytncuups.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtiapscpuu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtupfcymgl.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtcdxrtora.html

Py:   len(arr)
来源：http://hz.zhiwuduotai.top/gtyevoxfme.html

PHP:  count($arr);
来源：http://hz.daxiang520.top/gtvdihxgcj.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtmiedviae.html

TS:   arr.length
来源：http://hz.zhiwuduotai.top/gtfqllbden.html

Java: list.size();
来源：http://hz.hywenlv.cn/gtlqyaqggk.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtcsudzvwu.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtyawhkmux.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gtutppirkq.html

[D07] 切片 / 取子数组
来源：http://hz.pycfn.com/gtaeusmcax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xingfuxueyuan.xyz/gtipexolwu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daxiang520.top/gtyyeyutsx.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtjuwqtsnx.html

TS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gttanuyvox.html

Java: list.subList(1, 4);
来源：http://hz.dianchejie.cn/gtdqxvyhpt.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangkeji.top/gthknmpaww.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtyxpyqtif.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtlubuohuv.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gtlnwukggp.html

Py:   a + b;  a.extend(b)
来源：http://hz.jiagoushi.top/gtjxonxsqk.html

PHP:  array_merge($a, $b);
来源：http://hz.vqdsnc.cn/gtzifgjvka.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tanke756.top/gtwpljmuou.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gttfpnbnny.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gtpfcvczxy.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtrtgvhoil.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhaomingkeji.xyz/gtguclcyrg.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtvntvpewo.html

[D09] 排序（升序）
来源：http://hz.ydjk.org.cn/gtsedrhkxo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtfmwxumab.html

PHP:  sort($arr);
来源：http://hz.yanxiufei.cn/gtzwuyjiok.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtursrquhd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.316326.xyz/gtacwfbubl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.kuanghao11.cn/gtwkuskebh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtxzqjvbkl.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtbzleetmr.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtexozrrbo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtegakqmyz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fengsongda.top/gtpdijusqw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtdsrobmih.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtuzbhnuto.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.mhx1999.top/gtjearmsct.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtqhoykqkq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gthzdgldxs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fzhhl.top/gtdbofrwqc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cashguo.top/gtopbozdoq.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtyuxhqnnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtfphztamp.html

PHP:  array_reverse($arr);
来源：http://hz.ivvv.top/gtmnktsaoo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnxiangtu.top/gtzsipdolz.html

TS:   [...arr].reverse();
来源：http://hz.hywenlv.cn/gtxknlwwwj.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtrkzwybxf.html

Go:   slices.Reverse(arr)
来源：http://hz.xinyue.icu/gteqhnqonw.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtrwrnrvyt.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtilukivjw.html

[D12] 查找元素下标
来源：http://hz.9152youxi.cn/gtwwnbtyms.html

Py:   arr.index(x);  x in arr
来源：http://hz.shzxlz.cn/gtnbzmqeca.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gtqupnqbew.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtzkicxneu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gthgkdgttx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigfzy.top/gtxaempjio.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtvqryzjgg.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtztvpxseg.html

C#:   list.IndexOf(x);
来源：http://hz.hfpthk.cn/gtmheohokf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jianghu66.top/gtmmfhkmnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhoulong.xyz/gtcfzejqcr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gtjsapjjkm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtjrdklnei.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtonblehtj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xziqi.cn/gtqkmktawe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtraxqdqdr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtfqukiwre.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xinyue.icu/gtikqtrxsp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtwjronsvy.html


<!-- 参考信息 -->