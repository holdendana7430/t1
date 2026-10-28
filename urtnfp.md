代发 wailian999

Py:   if not data: return
来源：http://hz.feifeiyinyue.top/gtngpztpsj.html

PHP:  if (!$data) { return; }
来源：http://hz.zhengqikj.top/gtlyccydov.html

JS:   if (!data) return;
来源：http://hz.316326.xyz/gtfmprfvce.html

TS:   if (!data) return;
来源：http://hz.aizwys.cn/gtpzwxiltq.html

Java: if (data == null) return;
来源：http://hz.gogol.net.cn/gtdpvgsknn.html

Go:   if data == nil { return }
来源：http://hz.guannengcc.top/gtgcexshgi.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtwhyqxtqq.html

C#:   if (data == null) return;
来源：http://hz.jqgfzy.top/gtvfvklljd.html

================================================================================
来源：http://hz.ydzc1.top/gtxyxzckrl.html

C. 函数与作用域
来源：http://hz.gogol.net.cn/gtkfzxkcay.html

================================================================================
来源：http://hz.smart0.xyz/gtnxqnufzb.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtndmfwetm.html

Py:   def add(a, b): return a + b
来源：http://hz.hfpthk.cn/gttlttdsrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtagzanjwq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtcdldmwzv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtirayzwrq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtsrcsvsag.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.bjfxy.top/gtowavjzko.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guannengcc.top/gtolrcyeio.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtunqqcecf.html

[C02] 默认参数
来源：http://hz.gaohongyu789.top/gtievjeyzd.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258.top/gtprqedodz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gaohongyu789.top/gtaemlsukz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigufen.top/gtquoatcwk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yongpay.top/gtpfittaxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daria6918.cn/gtpxjnvbbl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aizwys.cn/gtrbfhckqp.html

Ruby: def greet(name = "World") = name
来源：http://hz.svipenyu.cn/gtdizqpyre.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sxryk.cn/gthgrlijcb.html

[C03] 可变参数
来源：http://hz.fzhhl.top/gtepwhzysx.html

Py:   def total(*args): return sum(args)
来源：http://hz.ybcxt.top/gtfwmtyxvg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangshuangyany.cn/gtamzherif.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtubavllpb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gotoacloud.top/gtvmcbnztc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhijiandao.cn/gtrgsoreln.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yongpay.top/gtarjbfeca.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tanke756.top/gtslaqisqb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.52xcode.cn/gttfqqwjbg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtwbeuuuph.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgfzy.top/gtlnattcdp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.guannengcc.top/gtbdhnmywr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtvsaoslwd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtgbjcjrmw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtyhyoqpni.html

Go:   // 无：用配置结构体参数
来源：http://hz.xingfuxueyuan.xyz/gtlfehzost.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtycbixeiy.html

C#:   f(a: 1, b: 2)
来源：http://hz.yonumen.top/gttgnhvbin.html

[C05] 返回多个值
来源：http://hz.shanyushiyangtech.top/gtbdrihqxi.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtzqvaunjl.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gthpbijczs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhiwuduotai.top/gtfmudgggg.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gtagedttlk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fengsongda.top/gtqcpindcj.html

Go:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtskrzgzbm.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtthibthor.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.quarkkingdee.top/gtlvmiqcoc.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtuhwmklza.html

Py:   square = lambda x: x * x
来源：http://hz.jinghuilouyu.cn/gtesxcdvnt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cheryme.top/gtcrgyzxqf.html

JS:   const square = x => x * x;
来源：http://hz.zycfv.cn/gtzlkvzlte.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtrvilubpv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cucudq.cn/gtohvxflrd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnxiangtu.top/gtstqtyako.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhijiandao.cn/gtzlmyfnzs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aibaodan.cn/gtebulnnor.html

[C07] 把函数作为参数传入
来源：http://hz.cashguo.top/gttidylfzz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtiasgyswx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtcpcyboui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jianghu66.top/gttpccdxfl.html

TS:   arr.map(String)
来源：http://hz.tianlin.xyz/gtcnjgeaec.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangdashe.top/gtkyaoajux.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuetiantiany.cn/gtpnrebndj.html

Ruby: arr.map(&:upcase)
来源：http://hz.andypj.xyz/gtqdnczfnu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.52xcode.cn/gtablyeoqo.html

[C08] 闭包
来源：http://hz.gzhubu.top/gttldqfspa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258.top/gtkqeftohp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gthyweirna.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtzqqpcevk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtfxwatbsq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jyoumei.cn/gtbiaadjcl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtofxlqajg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhaomingkeji.xyz/gtucaahbgj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtworssvyt.html

[C09] 递归
来源：http://hz.yj20258888.top/gtlyhkcquf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zycfv.cn/gtgydvitrh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtefnbtpiw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtoelocltv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtkyxxsahv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtjxpmmgdc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtmeudfgrw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ivvv.top/gtxtsrresh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gzhubu.top/gtwgommkje.html

