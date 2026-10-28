代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xinyue.icu/gtfkdjlgnu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gzhubu.top/gtaotrqezc.html

[B15] 布尔运算与取反
来源：http://hz.vqdsnc.cn/gtpkproauq.html

Py:   a and b or not c
来源：http://hz.shzxlz.cn/gtbzeaspbh.html

PHP:  $a && $b || !$c
来源：http://hz.zhoulong.xyz/gtpkugjkem.html

JS:   a && b || !c
来源：http://hz.c1oappe.top/gtencybksw.html

TS:   a && b || !c
来源：http://hz.shzxlz.cn/gtgebscugq.html

Java: a && b || !c
来源：http://hz.yj20258.top/gttcxndufz.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtashveyah.html

Ruby: a && b || !c
来源：http://hz.nanxinkj.top/gtzgbemdol.html

C#:   a && b || !c
来源：http://hz.tian-w.cn/gtodxzajef.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinyuanbaomall.cn/gteehjfwky.html

Py:   if not data: return
来源：http://hz.guannengcc.top/gtuvdpkidt.html

PHP:  if (!$data) { return; }
来源：http://hz.birdmap.top/gtuqhkkzxr.html

JS:   if (!data) return;
来源：http://hz.sweek.top/gtstmismiz.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtkvlmpqxs.html

Java: if (data == null) return;
来源：http://hz.jlsjyb.cn/gtumjzahmp.html

Go:   if data == nil { return }
来源：http://hz.jianghu66.top/gtevbmbapw.html

Ruby: return if data.nil?
来源：http://hz.jlsjyb.cn/gtodngoveb.html

C#:   if (data == null) return;
来源：http://hz.zhijiandao.cn/gtphqmcuyl.html

================================================================================
来源：http://hz.zhixingplan.top/gtycgwufkt.html

C. 函数与作用域
来源：http://hz.yvedp.cn/gtofuhguyz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwxidzbxc.html

[C01] 定义函数
来源：http://hz.wangshuangyany.cn/gtbflghwmh.html

Py:   def add(a, b): return a + b
来源：http://hz.zhixingplan.top/gtmtegjhpy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtetlkflqy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtphkohnsl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtqbdssdau.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtdhuvkxab.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhengqikj.top/gtfxbnqsym.html

Ruby: def add(a, b); a + b; end
来源：http://hz.haohaochexian.top/gthahgwffc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtubuyxfos.html

[C02] 默认参数
来源：http://hz.tianlin.xyz/gtqqgrghik.html

Py:   def greet(name="World"): return name
来源：http://hz.meibo888.top/gtvqzceqcu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yuxming.cn/gtztntlsmh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgfzy.top/gtvwtxreuw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.52xcode.cn/gtbcanyhhe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daxiang520.top/gtuzcmnagv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zdqjudy.top/gtujouzigl.html

Ruby: def greet(name = "World") = name
来源：http://hz.smart0.xyz/gtqqxdbgwf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.316326.xyz/gtxkjvjpjm.html

[C03] 可变参数
来源：http://hz.jqgfzy.top/gtmfjunjso.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtjmxsfngk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinghuilouyu.cn/gtqeqbzyqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gttzgxgndy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhixingplan.top/gtpedogcun.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pycfn.com/gtmkfpdyup.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gtvtajwbvv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenjidiqi.icu/gtjnwkiuwl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ivvv.top/gtncjevxko.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinyuanbaomall.cn/gtkqbomgii.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dianchejie.cn/gtklwmejgn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yongpay.top/gtxtxvmxjo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nwbrower.top/gticrluveb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtcysrvzfv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtgqmnwrxz.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigfzy.top/gtkamoqzyy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtmnmspqgx.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gttzskbyyt.html

[C05] 返回多个值
来源：http://hz.nanxuanxn.top/gtqorzqqsx.html

Py:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtgzuojiuw.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gtftykosey.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gtjbqdmosv.html

