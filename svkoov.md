代发 wailian999

================================================================================
来源：http://hz.meibo888.top/gtsqmadnps.html

C. 函数与作用域
来源：http://hz.yuxming.cn/gtjfatveio.html

================================================================================
来源：http://hz.havefunace.top/gtbspdfxmd.html

[C01] 定义函数
来源：http://hz.kuanghao11.cn/gtymspijux.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtrlfvxtho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtvkzgniht.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.redwolf501.top/gtfxufpgmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtsbswvses.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtiqvotdhj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nwbrower.top/gtswhyyhex.html

Ruby: def add(a, b); a + b; end
来源：http://hz.316326.xyz/gtxprzsvfn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtmximzlnb.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gthxnjzskw.html

Py:   def greet(name="World"): return name
来源：http://hz.daria6918.cn/gtfiqjyigp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnxiangtu.top/gtimcsgfne.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pycfn.com/gtqadkdpzs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtgajshkkj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.quarkkingdee.top/gthlafqyma.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tanke756.top/gtdqklkonq.html

Ruby: def greet(name = "World") = name
来源：http://hz.yj20258888.top/gtaldlyjzk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtqfaixzkq.html

[C03] 可变参数
来源：http://hz.cashguo.top/gtgjdidcpy.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydjk.org.cn/gtrrbgdlbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhaomingkeji.xyz/gtsezqevof.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtbesxyaxd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtirwstnve.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gthsgnnnol.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gtneojjhtj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fengsongda.top/gtmugrjsmb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj20258888.top/gtfifaefml.html

[C04] 命名参数 / 关键字参数
来源：http://hz.chenzaomai.com/gtjvkbecia.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xingfuxueyuan.xyz/gteowynfow.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nwbrower.top/gtglmsvoss.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtpkwieibq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.iojbl.cn/gtcpnfkfgj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gthjzpbolu.html

Go:   // 无：用配置结构体参数
来源：http://hz.dianchejie.cn/gtuglaekkn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtaffglydv.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtsnhftpam.html

[C05] 返回多个值
来源：http://hz.yj20258888.top/gtbeosismz.html

Py:   return a, b
来源：http://hz.sysykeji.top/gtdblisbjs.html

PHP:  return [$a, $b];
来源：http://hz.xingfuxueyuan.xyz/gtheurwoan.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xuanzx.com/gtotpnxtyx.html

TS:   return { a, b };
来源：http://hz.meibo888.top/gtjvrojqqg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtrldlxbtj.html

Go:   return a, b
来源：http://hz.zhongyouzk.top/gtsmjqecto.html

Ruby: return a, b
来源：http://hz.yanxiufei.cn/gtgemosjwr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gtnsdrheyc.html

[C06] 匿名函数 / lambda
来源：http://hz.xziqi.cn/gtphdivuwz.html

Py:   square = lambda x: x * x
来源：http://hz.shangyingyoupin.top/gtcbvumgak.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ydzc1.top/gtntucppbe.html

JS:   const square = x => x * x;
来源：http://hz.andypj.xyz/gtkpoikyvj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shuidangran.top/gtdlssqbof.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shuidangran.top/gtteymwsme.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pengpengdd.cyou/gtkpzumcpe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cucudq.cn/gtxeomdnnl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhongyouzk.top/gtuokywtab.html

[C07] 把函数作为参数传入
来源：http://hz.hysaishi.cn/gttvglwevu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yonumen.top/gtlgdcggki.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aizwys.cn/gtujhvwifu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtgibrawps.html

TS:   arr.map(String)
来源：http://hz.guannengcc.top/gtjqvbluml.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnxiangtu.top/gtbojhlcka.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gtudkumjmj.html

Ruby: arr.map(&:upcase)
来源：http://hz.ywan-chungtsiang.top/gtuhizdmtz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenjidiqi.icu/gtntadmhmg.html

[C08] 闭包
来源：http://hz.52xcode.cn/gtrogfsbba.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtracvvbgi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.9152youxi.cn/gtczsrpstl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtzjtbetbo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtjviprwkz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aizwys.cn/gtbqnvoyya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cheryme.top/gtluerwmxt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhoulong.xyz/gtbvmhyqom.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtodjyymij.html

[C09] 递归
来源：http://hz.52xcode.cn/gtvedeoefg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtzdhfqrfp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hywenlv.cn/gtqgamcwjk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cqqwz.cn/gtmtkmwncv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtllwuutso.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhengqikj.top/gtlqpwwzzt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sysykeji.top/gtxxwsqkvs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtzoaloghc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xinyue.icu/gtdshbfbst.html

