代发 wailian999

================================================================================
来源：http://hz.cqqwz.cn/gthqppqzrp.html

C. 函数与作用域
来源：http://hz.316326.xyz/gtytngpwbl.html

================================================================================
来源：http://hz.jqgfzy.top/gtiweetttu.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtmhxekfsf.html

Py:   def add(a, b): return a + b
来源：http://hz.pengpengdd.cyou/gteofmitnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtodbnljsg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtcsjxabmv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gthgzgpkai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtfrczqupb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxuanxn.top/gtlaebclkc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zdqjudy.top/gtezsyqvvj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtqvmewfbr.html

[C02] 默认参数
来源：http://hz.yonumen.top/gtaltlzktw.html

Py:   def greet(name="World"): return name
来源：http://hz.hnxiangtu.top/gtmovifwkf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yueranfly.top/gtnwpxszfl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sufxvd.cn/gtuccmmsmq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jianghu66.top/gtigttgqaq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tianlin.xyz/gtitrxmdzm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtuiqutfve.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtipfgqasg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pycfn.com/gtakayywyu.html

[C03] 可变参数
来源：http://hz.ywan-chungtsiang.top/gtmuoapukz.html

Py:   def total(*args): return sum(args)
来源：http://hz.jianghu66.top/gtzhxzgbam.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.kuanghao11.cn/gtekgyxule.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtdkcnoenn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtkwiphvbe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.wangdashe.top/gtbzqwfwlu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cucudq.cn/gtoslqaqdt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gotoacloud.top/gtlaqddfla.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtjufqtelc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgfzy.top/gthhgvnqlq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xylfe.cn/gtpestcrtq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gogol.net.cn/gtvnjvnhuy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tanke756.top/gtgvkjhigo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gtwaiyxtns.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gtervdqtbu.html

Go:   // 无：用配置结构体参数
来源：http://hz.vqdsnc.cn/gtfziozzzh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtgxuakkxw.html

C#:   f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtbajstwfw.html

[C05] 返回多个值
来源：http://hz.jianghu66.top/gteugyydak.html

Py:   return a, b
来源：http://hz.gogol.net.cn/gtujbvimnx.html

PHP:  return [$a, $b];
来源：http://hz.dianchejie.cn/gtbbttkutj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtponciufl.html

TS:   return { a, b };
来源：http://hz.jqgufenzy.top/gtdgvmgrcs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtgbvolufe.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtuvllwllz.html

Ruby: return a, b
来源：http://hz.yuanzhike.top/gtwdxqzcnk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtwtessqzk.html

[C06] 匿名函数 / lambda
来源：http://hz.aibaodan.cn/gthhpnurnn.html

Py:   square = lambda x: x * x
来源：http://hz.xuetiantiany.cn/gtvroetyhf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gogol.net.cn/gtovalhxxs.html

JS:   const square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtcombsxna.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shanyushiyangtech.top/gtulusbqcy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xingfuxueyuan.xyz/gtjeadriuh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.meibo888.top/gtbvarcmme.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydzc1.top/gtlrcuzhax.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hfpthk.cn/gtbtdxzlez.html

[C07] 把函数作为参数传入
来源：http://hz.ivvv.top/gtupdbqeqp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daxiang520.top/gtesdhyvmz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dianchejie.cn/gtumliwyzo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sweek.top/gtvllyvznv.html

TS:   arr.map(String)
来源：http://hz.quarkkingdee.top/gtthquvizf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gaohongyu789.top/gtsjnvzeey.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.svipenyu.cn/gtulsucyqi.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangkeji.top/gthcimtqiy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.pycfn.com/gtucfabnaa.html

[C08] 闭包
来源：http://hz.ehwqpu.com/gtlwmbwajj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jiagoushi.top/gttorqefib.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtdsynlryo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtleaovwhn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtkazbgfwi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.guowangkeji.top/gttexxyqeb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtlnjncfus.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj202588.top/gtwhelgcvs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtdvhcylqe.html

[C09] 递归
来源：http://hz.aizwys.cn/gtloterthl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtdyepjvgj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.haohaochexian.top/gtwqoemsqo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtyuqyxtdj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtdthecpwu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtqnnpgjjc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gtrkdlhcvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtgnhjtjya.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtvfeyquxq.html

[C10] 变量作用域
来源：http://hz.birdmap.top/gtgsqjgvwf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258888.top/gtpepigori.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtrmllkzgi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtdczqpwqa.html

TS:   同 JS
来源：http://hz.nanxinkj.top/gtpdsthalk.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtacuubura.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gtbvrgepos.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ybcxt.top/gtlxbvwmyp.html

C#:   块级作用域
来源：http://hz.gaohongyu789.top/gtjqbaecon.html

[C11] 模块导入与导出
来源：http://hz.guannengcc.top/gtrqkgeesv.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtvatswpll.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtffdlbyvo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cdnleiting.top/gtnajmulzw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jlsjyb.cn/gtqdloehst.html