TS:   return { a, b };
来源：http://hz.fengsongda.top/gtcmqatnip.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtwmgjorhg.html

Go:   return a, b
来源：http://hz.yj20258.top/gtwrkghjge.html

Ruby: return a, b
来源：http://hz.jianghu66.top/gtgpqdaghd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtpumgbneo.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gteksjebxm.html

Py:   square = lambda x: x * x
来源：http://hz.nwbrower.top/gtowcuaaje.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtfgkdnhii.html

JS:   const square = x => x * x;
来源：http://hz.0kj1m.cn/gttnkfyeql.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cashguo.top/gtczlkjucz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigufen.top/gtisljgudm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.redwolf501.top/gtphkyajqb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gzhubu.top/gtlziusgik.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258888.top/gtgaofndqq.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtajihodxu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtbqeqnmqi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgufenzy.top/gtqshwpsgx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtzjscbfyr.html

TS:   arr.map(String)
来源：http://hz.hnqzz.top/gtvohopetb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxinkj.top/gtxjnpazmk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtjzvmziyc.html

Ruby: arr.map(&:upcase)
来源：http://hz.shzxlz.cn/gtdywycgjg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tanke756.top/gtvclcgrdm.html

[C08] 闭包
来源：http://hz.yvedp.cn/gtsftmgsin.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jqgufenzy.top/gtjfjwrsvl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fengsongda.top/gtelthyjur.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtbehkorng.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtwkyhuitg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangshuangyany.cn/gtuwtuwldw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.9152youxi.cn/gtmxpwikel.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtplkhbqur.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtpcfvmnqe.html

[C09] 递归
来源：http://hz.mhx1999.top/gtpdspsxls.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtjqpjriak.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.feifeiyinyue.top/gtwqcdqobv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtzweqivfx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtnxbmpjmv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtvqjsvrjk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shuidangran.top/gtgsyhaoyq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtubggpmjr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gotoacloud.top/gttagkemgd.html

[C10] 变量作用域
来源：http://hz.hywenlv.cn/gtcqrszlym.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cdnleiting.top/gtgeaefpea.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtliwkcuae.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtwmhiqnbi.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtetqfhkka.html

Java: 方法内为块级作用域
来源：http://hz.sxryk.cn/gtncvzziqh.html

Go:   花括号块级作用域
来源：http://hz.aibaodan.cn/gtnklplkfj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinyuanbaomall.cn/gtevbccndm.html

C#:   块级作用域
来源：http://hz.tianlin.xyz/gtqtxlbpyn.html

[C11] 模块导入与导出
来源：http://hz.shzxlz.cn/gtgwtuelqt.html

Py:   from module import func
来源：http://hz.iojbl.cn/gtrnuykoyh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtmuxfztym.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daxiang520.top/gtxcjspfmi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aizwys.cn/gttkspkpun.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gtgzcyypwe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hysaishi.cn/gtjdpuinhd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ivvv.top/gtgjghmwqk.html

C#:   using System.Text;
来源：http://hz.cheryme.top/gtaelmpexf.html

[C12] 立即执行函数 IIFE
来源：http://hz.sweek.top/gtptuxcxfr.html

Py:   (lambda: print("run"))()
来源：http://hz.daxiang520.top/gtxdiexoyx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shzxlz.cn/gtmmyynorx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtlirxmtfj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.haohaochexian.top/gtwmtvargt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zycfv.cn/gtsiocakro.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gtcjywmxul.html

Ruby: -> { puts "run" }.call
来源：http://hz.yvedp.cn/gtkgfvenfm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ydjk.org.cn/gtzgrfaygk.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtrxnirujx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtkshwuzmp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtfviwfbmd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxinkj.top/gtfkoyjjli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtrjaridul.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtchdxnyux.html

Go:   func add(a, b int) int
来源：http://hz.xingfuxueyuan.xyz/gtlyxuecnc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tianlin.xyz/gtpuaavhth.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jyoumei.cn/gtehjfcezs.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtwgmkrxor.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj202588.top/gtvgjjghlz.html

