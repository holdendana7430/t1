代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cashguo.top/gtrgdbfesp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yongpay.top/gtlgaoicbv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtsgnjfnvz.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtbmocgazj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtlqycffmx.html

[C03] 可变参数
来源：http://hz.shangyingyoupin.top/gtyqbliynu.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtfqzkmspf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtdwmmmaqx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtjywappwm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtjrhmbcgu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenlongwang.top/gtpmnikfxw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.iojbl.cn/gtgakebxbo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gogol.net.cn/gtegqutxvn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.svipenyu.cn/gtrzstwbmy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.vqdsnc.cn/gtzlwcaava.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.quarkkingdee.top/gtjmmhognz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nanxinkj.top/gtodqrxrrj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtpfanyivy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtkpcflghi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.dashuyun.cn/gtmectvmkr.html

Go:   // 无：用配置结构体参数
来源：http://hz.tian-w.cn/gtzgneuzam.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtvaqksfpd.html

C#:   f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtyieludqe.html

[C05] 返回多个值
来源：http://hz.tian-w.cn/gtsblwmsru.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtwccxlell.html

PHP:  return [$a, $b];
来源：http://hz.hywenlv.cn/gtmvginntq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenjidiqi.icu/gtfueqykyw.html

TS:   return { a, b };
来源：http://hz.birdmap.top/gtxicgujsc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fzhhl.top/gtxdcywafg.html

Go:   return a, b
来源：http://hz.zhijiandao.cn/gtvoboajvr.html

Ruby: return a, b
来源：http://hz.xuetiantiany.cn/gtujxlbnyh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shuidangran.top/gtxbzxbavd.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtohtjpqfc.html

Py:   square = lambda x: x * x
来源：http://hz.mhx1999.top/gtttvslyga.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.kuanghao11.cn/gthvyrmcbq.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtaqjkvvyt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgfzy.top/gthdmxueqo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gthhfhzqgb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hammf.cn/gtenxmvhor.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tanke756.top/gtitpomoun.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtvbjewrvx.html

[C07] 把函数作为参数传入
来源：http://hz.yonumen.top/gtsxsuemgg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtzdvpwqnp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtciyqkeau.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhaomingkeji.xyz/gttpoxgobg.html

TS:   arr.map(String)
来源：http://hz.hongshengwenyu.top/gtdrdatusj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.vqdsnc.cn/gtoldadttl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtujoluucn.html

Ruby: arr.map(&:upcase)
来源：http://hz.ehwqpu.com/gtgykyctpf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nanxuanxn.top/gtyvfdvfus.html

[C08] 闭包
来源：http://hz.zhixingplan.top/gtjrrhwwha.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gogol.net.cn/gtbcvkslel.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.redwolf501.top/gtdivzollw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtwxixuauz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtjakaczfo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.havefunace.top/gtidciguyw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtmkaxbgzj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtaxdqqywu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtoiadmfcr.html

[C09] 递归
来源：http://hz.quarkkingdee.top/gtrbgfnsdb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ybcxt.top/gthnhucaqy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtqwsskdjf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtiihinvyk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtkkbitkap.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jlsjyb.cn/gtjbvipfzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenjidiqi.icu/gtsxxqccuv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gtrrmheuhi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuetiantiany.cn/gtbivanzbh.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gthspzjiyh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtdagmnzch.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xingfuxueyuan.xyz/gtdordskbl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yonumen.top/gtjcpcyuls.html

TS:   同 JS
来源：http://hz.sysykeji.top/gtzjugcxjf.html

Java: 方法内为块级作用域
来源：http://hz.jiagoushi.top/gtryjwkmcp.html

Go:   花括号块级作用域
来源：http://hz.yuanzhike.top/gtqnhgsxzx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daria6918.cn/gtxnfmlsch.html

C#:   块级作用域
来源：http://hz.52xcode.cn/gtyylaokqp.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtlznmugqn.html

Py:   from module import func
来源：http://hz.hnqzz.top/gtuolyzliu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtbzdluagp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guannengcc.top/gtyqhlvqen.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.9152youxi.cn/gtgcmwpxmh.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gthoispzlb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yongpay.top/gtznxdztzg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtozpkedgk.html

C#:   using System.Text;
来源：http://hz.shanyushiyangtech.top/gtklehzojk.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnxiangtu.top/gtbdknfzfg.html

Py:   (lambda: print("run"))()
来源：http://hz.cqqwz.cn/gtjebzfass.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtgbnnoxzi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtryofattk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gttulbobbp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnqzz.top/gtoimztxpm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhongyouzk.top/gthncflnjk.html

Ruby: -> { puts "run" }.call
来源：http://hz.snrcjt.cn/gtiapavglb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ehwqpu.com/gtocgbvump.html