Java: import java.util.List;
来源：http://hz.feifeiyinyue.top/gtlrhmanxo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtkqlvguzl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhixingplan.top/gthlxdyims.html

C#:   using System.Text;
来源：http://hz.ydzc1.top/gtlhximybe.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258888.top/gthnqcmywc.html

Py:   (lambda: print("run"))()
来源：http://hz.fengsongda.top/gtldxaoirs.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangtech.top/gtblwkcasi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtesbfkbeg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtctobrbjc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gtykffolgl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aibaodan.cn/gtfmfsyxiv.html

Ruby: -> { puts "run" }.call
来源：http://hz.dashuyun.cn/gttdczdqbh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.snrcjt.cn/gtdrifgcos.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtdyvtpfuv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtyasdpkyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtedneqbkj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sxryk.cn/gtxwhvbqgt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtikzzeuiu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtfhlkjveb.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gtsblkevgg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtdrhrgfge.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.snrcjt.cn/gtbokymluk.html

[C14] 泛型函数
来源：http://hz.xuanzx.com/gtbbnmomfi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gthaqgclmz.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gteggnzhjk.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gtvcnlajlv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxuanxn.top/gtbqhrjtif.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtfnvninny.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cdnleiting.top/gtqdmuwjxc.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtfwdlynzp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtxrxgrfkk.html

[C15] 解构 / 展开参数
来源：http://hz.cashguo.top/gtihokcxqf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtgzinyimm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cqqwz.cn/gtlpswywtx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtszyeqcql.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gteqfjnrye.html

Java: // 无解构
来源：http://hz.hfpthk.cn/gtijumxazv.html

Go:   // 无解构
来源：http://hz.tian-w.cn/gtjwrjyvul.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gthfwnbegd.html

C#:   var (a, b) = pair;
来源：http://hz.hysaishi.cn/gtukvfnhxw.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtmmdfzoqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ppjwa.cn/gtrnfggjvh.html

PHP:  // 无重载
来源：http://hz.cdnleiting.top/gtzhxaqdom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtxbjnfmlh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gtiubtuhbq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.0kj1m.cn/gtjxmddgom.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj202588.top/gtaawagjdd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.52xcode.cn/gtacczpqie.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtdklxqxbw.html

================================================================================
来源：http://hz.xinyue.icu/gtzhznxjue.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtswitupdu.html

================================================================================
来源：http://hz.aibaodan.cn/gtbfpoygln.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtmnuqbupy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gteziawytt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.9152youxi.cn/gtwgjgkzqs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cdnleiting.top/gtjkxwrjzc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.snrcjt.cn/gtvfzdhxcv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xziqi.cn/gtnkzpumog.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxuanxn.top/gtvrdlehgn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtzvcdwhpk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.redwolf501.top/gtnmlksxqi.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtbyihxsnf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gtjlxwhjql.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuxming.cn/gtyffgfbvk.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtpveuivcw.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtttbhhiad.html

Java: list.add(4);
来源：http://hz.hfpthk.cn/gtrkpjgtda.html

Go:   arr = append(arr, 4)
来源：http://hz.cashguo.top/gtpsvgrvbc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhijiandao.cn/gtxxmufwuh.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtuecwguzj.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtfimqbagc.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtnhdbnpfb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhongyouzk.top/gtlyzcocdd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtmcxnfery.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.smart0.xyz/gttkhtypcp.html

Java: list.add(0, 0);
来源：http://hz.yongpay.top/gtgqbtkbas.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtkhyxamxi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.quarkkingdee.top/gtskpxtcni.html

C#:   list.Insert(0, 0);
来源：http://hz.hammf.cn/gtggvjnkdc.html

[D04] 删除元素
来源：http://hz.shanyushiyangkeji.top/gtddhbymbh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jyoumei.cn/gtpplsppny.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuanzhike.top/gtrtfkaabu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtcntdbpom.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtfifkjysa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hfpthk.cn/gttbmluyel.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtqkelycmi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gthqocinqw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sufxvd.cn/gttqpgazzi.html

[D05] 访问与修改元素
来源：http://hz.0kj1m.cn/gtjmrkphnw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtkqubdieg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtnhoilhbx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtnllrqmit.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtqdaocdbg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yangfankeji.com/gtsvjvjrpl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gthryvhshh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtmuygookz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuanzx.com/gtjcxfripn.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gtqmhrivpm.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtbvjxrozw.html

PHP:  count($arr);
来源：http://hz.haohaochexian.top/gtskxfskiw.html

JS:   arr.length
来源：http://hz.xylfe.cn/gtqsvlxkgk.html

TS:   arr.length
来源：http://hz.fzhhl.top/gttfhckell.html

Java: list.size();
来源：http://hz.hnqzz.top/gtoqwzayfz.html

Go:   len(arr)
来源：http://hz.shangyingyoupin.top/gtljciolzr.html