PHP:  // 无泛型
来源：http://hz.aibaodan.cn/gtbjekrmex.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtdclqooza.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.52xcode.cn/gtozszykyl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtpaeornyg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuxming.cn/gtiuluyqyk.html

Ruby: # 无泛型
来源：http://hz.9152youxi.cn/gtoqbpadox.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dashuyun.cn/gtnipjhgem.html

[C15] 解构 / 展开参数
来源：http://hz.fengsongda.top/gtmfqvdste.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtocsrdayx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.meibo888.top/gtmenxqfrv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtiwsjmsvz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jiagoushi.top/gtsnnflmgd.html

Java: // 无解构
来源：http://hz.ehwqpu.com/gtmhljepol.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtnpjlmgym.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtrdcspeph.html

C#:   var (a, b) = pair;
来源：http://hz.jiagoushi.top/gtnxxgtdks.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtkiexodoe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtcxkkyhow.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtifjnkzyq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.vqdsnc.cn/gtblskfzay.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zdqjudy.top/gtnhmxoytk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.316326.xyz/gtozniecdb.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gtswavvcdi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nwbrower.top/gtxwivmapa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtoiouxuah.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gteokdtcrc.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtymzomrzc.html

================================================================================
来源：http://hz.ybcxt.top/gtluhumxvq.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtjwunvgxm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guannengcc.top/gtzhymruxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.svipenyu.cn/gtipsfjuja.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yongpay.top/gtvgeqfjoi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtpdlmzeil.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigufen.top/gtgxieslil.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhongyouzk.top/gtpxiqjhdr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xziqi.cn/gtcrsvowcl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangshuangyany.cn/gtwhuxfamr.html

[D02] 追加元素到末尾
来源：http://hz.wangdashe.top/gtildsqlbh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aibaodan.cn/gtmeaeadgx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhixingplan.top/gtvqsxvgxs.html

JS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtciflirdy.html

TS:   arr.push(4);
来源：http://hz.c1oappe.top/gtkzrwpdeb.html

Java: list.add(4);
来源：http://hz.ywan-chungtsiang.top/gtrkskvfqe.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtmhfjhorq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtyytkojhy.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gthftfulpm.html

[D03] 在指定位置插入元素
来源：http://hz.zhaomingkeji.xyz/gtrojprqpl.html

Py:   arr.insert(0, 0)
来源：http://hz.9152youxi.cn/gtebbkjbpg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.9152youxi.cn/gtnmfecjlt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtubebeqic.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sxryk.cn/gtxlutcfwd.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gtwjbykpvx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zdqjudy.top/gtaruhipou.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yueranfly.top/gtnmmchqto.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtvuyzobyc.html

[D04] 删除元素
来源：http://hz.hammf.cn/gtpbzszixf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.feifeiyinyue.top/gtqxxtiupe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xziqi.cn/gtdakulwcw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigfzy.top/gtkieptpts.html

TS:   arr.splice(0, 1);
来源：http://hz.hongshengwenyu.top/gtkikgezbt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtbpjjuvgb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.52xcode.cn/gtjvxsluzt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtbbrmmwxf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guowangkeji.top/gtgleulboy.html

[D05] 访问与修改元素
来源：http://hz.redwolf501.top/gtzmagjjba.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtscwurzla.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtmmpqjnmd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xinyue.icu/gtvhomhsoe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangshuangyany.cn/gtlmuwbavt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.c1oappe.top/gtwgadrncb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.bjfxy.top/gtnqlmwvdh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtiiyoocsd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.0kj1m.cn/gtpaunavhh.html

[D06] 数组长度
来源：http://hz.svipenyu.cn/gtrytbrfjy.html

Py:   len(arr)
来源：http://hz.hongshengwenyu.top/gtysvwgjqz.html

PHP:  count($arr);
来源：http://hz.zhoulong.xyz/gtxajuifcc.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtxgznmlhc.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gttugtmdse.html

