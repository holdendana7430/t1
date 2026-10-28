代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cqqwz.cn/gtodsqkfvw.html

Java: x instanceof Number
来源：http://hz.snrcjt.cn/gtscjsjeke.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.feifeiyinyue.top/gtzisujixa.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgfzy.top/gtiyqgunuy.html

C#:   x is int or double or decimal
来源：http://hz.nanxuanxn.top/gtqawkvdgd.html

[B14] 判断值是否在集合内
来源：http://hz.cucudq.cn/gtgezvubta.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtnserrkpa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gturrxovxt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gtoyzayimt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtgighmuab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhiwuduotai.top/gtvlbkmhzo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xziqi.cn/gtmjefbaqs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shuidangran.top/gtjhqwnejt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuanzx.com/gttoklepam.html

[B15] 布尔运算与取反
来源：http://hz.andypj.xyz/gtydhuqyjf.html

Py:   a and b or not c
来源：http://hz.aibaodan.cn/gtfzezqlxy.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtwyvvpqlk.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gtpvqzdyxb.html

TS:   a && b || !c
来源：http://hz.yonumen.top/gtclwqfbgi.html

Java: a && b || !c
来源：http://hz.jqgfzy.top/gtknmgnbau.html

Go:   a && b || !c
来源：http://hz.yj20258.top/gtscnpcapn.html

Ruby: a && b || !c
来源：http://hz.daria6918.cn/gtdvqlcukp.html

C#:   a && b || !c
来源：http://hz.hnqzz.top/gtssinmtyg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.redwolf501.top/gtuqvalsxl.html

Py:   if not data: return
来源：http://hz.haohaochexian.top/gtpsyazmwe.html

PHP:  if (!$data) { return; }
来源：http://hz.tian-w.cn/gtgtdyfgye.html

JS:   if (!data) return;
来源：http://hz.ydjk.org.cn/gtcfartrzy.html

TS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtschfblii.html

Java: if (data == null) return;
来源：http://hz.jianghu66.top/gtpffjuxvo.html

Go:   if data == nil { return }
来源：http://hz.hfpthk.cn/gthbagvngq.html

Ruby: return if data.nil?
来源：http://hz.birdmap.top/gtjhaxrxrm.html

C#:   if (data == null) return;
来源：http://hz.zhixingplan.top/gtmomukrwx.html

================================================================================
来源：http://hz.yj20258.top/gtopcinqnp.html

C. 函数与作用域
来源：http://hz.shanyushiyangtech.top/gtlygulyeu.html

================================================================================
来源：http://hz.xuanzx.com/gtpbymzenx.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtnbvzxqtr.html

Py:   def add(a, b): return a + b
来源：http://hz.jinyuanbaomall.cn/gtdqwsaojl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtdhinolzq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.andypj.xyz/gthxhesimt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtwbftedvu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtxznvsqwk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnxiangtu.top/gtkbgsncea.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tian-w.cn/gtvpnckfxv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtipoitmhb.html

[C02] 默认参数
来源：http://hz.cqqwz.cn/gtgxmlamfo.html

Py:   def greet(name="World"): return name
来源：http://hz.cqqwz.cn/gtgbwfbyom.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shanyushiyangtech.top/gtswidfcgt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenzaomai.com/gtvrcxjknm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtsgqzymfm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtjradinbn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gtbinrbhos.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgufenzy.top/gtkaomlzbt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yvedp.cn/gtovhnnkkq.html

[C03] 可变参数
来源：http://hz.gogol.net.cn/gtawbbtjoh.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtdwozqeuz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cucudq.cn/gtgrxkennl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtykbkqowu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtxdkvvqdh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ppjwa.cn/gtztqjbacy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ydzc1.top/gtyqksiibp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhijiandao.cn/gtxnkglqzf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nanxuanxn.top/gtufjwadzh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtkyxliocp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnxiangtu.top/gttemtgqjc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.feifeiyinyue.top/gtywcdupoy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtfjnzaddo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yanxiufei.cn/gtchbdmdvx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinyuanbaomall.cn/gtxbttgbpk.html