[C10] 变量作用域
来源：http://hz.sweek.top/gtqhsuqwda.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtlocnbuzh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtopmtmhrb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtzczoxjwa.html

TS:   同 JS
来源：http://hz.yj20258.top/gtkmncgznd.html

Java: 方法内为块级作用域
来源：http://hz.gotoacloud.top/gtxajbjyvm.html

Go:   花括号块级作用域
来源：http://hz.mhx1999.top/gtvwmhwsiz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnqzz.top/gtevalxeku.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtjnyeegvb.html

[C11] 模块导入与导出
来源：http://hz.jinqigufen.top/gtpymlwufg.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gthxjdmscx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jlsjyb.cn/gtuknwlepb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.svipenyu.cn/gtgmamtqxn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sufxvd.cn/gtjcogopss.html

Java: import java.util.List;
来源：http://hz.zhijiandao.cn/gtluqgdtjj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ppjwa.cn/gtkjybripu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xylfe.cn/gtesvcnydp.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtmkvtlhqf.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtfkbivmii.html

Py:   (lambda: print("run"))()
来源：http://hz.yonumen.top/gtaqiesvse.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xziqi.cn/gthfxogrzv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtlwtokvuf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangshuangyany.cn/gtohpqreap.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtygzynwkv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtiobpljrh.html

Ruby: -> { puts "run" }.call
来源：http://hz.hongshengwenyu.top/gtzytllfde.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtarfytqzs.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtlcqhdvzf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtmxrvsxmm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtpmsdxkin.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtxoqhjddd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtnjibokzm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtbverqvtl.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtqyhrnnxe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhoulong.xyz/gtlabjixwo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daria6918.cn/gtfllkgojm.html

[C14] 泛型函数
来源：http://hz.birdmap.top/gtsjxkkgrq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtiuvwhjzt.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtbannhvon.html

JS:   // 无泛型
来源：http://hz.zdqjudy.top/gtknoqbxgp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nwbrower.top/gtauknzcql.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cdnleiting.top/gtvguelqbk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hammf.cn/gtdfmvvzfd.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangkeji.top/gteszcxuir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gtrzrvohdy.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gtyjmnrymd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenzaomai.com/gtqnusruix.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fengsongda.top/gtdqkohstc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhengqikj.top/gtrsphpbjd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhengqikj.top/gtzvzntsqu.html

Java: // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtugmiodxu.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtxiaragce.html

Ruby: a, b = pair
来源：http://hz.mhx1999.top/gtlwzsotnj.html

C#:   var (a, b) = pair;
来源：http://hz.ybcxt.top/gtaijtggjj.html

[C16] 函数 / 方法重载
来源：http://hz.hnqzz.top/gtmytugnaj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtnqwxkplk.html

PHP:  // 无重载
来源：http://hz.daria6918.cn/gteyuhqwkq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuanzx.com/gtmjgqvcys.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yanxiufei.cn/gtxpzizlhj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zdqjudy.top/gtrgkkoeol.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtwriowizx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.redwolf501.top/gthjatckfq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtawiwneky.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjsaghncv.html

D. 数组 / 列表 / 集合
来源：http://hz.sxryk.cn/gtqzohkybd.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtefrcsupx.html

[D01] 创建数组 / 列表
来源：http://hz.birdmap.top/gtekirixla.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gthflpgsjw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cdnleiting.top/gtffsfanlz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtffyfqogb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenlongwang.top/gtokchklhv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtjzmfydjl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtkvsjgfeb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtbmofoxfz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yongpay.top/gtrnwvwwut.html

[D02] 追加元素到末尾
来源：http://hz.shangyingyoupin.top/gtpxkzwkcx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtkfhwklbo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtcbsmvvoa.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtalkuoyxm.html

TS:   arr.push(4);
来源：http://hz.smart0.xyz/gtjlqmqdzp.html

Java: list.add(4);
来源：http://hz.c1oappe.top/gtpkbigbmw.html

Go:   arr = append(arr, 4)
来源：http://hz.xziqi.cn/gtlknsonwd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gttputvfma.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtvnodnvdu.html

[D03] 在指定位置插入元素
来源：http://hz.zhiwuduotai.top/gtcjnqcqsl.html

Py:   arr.insert(0, 0)
来源：http://hz.cashguo.top/gtrlgjfsox.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.snrcjt.cn/gtqgaxfdfu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hfpthk.cn/gtlelkpyik.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtwfzhbscq.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gtguxryqbm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtdgudewal.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gtieeknlqa.html

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gtbdsaujwp.html

[D04] 删除元素
来源：http://hz.gaohongyu789.top/gtxfoysxpb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shangyingyoupin.top/gtqcjaahdi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtyeyhxyht.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zdqjudy.top/gtrfqctzeu.html