[C10] 变量作用域
来源：http://hz.xingfuxueyuan.xyz/gtmdqvocho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtrecqkcma.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jiagoushi.top/gtvhrdmhko.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtytxfnaup.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtiqhmqdab.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtygtuolqw.html

Go:   花括号块级作用域
来源：http://hz.snrcjt.cn/gtbfqwvahf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.mhx1999.top/gtrswhnoqy.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtaetnvyqb.html

[C11] 模块导入与导出
来源：http://hz.9152youxi.cn/gtybxrbcco.html

Py:   from module import func
来源：http://hz.hysaishi.cn/gttboiiogi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hammf.cn/gtpczdpyjn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jianghu66.top/gtzpbgybbr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xziqi.cn/gtxbcjqfgg.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gthaospjso.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxinkj.top/gtxgkesmsw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ppjwa.cn/gteemxjsnm.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtaxygzmku.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gtxzbtbqvm.html

Py:   (lambda: print("run"))()
来源：http://hz.0kj1m.cn/gtiokxokit.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangtech.top/gtqgoxywya.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtthwmejlf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtzvacyyio.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgufenzy.top/gtkxtaptmu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtxdmpgfoe.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gttuyxketu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtekawbdqd.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gtrmwgjqes.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtrwjjhxgs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtwxmqlnkh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gaohongyu789.top/gtvffqvsox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtenlrerry.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gttqzixumz.html

Go:   func add(a, b int) int
来源：http://hz.guowangkeji.top/gtgqcfqivo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.redwolf501.top/gtpkxtlref.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hywenlv.cn/gtgpnobkhx.html

[C14] 泛型函数
来源：http://hz.hnqzz.top/gtnvgjgajq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhijiandao.cn/gtvmjrxcen.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtlbmmmlzu.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gtqxzotgzf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gthvfgigof.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtrdqrijkf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gtlqleyopt.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtkzwdylez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhengqikj.top/gtarhnngal.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtysazdpoq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtiwzvktmr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtzjowjwok.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtybwpicvn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tianlin.xyz/gtghjdqzyi.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtesagefrv.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtblurvoaz.html

Ruby: a, b = pair
来源：http://hz.hywenlv.cn/gtngqeeluc.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtfcdqtoeg.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gttfhchhhi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtmjpwarhc.html

PHP:  // 无重载
来源：http://hz.hongshengwenyu.top/gtoymgogpj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nwbrower.top/gtojzrbhtj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtmghbmmnr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtyofmultl.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtotqqzogw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhaomingkeji.xyz/gtzfpmjyqn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cdnleiting.top/gtbzsfgbfb.html

================================================================================
来源：http://hz.haohaochexian.top/gtohubbjca.html

D. 数组 / 列表 / 集合
来源：http://hz.cucudq.cn/gtfpjxodlb.html

================================================================================
来源：http://hz.zhixingplan.top/gtqiaznxva.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtydiaagug.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.haohaochexian.top/gtnhcmicqb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhaomingkeji.xyz/gtrqrmkbaw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtfvcsomsg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtolasgyzf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gtcagfrhxo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtfxmsxhhl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtmwbearqy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtrdcdwppq.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gttrzhnubs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtkuhrjahs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gtxncyjgxd.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtbdsoxjrr.html

TS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtyyobfxtx.html

Java: list.add(4);
来源：http://hz.sysykeji.top/gtasryajco.html

Go:   arr = append(arr, 4)
来源：http://hz.xingfuxueyuan.xyz/gtubdlehct.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jiagoushi.top/gtwrzfgggl.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtoavxqdvh.html

[D03] 在指定位置插入元素
来源：http://hz.gogol.net.cn/gtkwhpxych.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtdimvikwx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hfpthk.cn/gtjlqmoyra.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gtqtkfwtfe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenjidiqi.icu/gtzfurbsfw.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtcqvhjisa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gtgbduxnck.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuanzhike.top/gtnzvjdjzk.html

C#:   list.Insert(0, 0);
来源：http://hz.ybcxt.top/gtcczoqzot.html

[D04] 删除元素
来源：http://hz.shangyingyoupin.top/gthaxwjdbv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtrycrjmjx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhiwuduotai.top/gtdjpgspme.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinyuanbaomall.cn/gtcnrgmaxd.html

TS:   arr.splice(0, 1);
来源：http://hz.jiagoushi.top/gtayhajdqu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cashguo.top/gtztaocbvk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj202588.top/gtxvjelfha.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xinyue.icu/gtvwlcztrq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daxiang520.top/gterqbnucq.html

[D05] 访问与修改元素
来源：http://hz.shzxlz.cn/gtweqnjwwh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtaeizvznc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gtgrljfyxn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtrowzuzga.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.birdmap.top/gteteqxwcg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenlongwang.top/gtdhkehvwg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtvsdumnkd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gthaosuxax.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtwczmsrsz.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtazhliivs.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtvsfubprp.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtrxjxclni.html