Go:   // 无：用配置结构体参数
来源：http://hz.tianlin.xyz/gtudblajql.html

Ruby: f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtwqqsprav.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtqephocpy.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtsftxawdz.html

Py:   return a, b
来源：http://hz.cashguo.top/gtibfqegpo.html

PHP:  return [$a, $b];
来源：http://hz.pengpengdd.cyou/gtfpljxquk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtwkpllzps.html

TS:   return { a, b };
来源：http://hz.jinqigufen.top/gtsxlfvevu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.0kj1m.cn/gtvosnjyqu.html

Go:   return a, b
来源：http://hz.zhongyouzk.top/gtjumsjpma.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtvvnpenva.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yvedp.cn/gtaivcycot.html

[C06] 匿名函数 / lambda
来源：http://hz.daxiang520.top/gteqdxpvcq.html

Py:   square = lambda x: x * x
来源：http://hz.zdqjudy.top/gtpknctfyp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xziqi.cn/gtzfyzaupr.html

JS:   const square = x => x * x;
来源：http://hz.gaohongyu789.top/gtmxfgpulg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.snrcjt.cn/gthfriqtxe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtwcftoink.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtmnsxlxzs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.iojbl.cn/gtiurxnqob.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtecqhkmtq.html

[C07] 把函数作为参数传入
来源：http://hz.jlsjyb.cn/gtwoizpeln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tian-w.cn/gtgmudelbv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangdashe.top/gtkkyoepai.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gtnrsexrgd.html

TS:   arr.map(String)
来源：http://hz.mhx1999.top/gtpyxtfhtw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtshpcsoze.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.0kj1m.cn/gtoqgqpzhg.html

Ruby: arr.map(&:upcase)
来源：http://hz.fzhhl.top/gtfjsheulj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgfzy.top/gtvnqwitbg.html

[C08] 闭包
来源：http://hz.daria6918.cn/gtluppyjtm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuanzhike.top/gtjoygpnxl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sysykeji.top/gtambpkqzx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtfmvtriir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtvrbxmoka.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shangyingyoupin.top/gtfkpfufad.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtxhdbbmom.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shzxlz.cn/gtjeqlzxdo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtkzbfpthu.html

[C09] 递归
来源：http://hz.yj20258.top/gtgklxsqts.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtnxzxahnd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gzhubu.top/gtwcwyvshn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtlxqwltfq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtyghelfgb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtihxjrude.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gthhwnxamm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtvtycjssi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nwbrower.top/gtxzniicnc.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtnzjricre.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.haohaochexian.top/gtppgbpqwe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuetiantiany.cn/gtptgqhxub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtoltvetfx.html

TS:   同 JS
来源：http://hz.jinqigfzy.top/gtaiqstvus.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtpkvchivf.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtgqsfrcic.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gtclaukvbe.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gtsuapgluv.html

[C11] 模块导入与导出
来源：http://hz.quarkkingdee.top/gtjznejwec.html

Py:   from module import func
来源：http://hz.ydzc1.top/gtjjuixujz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.0kj1m.cn/gtzjhtxagh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj20258888.top/gtrkegpwfw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtuldrppkw.html

Java: import java.util.List;
来源：http://hz.ywan-chungtsiang.top/gtwulaxlkw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cqqwz.cn/gtirdqpmzq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gtbakfqxea.html

C#:   using System.Text;
来源：http://hz.nanxinkj.top/gtphlfhqkp.html

[C12] 立即执行函数 IIFE
来源：http://hz.gzhubu.top/gtoljewmle.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gthugodbtw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnqzz.top/gtakxztten.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtcjxdzcfu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtmpdokopg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuxming.cn/gtqmroukvk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnqzz.top/gtymtwlftu.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtptjbsvdw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtvomsxzgq.html