TS:   arr.splice(0, 1);
来源：http://hz.ywan-chungtsiang.top/gtpljzygam.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.316326.xyz/gtpojtmeqw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gttqgtxfpy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtezibjobi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnxiangtu.top/gtwbbuwcqs.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtjzrojxpf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gtclkrwjdo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ybcxt.top/gtkboqrilv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtatxcqlje.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtjkzkejlr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtgjvwzvif.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtrrkmwrif.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtrvxkgrmt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gtzdyiltoh.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gteqlcyscu.html

Py:   len(arr)
来源：http://hz.yj202588.top/gthgdjjklb.html

PHP:  count($arr);
来源：http://hz.guannengcc.top/gtntprrjjm.html

JS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtlaqgysmc.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtmnuoiayr.html

Java: list.size();
来源：http://hz.shangyingyoupin.top/gtiafzhufv.html

Go:   len(arr)
来源：http://hz.svipenyu.cn/gtwkwgaybj.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gtlmqqxyje.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtqazbglaq.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtbqafgraq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gtryyqndsb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xylfe.cn/gtrbinmvxb.html

JS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtmcitqpoz.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtikrmppck.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtatbwpzqh.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtoxxtowkl.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtoneufykv.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenzaomai.com/gtnufnobtc.html

[D08] 合并两个数组
来源：http://hz.meibo888.top/gtvyqzcwre.html

Py:   a + b;  a.extend(b)
来源：http://hz.jiagoushi.top/gtclsftlhs.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtcleadiwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtnpialxxh.html

TS:   [...a, ...b];
来源：http://hz.yj20258.top/gtrcplxbxx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtqlvbvvua.html

Go:   append(a, b...)
来源：http://hz.guannengcc.top/gtggnqlnjk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sufxvd.cn/gtnmhtmetn.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtoflvzhqd.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtqwbjelca.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtoecvztmi.html

PHP:  sort($arr);
来源：http://hz.yj202588.top/gtpbxtwvcd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jlsjyb.cn/gthmmwxjgk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtvexiojpo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtjqhuphza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtndzqkmqr.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtvqtaiumx.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtnhpemgjk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dashuyun.cn/gtpeniwnfa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.mhx1999.top/gtkcjslbdm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtkkifcdnp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtemntwfuf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtoiafmvqr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtakjosmlc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtwtpltpzy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangshuangyany.cn/gttwbvmtnf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gtfnfhgwpe.html

[D11] 反转数组
来源：http://hz.zdqjudy.top/gtabaqbzer.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtwgksuoyo.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtsgckeifk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtueiysxbk.html

TS:   [...arr].reverse();
来源：http://hz.jinghuilouyu.cn/gtnggefkgh.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtcfjjyygn.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gtujlqqrdj.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangkeji.top/gtdaclocbt.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtinolocka.html

[D12] 查找元素下标
来源：http://hz.guowangkeji.top/gtxodauncj.html

Py:   arr.index(x);  x in arr
来源：http://hz.ppjwa.cn/gtmedsuigd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtqlqbdbkh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtpnxpxicw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtklkzxfyf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuanzhike.top/gtqiwwxmew.html

Go:   slices.Index(arr, x)
来源：http://hz.sxryk.cn/gtcrbzideh.html

Ruby: arr.index(x)
来源：http://hz.hongshengwenyu.top/gtwaokyonz.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gtqjxwroph.html

[D13] 过滤（保留满足条件的）
来源：http://hz.quarkkingdee.top/gtqteiqocb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tian-w.cn/gtlwywzrai.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yangfankeji.com/gtpgoszcjr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtbdmlzftw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtuagqulmc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtywdxcmot.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xinyue.icu/gtkyxdhfpj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yonumen.top/gtdmnjjlzr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ppjwa.cn/gtbmlctfqo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.havefunace.top/gtkpbjgpwb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtracougtw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtvfrbnoiy.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtnbcbgipa.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtnxfntacm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gttwccddta.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gteeyqwyqu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhiwuduotai.top/gtatyqoexb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtpbvxtoai.html

[D15] 去重
来源：http://hz.cashguo.top/gtcjfhvkzc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yvedp.cn/gtpsehpoiw.html

PHP:  array_unique($arr);
来源：http://hz.hywenlv.cn/gtrvitjxlm.html

JS:   [...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtronihhhl.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtreswziih.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhixingplan.top/gtlgjiiasj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.feifeiyinyue.top/gtffxnfwpm.html

Ruby: arr.uniq
来源：http://hz.guannengcc.top/gtlkckcmip.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtvqqrdjhr.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangkeji.top/gtixyyubya.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtdooaplwn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gttwojmycb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtfiwpbnhm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtibertdja.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtzhhwlxjg.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtthkanqwm.html


<!-- 参考信息 -->