JS:   arr.length
来源：http://hz.iojbl.cn/gtfcqypbsz.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtryqqztzy.html

Java: list.size();
来源：http://hz.tanke756.top/gtfvxwolpy.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gtsjiiwarw.html

Ruby: arr.length; arr.size
来源：http://hz.ppjwa.cn/gtzysweqrl.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtswspyglq.html

[D07] 切片 / 取子数组
来源：http://hz.aizwys.cn/gtstlwpqhn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtlvlurihi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cashguo.top/gtocyoyiki.html

JS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gtzjbtcybo.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtbkgusmih.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtjfnagfnd.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtjlwndvlv.html

Ruby: arr[1, 3]
来源：http://hz.dashuyun.cn/gtyfemgjwg.html

C#:   list.GetRange(1, 3);
来源：http://hz.sxryk.cn/gtejolrncd.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtpnijloap.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gtpgeyvvys.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtxvwhyhls.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.c1oappe.top/gtokotybvs.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gtukpzpyut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtbztffjyi.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtewrpqaap.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xylfe.cn/gtrkzlamxs.html

C#:   a.Concat(b).ToList()
来源：http://hz.cashguo.top/gtbuybvsro.html

[D09] 排序（升序）
来源：http://hz.tian-w.cn/gtysyhxntk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtegpiqrbs.html

PHP:  sort($arr);
来源：http://hz.nanxinkj.top/gtzwfodrva.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gtcupzipvv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gttrkeohxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtqytgqxxl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xinyue.icu/gtyfeuabdp.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtstlfytvr.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtcvqktthy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gtgarmsvvd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtegdqbvey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtitooivkp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtapaeiyyh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtxmwopobt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ivvv.top/gtnfoyavpq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnxiangtu.top/gtfkbxfane.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.pengpengdd.cyou/gtttkvxivx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daxiang520.top/gtjpjzvwku.html

[D11] 反转数组
来源：http://hz.zhongyouzk.top/gtotzudhfl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.daria6918.cn/gtlfaevvyb.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtlzototxi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zycfv.cn/gtuxooeiqu.html

TS:   [...arr].reverse();
来源：http://hz.yangfankeji.com/gtvayrpplo.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtcjxyfzao.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gttxfgmpnn.html

Ruby: arr.reverse
来源：http://hz.yj20258888.top/gtdfvtoced.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtgtkjjfdh.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtqokoxuat.html

Py:   arr.index(x);  x in arr
来源：http://hz.shzxlz.cn/gtscdfmppb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuetiantiany.cn/gtebetvvqv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtuxsnmzue.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtgrzaasnh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hywenlv.cn/gtgfbgxywj.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtlbbfdvlc.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangkeji.top/gtgxqiyvtk.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtaldhltkg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fengsongda.top/gtrcqfxpno.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtrozyjsuw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtxnausjmj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtqcconzvq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtfvgzlgdq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtyvoydsvf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenlongwang.top/gtlemomppr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gogol.net.cn/gtovqhshhf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuetiantiany.cn/gttgtmbpbr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigufen.top/gtkjjkuhjw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtmurqrdzs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jianghu66.top/gtjenslkdd.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtlrnuwnbs.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtusspjjfb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cqqwz.cn/gtmqtnwhis.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtsbvwqign.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtqqzymhvt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangshuangyany.cn/gtqgvtbloc.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtaqxkrzhj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gthuipnuqo.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangkeji.top/gtwscpznrd.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtaezpyoqa.html

TS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtcfyahuna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtzdgnkvje.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtiynlgelw.html

Ruby: arr.uniq
来源：http://hz.zdqjudy.top/gtjsrzxmof.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtrpovruhc.html

[D16] 求和与平均值
来源：http://hz.jqgufenzy.top/gtpndrcuux.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhixingplan.top/gtmzwlelse.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtboqzwlrn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtukuvipzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtafshkinz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtwarwrgar.html

Go:   // 手写循环累加
来源：http://hz.gogol.net.cn/gtswandktp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtbkgqegsm.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtafaqlbml.html

[D17] 最大值与最小值
来源：http://hz.jinghuilouyu.cn/gtrdhghxfv.html

Py:   max(arr);  min(arr)
来源：http://hz.cqqwz.cn/gtnvyjigim.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhongyouzk.top/gtkjdymbai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.feifeiyinyue.top/gtzxzymprd.html

TS:   Math.max(...arr);
来源：http://hz.shzxlz.cn/gtwgcymjfp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.kuanghao11.cn/gtgkstiaym.html


<!-- 参考信息 -->