Java: list.size();
来源：http://hz.vqdsnc.cn/gtaoklmeqs.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtfuyreukb.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtcactzfim.html

C#:   list.Count;
来源：http://hz.havefunace.top/gtlaztiylk.html

[D07] 切片 / 取子数组
来源：http://hz.hnxiangtu.top/gtjqopvalk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.0kj1m.cn/gthnksgmcg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.haohaochexian.top/gtdxfpcjil.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gttynztlwx.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtgxyaknlv.html

Java: list.subList(1, 4);
来源：http://hz.fengsongda.top/gteqrawwjp.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtskahfudw.html

Ruby: arr[1, 3]
来源：http://hz.daxiang520.top/gtfieklxwf.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhoulong.xyz/gtwjjmkqjn.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtxitjjsvt.html

Py:   a + b;  a.extend(b)
来源：http://hz.c1oappe.top/gtowlviytg.html

PHP:  array_merge($a, $b);
来源：http://hz.snrcjt.cn/gtawlqgocp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenlongwang.top/gtajslrxqs.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtrquflivh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtylqeywbg.html

Go:   append(a, b...)
来源：http://hz.gzhubu.top/gtxpmzgkur.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jiagoushi.top/gtmimbeutk.html

C#:   a.Concat(b).ToList()
来源：http://hz.shzxlz.cn/gtjfrmmivh.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtrurvfrou.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtslyaukvx.html

PHP:  sort($arr);
来源：http://hz.jianghu66.top/gtbikpwsxj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtorgrdaym.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtphmooiek.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jyoumei.cn/gtluxamlsx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtksnynjbh.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtjfabzzrt.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtximauwwk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ppjwa.cn/gtolgqsxbo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtemvtuvjj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nwbrower.top/gtsfksipcs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtdryvmdae.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gteqbkxgsa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.0kj1m.cn/gtjdwyvtmh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtvylvhmoq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gttcfmrhhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gtzflwblzd.html

[D11] 反转数组
来源：http://hz.xuetiantiany.cn/gtlywnhmwu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigfzy.top/gtarxcpggp.html

PHP:  array_reverse($arr);
来源：http://hz.guannengcc.top/gtmnohdfgy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gtdkfyfzaj.html

TS:   [...arr].reverse();
来源：http://hz.hnqzz.top/gtxcrdzeye.html

Java: Collections.reverse(list);
来源：http://hz.cheryme.top/gtynapgibu.html

Go:   slices.Reverse(arr)
来源：http://hz.xinyue.icu/gtgslezils.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtdxzfmbco.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gthcpkztsm.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangtech.top/gtttjvceau.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenzaomai.com/gtunjhawbl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtehfyiauz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtkozzhsom.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.vqdsnc.cn/gtquulgxiq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.havefunace.top/gtfxeifucu.html

Go:   slices.Index(arr, x)
来源：http://hz.hywenlv.cn/gtsmqkxbly.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangkeji.top/gtstjokjxr.html

C#:   list.IndexOf(x);
来源：http://hz.xuetiantiany.cn/gtxqndkugk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gtnjrxeufn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.svipenyu.cn/gttvepxokw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtexehlnpr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtkqqfsiju.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtgkjtyeej.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.havefunace.top/gtrstitcxz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hfpthk.cn/gtshaavjbb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xziqi.cn/gtpsrpsbmz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ybcxt.top/gtuedphbup.html

[D14] 映射转换（每个元素变形）
来源：http://hz.vqdsnc.cn/gtdtyeutcz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinyuanbaomall.cn/gtciileuuk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtdoveujmc.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtumhpmjee.html

TS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gttelpkdll.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtwxspyuwz.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtfsxqakxn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258.top/gtkxtfrtjq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhixingplan.top/gtvpwmamwj.html

[D15] 去重
来源：http://hz.316326.xyz/gtagqaheso.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtbbihauzt.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtdihjpcgt.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtqfytirwq.html


<!-- 参考信息 -->