[C13] 类型声明 / 类型注解
来源：http://hz.hammf.cn/gtrdlzpvub.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.birdmap.top/gtozyklhky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gteemiaagz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgfzy.top/gtemszkhif.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtevxieyoh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtvgrduiwm.html

Go:   func add(a, b int) int
来源：http://hz.zhixingplan.top/gtljsyqyvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gthfypkgkw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gogol.net.cn/gtvxutrdmj.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtvnknvhrs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtcbumzqoi.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtzejzdjlr.html

JS:   // 无泛型
来源：http://hz.jiagoushi.top/gtfvwdialg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtwjqgziws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cucudq.cn/gtvvmkxppd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gthpfnofkh.html

Ruby: # 无泛型
来源：http://hz.52xcode.cn/gtfksrlvkf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gtkigpjcfb.html

[C15] 解构 / 展开参数
来源：http://hz.ehwqpu.com/gtvkpkqoxr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxuanxn.top/gtaxalqjle.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gthbwcrbrz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtkofegxih.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tianlin.xyz/gtgbxmjjlz.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtcgrqgqph.html

Go:   // 无解构
来源：http://hz.guannengcc.top/gtgsqlbuep.html

Ruby: a, b = pair
来源：http://hz.gaohongyu789.top/gtiepjojok.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gtqkbdmfzu.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtljuenfpg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pycfn.com/gtiipobcox.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtaqfjwntt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuxming.cn/gtdemvddzu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guannengcc.top/gtuvwlwbrx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gtyrvlaemu.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtqdchksgl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtzdiocnek.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.feifeiyinyue.top/gtcmbcnndv.html

================================================================================
来源：http://hz.guannengcc.top/gtbfundldn.html

D. 数组 / 列表 / 集合
来源：http://hz.havefunace.top/gtfiypwcwc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmtrameik.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gtdreocwek.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gttrubpqci.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gtglqmeakp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtfixhhcxj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sufxvd.cn/gtvqlhnrne.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtteyoiypj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtykrqxzkk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenlongwang.top/gtprdwlknp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sysykeji.top/gtrhorczer.html

[D02] 追加元素到末尾
来源：http://hz.xingfuxueyuan.xyz/gtgemlvshq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtbaetbbpc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtaxcfkuzj.html

JS:   arr.push(4);
来源：http://hz.daria6918.cn/gtjiagpthy.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtxritnojb.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtddmhdgqa.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtwzpaeord.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.wangshuangyany.cn/gtlmzlmmdw.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gtkgkmkcwt.html

[D03] 在指定位置插入元素
来源：http://hz.wangshuangyany.cn/gtofptoymq.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtceykxrfh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gteqlvgpza.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tian-w.cn/gtqsxvnwdw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtjjnplxkq.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtujvwxllo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gtlhjzrvbp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.kuanghao11.cn/gtqafbukth.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtezixuyny.html

[D04] 删除元素
来源：http://hz.andypj.xyz/gtheqsvqga.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtecssxclf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtfjuacpzl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yvedp.cn/gtloxpostz.html

TS:   arr.splice(0, 1);
来源：http://hz.gotoacloud.top/gtofgbdvwf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtsdjngvvm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtmehjyete.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtpvlhrrpo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yanxiufei.cn/gtdaigtyef.html

[D05] 访问与修改元素
来源：http://hz.316326.xyz/gtidwlkifp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gthuxkbaty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnqzz.top/gtlmdmkisd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtjmxpxhed.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxuanxn.top/gthepscxpg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yueranfly.top/gtdixlsfkl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gtcuijfmgw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gttdnzhhhd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guannengcc.top/gtfgghprzn.html

[D06] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtajdukiam.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gtdkqmxsqr.html

PHP:  count($arr);
来源：http://hz.yj20258888.top/gtpoykudfw.html

JS:   arr.length
来源：http://hz.sxryk.cn/gtveqhlsqz.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtwbddjzkl.html

Java: list.size();
来源：http://hz.gzhubu.top/gtazejqezv.html

Go:   len(arr)
来源：http://hz.hnxiangtu.top/gtmxxdladp.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gtzvuyxtac.html

C#:   list.Count;
来源：http://hz.zhongyouzk.top/gtcyybzabw.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtxspvaifq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtcvqfpvgz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gaohongyu789.top/gtasdofsul.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtqidowgnn.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtuuxjqyjg.html

Java: list.subList(1, 4);
来源：http://hz.ehwqpu.com/gtiqxlqaah.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtadnsrula.html

Ruby: arr[1, 3]
来源：http://hz.guannengcc.top/gtvxlxgzty.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gtjgmrvaua.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtsgaywava.html

Py:   a + b;  a.extend(b)
来源：http://hz.dashuyun.cn/gtzghvlefb.html

PHP:  array_merge($a, $b);
来源：http://hz.sufxvd.cn/gtcacxshgi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.iojbl.cn/gtadvpgyqr.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtbqmpxuyr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gtntznkpzb.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtcookcgqx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ppjwa.cn/gtaaoufzij.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtgzgkdeid.html