[C13] 类型声明 / 类型注解
来源：http://hz.iojbl.cn/gtughwkgov.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtyonszhwt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtwoyyswry.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxinkj.top/gthkbmhzjc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtrotywyec.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtlufjzwsy.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gtachzjqdl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gtzhamphxf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxinkj.top/gtkpcliusp.html

[C14] 泛型函数
来源：http://hz.yj20258888.top/gtqokfymjd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tanke756.top/gtihthtlsa.html

PHP:  // 无泛型
来源：http://hz.nanxuanxn.top/gtjsucwzwy.html

JS:   // 无泛型
来源：http://hz.hnxiangtu.top/gtzhulgpoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gteyilwqhe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gaohongyu789.top/gtlpqjvetg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gttotwwncc.html

Ruby: # 无泛型
来源：http://hz.daria6918.cn/gtzpjswzkw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtwiraekdn.html

[C15] 解构 / 展开参数
来源：http://hz.zhijiandao.cn/gtbglzbtww.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ehwqpu.com/gtxhgegqmg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtvjabsjak.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtlgijrflf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gtqfnsbxug.html

Java: // 无解构
来源：http://hz.zhixingplan.top/gtfisezhff.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtqopetwug.html

Ruby: a, b = pair
来源：http://hz.jianghu66.top/gtueoxnjvy.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtfpzynnno.html

[C16] 函数 / 方法重载
来源：http://hz.guannengcc.top/gtqufzptzj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gtwusbsxau.html

PHP:  // 无重载
来源：http://hz.gzhubu.top/gtjhuegvgg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtgpcwdpbi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuanzx.com/gttwekncld.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gtqjyeoxnd.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtzngsikdk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dashuyun.cn/gtgcvkgmdu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sufxvd.cn/gtjfatjvce.html

================================================================================
来源：http://hz.hysaishi.cn/gtzmishrsk.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtmcmjnecs.html

================================================================================
来源：http://hz.9152youxi.cn/gtbqllruuw.html

[D01] 创建数组 / 列表
来源：http://hz.ywan-chungtsiang.top/gtqskvsetn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hammf.cn/gtjfdgttrv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinghuilouyu.cn/gtnrpuuewr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhiwuduotai.top/gtbguoyonz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ybcxt.top/gtrongllxm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtmhbrffzs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangkeji.top/gtwrzzqwow.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtzxubnajb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tanke756.top/gtncqfyezg.html

[D02] 追加元素到末尾
来源：http://hz.havefunace.top/gtcgdzyzet.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sxryk.cn/gtvofjkpfg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtgylmwkmq.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtvtrejdwf.html

TS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtpglsoqgi.html

Java: list.add(4);
来源：http://hz.zycfv.cn/gtyjfzgpvn.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtbqlbztox.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtwlkcuqiq.html

C#:   list.Add(4);
来源：http://hz.gogol.net.cn/gtsxbebaef.html

[D03] 在指定位置插入元素
来源：http://hz.tanke756.top/gtojabjqfw.html

Py:   arr.insert(0, 0)
来源：http://hz.shangyingyoupin.top/gtcsthklgg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258888.top/gtmqstddcr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.quarkkingdee.top/gtnaozjhcx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtdzvzpgoq.html

Java: list.add(0, 0);
来源：http://hz.xuanzx.com/gtumvxbbyk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gogol.net.cn/gtgogjbkpk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jlsjyb.cn/gtapamwszs.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtgqbghvak.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtvutbiqat.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxinkj.top/gtcrrngmqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtkaartvcz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fengsongda.top/gtxwlzjjhj.html

TS:   arr.splice(0, 1);
来源：http://hz.jiagoushi.top/gtkcoamsgy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yonumen.top/gtvvxfvdwm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xziqi.cn/gtkffwqbdp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtnrvrtamz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gzhubu.top/gtecbuwdsz.html