Ruby: arr.length; arr.size
来源：http://hz.iojbl.cn/gtlijsjejy.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtlwufazxg.html

[D07] 切片 / 取子数组
来源：http://hz.havefunace.top/gtcpzmhvne.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtmcrlrpui.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtgqrkyfhx.html

JS:   arr.slice(1, 4);
来源：http://hz.vqdsnc.cn/gtzbfttfcu.html

TS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtyolzjuim.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtyvouqsud.html

Go:   arr[1:4]
来源：http://hz.cashguo.top/gtniqbabjy.html

Ruby: arr[1, 3]
来源：http://hz.52xcode.cn/gtxirhwlmw.html

C#:   list.GetRange(1, 3);
来源：http://hz.birdmap.top/gtkmudombp.html

[D08] 合并两个数组
来源：http://hz.jqgufenzy.top/gtzakwrhdq.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtkvureeuz.html

PHP:  array_merge($a, $b);
来源：http://hz.sufxvd.cn/gtnfhmlacz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtcqiqktlx.html

TS:   [...a, ...b];
来源：http://hz.yj202588.top/gtjqryibqv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.haohaochexian.top/gtplpqacnp.html

Go:   append(a, b...)
来源：http://hz.ywan-chungtsiang.top/gtmeozhkqv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.snrcjt.cn/gtsvrktffb.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtddroiknc.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtrjbjqtsj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtdmqahajv.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtfumasbvu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.haohaochexian.top/gtudthnmdv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtwyxhgxlz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.snrcjt.cn/gtgbqfptcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtdiqtgdra.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtyhvcdkjm.html

C#:   list.Sort();
来源：http://hz.yonumen.top/gtclmvpbzr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtmfhssomm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gtvtpfumsz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtnxuuyebs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtdawtofny.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtgljzywle.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gttffxdubr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sysykeji.top/gttlcxbapl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhixingplan.top/gtuwspafox.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daria6918.cn/gteofviukw.html

[D11] 反转数组
来源：http://hz.andypj.xyz/gtnmwsvhhw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgufenzy.top/gtxvihtdyu.html

PHP:  array_reverse($arr);
来源：http://hz.316326.xyz/gtpkhscmfy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtdshxppdd.html

TS:   [...arr].reverse();
来源：http://hz.fzhhl.top/gtjitxxapu.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtbpekfxnc.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtwrslmkeb.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtqbnwqxrp.html

C#:   list.Reverse();
来源：http://hz.zhijiandao.cn/gtuagjqxha.html

[D12] 查找元素下标
来源：http://hz.jinghuilouyu.cn/gtyukykdmx.html

Py:   arr.index(x);  x in arr
来源：http://hz.sweek.top/gtsdhskioh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuetiantiany.cn/gtpmnfhhph.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.smart0.xyz/gtacrqoibl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtlyecjbpr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cheryme.top/gtbecnydao.html

Go:   slices.Index(arr, x)
来源：http://hz.chenzaomai.com/gturehwryl.html

Ruby: arr.index(x)
来源：http://hz.pycfn.com/gttmvcqmww.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtmclypklw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cheryme.top/gtmnzbrvui.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtkfsfptza.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigfzy.top/gttydotnhc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtveqhlfah.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtjgzioqps.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258888.top/gtwlwsyefx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jyoumei.cn/gtshptvfkq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtzsedpehm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tian-w.cn/gtievqtqwt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.smart0.xyz/gtciyoyjei.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gotoacloud.top/gtgjyqmzib.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangkeji.top/gtvfsafruj.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtiqivvvxr.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtudmiwstc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gtyzcsvipm.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtvxinhnoq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtldhljboc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gtieykqmgd.html

[D15] 去重
来源：http://hz.xinyue.icu/gtfmrdoamn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtljpahsix.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtgfnoryzk.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtabfgbmsm.html

TS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtjjtlndpl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhoulong.xyz/gtdowjohhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhijiandao.cn/gtxsbxqfgf.html

Ruby: arr.uniq
来源：http://hz.9152youxi.cn/gtuzzjwcei.html

C#:   list.Distinct().ToList()
来源：http://hz.shzxlz.cn/gtlgjcouzl.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtlryjwjpf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.iojbl.cn/gtsuflnisb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhoulong.xyz/gtwqvkhhoe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtehveleap.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtrnctdoyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtklnlojit.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtuxggrlaj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dianchejie.cn/gttwycnebj.html

C#:   list.Sum();  list.Average()
来源：http://hz.fzhhl.top/gthouuvbhe.html

[D17] 最大值与最小值
来源：http://hz.yvedp.cn/gtshdeddoo.html

Py:   max(arr);  min(arr)
来源：http://hz.zhixingplan.top/gtwjuqvmkc.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuxming.cn/gtrhkzuqqx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ybcxt.top/gtoqdkucul.html

TS:   Math.max(...arr);
来源：http://hz.316326.xyz/gtpltbmxps.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtbtfcxesr.html


<!-- 参考信息 -->