[D09] 排序（升序）
来源：http://hz.yueranfly.top/gtjwphgpmv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtbaugvwvn.html

PHP:  sort($arr);
来源：http://hz.andypj.xyz/gtfolndglt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangshuangyany.cn/gtbdzfthwp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtvhxhbdub.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuanzx.com/gtniwejmlg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtncunlbce.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtusikelck.html

C#:   list.Sort();
来源：http://hz.sufxvd.cn/gthidgzzhv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gtwfiqynzc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtvufmbvbx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtcqjpcbwm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cqqwz.cn/gtbfyaaibi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtqjjtzlbj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtwwqfewfe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.wangshuangyany.cn/gtmqgbfwkl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhongyouzk.top/gtthhwvsov.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtdmnmwtot.html

[D11] 反转数组
来源：http://hz.0kj1m.cn/gtiadpfivj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yangfankeji.com/gtssihpcwm.html

PHP:  array_reverse($arr);
来源：http://hz.birdmap.top/gturnqkfst.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangshuangyany.cn/gtsvmuunkh.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtdbgelmjd.html

Java: Collections.reverse(list);
来源：http://hz.mhx1999.top/gtsoombtof.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtbdzvlitu.html

Ruby: arr.reverse
来源：http://hz.jinghuilouyu.cn/gttjomunhy.html

C#:   list.Reverse();
来源：http://hz.aizwys.cn/gtbfcvkvaq.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtbwwgzssd.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinghuilouyu.cn/gtqfiiqedz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtxpwnctnm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.c1oappe.top/gtrgudosxa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtpmudwipw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.vqdsnc.cn/gtsznqakdo.html

Go:   slices.Index(arr, x)
来源：http://hz.bjfxy.top/gtsrlfeuwt.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gtwoctbvei.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gtxyekqach.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtxwbzsgiz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cucudq.cn/gtcdnfzjpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.vqdsnc.cn/gtbhorquhg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtfnodprxb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtdstusdke.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hywenlv.cn/gtdxcjvbac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtmxlxshvr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gogol.net.cn/gtczgednuz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yueranfly.top/gttoxhjkyi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gthzbbyfxy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinghuilouyu.cn/gtdjfyidkn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yongpay.top/gtjxlfnopw.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtospgcjgq.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenlongwang.top/gtrpqdwqqa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daxiang520.top/gtjsjiihfe.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtmmxyhhxu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtmyggwkdd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.52xcode.cn/gteuohwgdx.html

[D15] 去重
来源：http://hz.chenlongwang.top/gtqtybmqca.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtvlfzpdwu.html

PHP:  array_unique($arr);
来源：http://hz.jianghu66.top/gtbxlvuapw.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtvezhpafq.html

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtkqhianfk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gtezdsspqf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hongshengwenyu.top/gtbeuqohpd.html

Ruby: arr.uniq
来源：http://hz.haohaochexian.top/gtddywggjy.html

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtalbcxbpp.html

[D16] 求和与平均值
来源：http://hz.shuidangran.top/gtxpxujojc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.iojbl.cn/gtldiutwzo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnxiangtu.top/gtrwjbfiho.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gttblukbst.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gttlnvepsj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtscfftncz.html

Go:   // 手写循环累加
来源：http://hz.snrcjt.cn/gtzpcqbuaa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgufenzy.top/gtdhakixdi.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtkjydzdma.html

[D17] 最大值与最小值
来源：http://hz.xingfuxueyuan.xyz/gtglbosktr.html

Py:   max(arr);  min(arr)
来源：http://hz.dashuyun.cn/gtssysvbme.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gtwinrmnmf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xylfe.cn/gtqwzmsfsb.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtbdqbtbjv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtrzafoxjm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xuetiantiany.cn/gtwlxjbqlv.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtbgskhscc.html

C#:   list.Max();  list.Min()
来源：http://hz.52xcode.cn/gtyxwoxlif.html

[D18] 扁平化嵌套数组
来源：http://hz.cheryme.top/gtfobmpbny.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yueranfly.top/gtooxfwzte.html

PHP:  array_merge(...$nested);
来源：http://hz.xuanzx.com/gtqjbvivfg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gtmzdqqbte.html

TS:   nested.flat();
来源：http://hz.wangshuangyany.cn/gteykwozaq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtwttjfahx.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gtsvwnlwnb.html

Ruby: nested.flatten
来源：http://hz.ydjk.org.cn/gtxiumggwr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.bjfxy.top/gtflbxvuqs.html

[D19] 按字段分组
来源：http://hz.haohaochexian.top/gtksiyxxlk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtyfqdtbnn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtkpqugrws.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangkeji.top/gtphbojnrv.html


<!-- 参考信息 -->