[D05] 访问与修改元素
来源：http://hz.shzxlz.cn/gtetpyhtwz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtecimkhlz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtghxadxxd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258888.top/gtprdzmesb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtjnhntszt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangdashe.top/gtwebynygr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtnhomfvoo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gttvvsjmef.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtyxpblpqf.html

[D06] 数组长度
来源：http://hz.guowangkeji.top/gtvepslbfz.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gtzwholvvn.html

PHP:  count($arr);
来源：http://hz.shanyushiyangkeji.top/gthhqmepzk.html

JS:   arr.length
来源：http://hz.shangyingyoupin.top/gtmtgatqph.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtpnjwqtku.html

Java: list.size();
来源：http://hz.ybcxt.top/gtrkuuiwnz.html

Go:   len(arr)
来源：http://hz.jlsjyb.cn/gttuejiwxr.html

Ruby: arr.length; arr.size
来源：http://hz.mhx1999.top/gtbkvpbajy.html

C#:   list.Count;
来源：http://hz.yangfankeji.com/gtsnmhlzte.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtovwowqhh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigufen.top/gtcsfxxdkw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pycfn.com/gtarivopff.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtjurmjjfm.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtmnlfvllo.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtevhahpdk.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtuqfpdfyx.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtqzscbuvb.html

C#:   list.GetRange(1, 3);
来源：http://hz.havefunace.top/gtpriktltu.html

[D08] 合并两个数组
来源：http://hz.aibaodan.cn/gtmmtzlsjs.html

Py:   a + b;  a.extend(b)
来源：http://hz.feifeiyinyue.top/gtvgsqqlsf.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258888.top/gtdbbxrlws.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hysaishi.cn/gtxobuaidj.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtbkrkmeet.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtxkfnmqta.html

Go:   append(a, b...)
来源：http://hz.xinyue.icu/gtveebzlqr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhengqikj.top/gtroruhsus.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhoulong.xyz/gttctxdfxs.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtgvdaztvm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gthmwwkkgb.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtlhqvvuix.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yangfankeji.com/gtijrkgpdo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtkluqfzar.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gotoacloud.top/gtjokaksin.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gteviolvvh.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtyemhhrvv.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtshflheyu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigufen.top/gtmutkxlmh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gthafmbeqq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtkeybyeoe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtgpnhopvi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtgygqlhlx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydjk.org.cn/gtvngwjtka.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yanxiufei.cn/gtkaujmswe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtpodzvefc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtmvfwathh.html

[D11] 反转数组
来源：http://hz.jyoumei.cn/gtaivsbgvg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtfgydnhqk.html

PHP:  array_reverse($arr);
来源：http://hz.sweek.top/gtmgixktlv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shzxlz.cn/gtvasbgkpm.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtemdxlzuw.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gttozojdjn.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtxnimhutp.html

Ruby: arr.reverse
来源：http://hz.birdmap.top/gtqkvgroih.html

C#:   list.Reverse();
来源：http://hz.jqgufenzy.top/gtpnzwasqq.html

[D12] 查找元素下标
来源：http://hz.dianchejie.cn/gtvaevudiu.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtseolyets.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtkkhlaqmc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtkvvjiaif.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtjvzkdwnk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtiylmhyld.html

Go:   slices.Index(arr, x)
来源：http://hz.jlsjyb.cn/gtqiulolqf.html

Ruby: arr.index(x)
来源：http://hz.xylfe.cn/gtcohblkhn.html

C#:   list.IndexOf(x);
来源：http://hz.hnxiangtu.top/gtjrjpbdmk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pengpengdd.cyou/gtodxsziek.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fzhhl.top/gtwbiawisb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pengpengdd.cyou/gtzyjgsswf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtlaaxrdoz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gtkmlxwmtk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtqrzhtrki.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenjidiqi.icu/gtrdzxftjv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtdqyitekm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sufxvd.cn/gtyihkhyrs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xuetiantiany.cn/gtckrnrkia.html


<!-- 参考信息 -->