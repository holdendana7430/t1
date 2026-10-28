代发 wailian999

Py:   if not data: return
来源：http://hz.mhx1999.top/gtdijgmawc.html

PHP:  if (!$data) { return; }
来源：http://hz.aizwys.cn/gtfasmxoaa.html

JS:   if (!data) return;
来源：http://hz.birdmap.top/gthlxahlza.html

TS:   if (!data) return;
来源：http://hz.svipenyu.cn/gtfsiquzqd.html

Java: if (data == null) return;
来源：http://hz.xinyue.icu/gttxjieooz.html

Go:   if data == nil { return }
来源：http://hz.xziqi.cn/gtgsaqxntn.html

Ruby: return if data.nil?
来源：http://hz.c1oappe.top/gtsykcpyex.html

C#:   if (data == null) return;
来源：http://hz.0kj1m.cn/gtbuygejzb.html

================================================================================
来源：http://hz.sweek.top/gtmauvtpgo.html

C. 函数与作用域
来源：http://hz.hfpthk.cn/gtwwtwhcix.html

================================================================================
来源：http://hz.yuanzhike.top/gtrxvqixaw.html

[C01] 定义函数
来源：http://hz.316326.xyz/gttqdcnvux.html

Py:   def add(a, b): return a + b
来源：http://hz.jiagoushi.top/gtxgpxotvu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtbpsvvqxu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yueranfly.top/gtmtuxwjjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtxobdqwcu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtpxkfeyrs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258.top/gtqbssjoni.html

Ruby: def add(a, b); a + b; end
来源：http://hz.dashuyun.cn/gthqhookmd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtvfsawztt.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtybbiwpst.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtcjzgqdra.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenzaomai.com/gtpxxdgtxn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gtzmqanofg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.316326.xyz/gtksghmpzo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtxmzqywyk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jianghu66.top/gtmeeaqsdf.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangshuangyany.cn/gtalfkiqek.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigufen.top/gtekybntfm.html

[C03] 可变参数
来源：http://hz.jlsjyb.cn/gtheebqiau.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtpouddujj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtbwescamn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtdxytmfyl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtruxjhilk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gogol.net.cn/gtibdnlfoe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yongpay.top/gtksounmer.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangshuangyany.cn/gttsqlrxox.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zdqjudy.top/gtygucmwmd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pengpengdd.cyou/gtaccvwiov.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtquhgnhfu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gthsyqjhtg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtexicbktd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtzmpkkmzo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ppjwa.cn/gtjlwisgqd.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtklomucar.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtzdqzzkuc.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtonlmoqhg.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtbbbiyica.html

Py:   return a, b
来源：http://hz.yuanzhike.top/gtoeyfnrmi.html

PHP:  return [$a, $b];
来源：http://hz.jinqigfzy.top/gtfjacymak.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nwbrower.top/gtkandvels.html

TS:   return { a, b };
来源：http://hz.9152youxi.cn/gtrqwjartv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shzxlz.cn/gtszcqxgov.html

Go:   return a, b
来源：http://hz.sufxvd.cn/gtdhcjkkms.html

Ruby: return a, b
来源：http://hz.zhaomingkeji.xyz/gtxbqjyofc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtssloerwj.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtnbjikvxh.html

Py:   square = lambda x: x * x
来源：http://hz.feifeiyinyue.top/gtsnkksudt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gtfkjzfjfw.html

JS:   const square = x => x * x;
来源：http://hz.hywenlv.cn/gthtugcpim.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.snrcjt.cn/gtwfdkopbm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gtahfvcqsv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigufen.top/gttfvkvnad.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhongyouzk.top/gtebjwgqgq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258888.top/gtuldgmorx.html

[C07] 把函数作为参数传入
来源：http://hz.fengsongda.top/gthclymrts.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cucudq.cn/gtchpxcfhz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtvriektko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangshuangyany.cn/gtpbdshiic.html

TS:   arr.map(String)
来源：http://hz.xylfe.cn/gtrrbxfogm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangkeji.top/gtndrgplug.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xinyue.icu/gtsaernlhu.html

Ruby: arr.map(&:upcase)
来源：http://hz.snrcjt.cn/gtputbhivi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.meibo888.top/gtxxbpkbqk.html

[C08] 闭包
来源：http://hz.zycfv.cn/gtpuctpfze.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhiwuduotai.top/gtkdtjrnjm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinyuanbaomall.cn/gtvjcyjrbd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtxrtdjsnv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtbqrzpolc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtbysnnpbp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cashguo.top/gtzclhmxzp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.0kj1m.cn/gtzbmdxwct.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtplwqlahb.html

[C09] 递归
来源：http://hz.shuidangran.top/gtmlccregi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gtjjsjgstn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.haohaochexian.top/gtgvndlavy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtruncvbzo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtrjpibsam.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tanke756.top/gttuksdctd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jianghu66.top/gtxkkykvoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hfpthk.cn/gtyrtxwazs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.52xcode.cn/gtyzttxvdi.html

[C10] 变量作用域
来源：http://hz.ehwqpu.com/gtaurstwme.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guowangkeji.top/gtmbrhbmtg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yvedp.cn/gtpenhmktf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jlsjyb.cn/gtocttbjnd.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtwceyridn.html

Java: 方法内为块级作用域
来源：http://hz.jqgfzy.top/gtfeihuqax.html

Go:   花括号块级作用域
来源：http://hz.hfpthk.cn/gtnysupbtl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydzc1.top/gtbujqsbgq.html

C#:   块级作用域
来源：http://hz.nanxuanxn.top/gtrslhqwuc.html

[C11] 模块导入与导出
来源：http://hz.cucudq.cn/gtfjpzefpy.html

Py:   from module import func
来源：http://hz.fengsongda.top/gtpedeaogn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yanxiufei.cn/gttftizyyb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.havefunace.top/gtiwgjjfhr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtwxymmszz.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtjxilnral.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yongpay.top/gtbafssxrs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258888.top/gttkikmtpl.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gteodccctz.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtukuakxsb.html

Py:   (lambda: print("run"))()
来源：http://hz.hnxiangtu.top/gtxoxntmed.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258888.top/gtsrkzzpod.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtdzrnxyvk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtylalrxoe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.andypj.xyz/gtiueqzfuc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtdquzhjew.html

Ruby: -> { puts "run" }.call
来源：http://hz.tanke756.top/gtehqurnpe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtjdvkxsfw.html

[C13] 类型声明 / 类型注解
来源：http://hz.c1oappe.top/gtskiupflc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtznbrpywz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtqrpiiqhc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangdashe.top/gtjrlycyit.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtpfnutalb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtbnddrmnw.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtltmfvehu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtwvikrafj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtqiwdkevw.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gtzqhnqywx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ehwqpu.com/gtrxmlhxdv.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtnvzjvxvu.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtxehxyglq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtvxdtiqkp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ivvv.top/gtcqprtwmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jyoumei.cn/gtqolcvuht.html

Ruby: # 无泛型
来源：http://hz.yueranfly.top/gtidelrafm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.havefunace.top/gtxjhswtxn.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtckabwxyn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxinkj.top/gtxrxbijrm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydjk.org.cn/gtpxekytme.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtghuvelvx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtyhyvhilh.html

Java: // 无解构
来源：http://hz.zycfv.cn/gtfdgqlpvt.html

Go:   // 无解构
来源：http://hz.andypj.xyz/gtfncmoere.html

Ruby: a, b = pair
来源：http://hz.jyoumei.cn/gtnlmopuum.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gthnnakmpb.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtpfyycwtv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gttiptzpak.html

PHP:  // 无重载
来源：http://hz.ppjwa.cn/gtaktyunlh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sysykeji.top/gtaqcpgpsg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gteesmnwas.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.iojbl.cn/gtrszysubc.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtafhklyqt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daxiang520.top/gttcoqewyn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtexemnfpt.html

================================================================================
来源：http://hz.ydjk.org.cn/gtavwjizng.html

D. 数组 / 列表 / 集合
来源：http://hz.zhiwuduotai.top/gtcvxetklv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlkpvyuyp.html

[D01] 创建数组 / 列表
来源：http://hz.xziqi.cn/gtdeccjyjg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtaewljfqp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.haohaochexian.top/gtzzgyhtzi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cdnleiting.top/gtzyaxljcq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gtdjnqrteq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtsmifahjp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtknroxsny.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ehwqpu.com/gteocmlldz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtsylhynnh.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtqaginnjo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shzxlz.cn/gthigxoqou.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhixingplan.top/gtiovtrvto.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtomavbxjw.html

TS:   arr.push(4);
来源：http://hz.mhx1999.top/gtdetntxml.html

Java: list.add(4);
来源：http://hz.dashuyun.cn/gtxgohgbyg.html

Go:   arr = append(arr, 4)
来源：http://hz.shzxlz.cn/gtzmaahrrh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtkvgjaemd.html

C#:   list.Add(4);
来源：http://hz.xinyue.icu/gtqbyyjfgr.html

[D03] 在指定位置插入元素
来源：http://hz.iojbl.cn/gtlhzxvwoo.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtkzxpifps.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtdnokcxdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hfpthk.cn/gtggbzxomp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtsfevvrfm.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtgtfmxaqg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yvedp.cn/gtnrkhcewk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnqzz.top/gtfnnfumhv.html

C#:   list.Insert(0, 0);
来源：http://hz.yueranfly.top/gtngvjduae.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtuzlopaiv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtqkaqbtpe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtytzdwkvc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtwepaojug.html

TS:   arr.splice(0, 1);
来源：http://hz.cqqwz.cn/gtcfnwvjgn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtflmzddgf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtmfkmckaw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtdwduonwo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtrhuzpxew.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtisbszruw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ivvv.top/gtioomzavu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtacogljqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtbujkwqgp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtzevjcvsi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxuanxn.top/gtuzboobgc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yonumen.top/gtutiknhay.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtwkvpfbfe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yongpay.top/gtlaksjyvq.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtpzpiafxc.html

Py:   len(arr)
来源：http://hz.ppjwa.cn/gtfwlwnkpz.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtdjyafkdx.html

JS:   arr.length
来源：http://hz.jqgufenzy.top/gtqcrnrxai.html

TS:   arr.length
来源：http://hz.dianchejie.cn/gtnmktowpa.html

Java: list.size();
来源：http://hz.xylfe.cn/gtcbqrbuba.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtvaqvqusu.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtczydgpkw.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gtkpwdrwiy.html

[D07] 切片 / 取子数组
来源：http://hz.ehwqpu.com/gtjayaxqml.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydzc1.top/gtkwenntgm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangkeji.top/gtoesqpnli.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtcnvizbys.html

TS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtxsyksidt.html

Java: list.subList(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtvpdcavjv.html

Go:   arr[1:4]
来源：http://hz.snrcjt.cn/gtwcxvhkuy.html

Ruby: arr[1, 3]
来源：http://hz.ydzc1.top/gtubajkqov.html

C#:   list.GetRange(1, 3);
来源：http://hz.cucudq.cn/gtgxkpqbqr.html

[D08] 合并两个数组
来源：http://hz.yonumen.top/gtkfqhvgbt.html

Py:   a + b;  a.extend(b)
来源：http://hz.nwbrower.top/gtwjpulaoa.html

PHP:  array_merge($a, $b);
来源：http://hz.meibo888.top/gtiahjcbfk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtfmuravim.html

TS:   [...a, ...b];
来源：http://hz.haohaochexian.top/gtzgwcrmjy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtyimhjxzt.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtbtdrzknh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gthhdkhjag.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhixingplan.top/gtjadqnzmi.html

[D09] 排序（升序）
来源：http://hz.daxiang520.top/gtzuiurlfs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtnifpfpkl.html

PHP:  sort($arr);
来源：http://hz.iojbl.cn/gtkevwgkjj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ppjwa.cn/gtxifsiuty.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtvynsjfuw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhixingplan.top/gtdbkkigtn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yonumen.top/gtqajbzuui.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtelxyvjcw.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gthfhkuond.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tianlin.xyz/gtrflswokb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cucudq.cn/gtknjzwlwc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtlymapgcl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtzapcpnqc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtarrorses.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.bjfxy.top/gtfppiddaj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tianlin.xyz/gtaocefkra.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nwbrower.top/gttfqbzpty.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtxrzayest.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtiwvuxsgh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtoxbqpwij.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtixwaerqu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gtvynmdxyb.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtbgwrwspv.html

Java: Collections.reverse(list);
来源：http://hz.feifeiyinyue.top/gtsdfwhcvo.html

Go:   slices.Reverse(arr)
来源：http://hz.iojbl.cn/gtzycrhsyo.html

Ruby: arr.reverse
来源：http://hz.shzxlz.cn/gtetxyshyz.html

C#:   list.Reverse();
来源：http://hz.zdqjudy.top/gtgjjufkyv.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtcnxkexyh.html

Py:   arr.index(x);  x in arr
来源：http://hz.shuidangran.top/gtdvqnekya.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj20258888.top/gtwmwtqdld.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtwmbvrwxx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gttjsxmuxu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtkwobwpmw.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gtczzmxzyb.html

Ruby: arr.index(x)
来源：http://hz.yj202588.top/gtqgltkngp.html

C#:   list.IndexOf(x);
来源：http://hz.xylfe.cn/gtlzbwyrzk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gtgqylrpzh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtyjaniaae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtnhhdmpyu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gtguchxuvv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtyuwraeob.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gtkhfgznhn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtlihvbkji.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhaomingkeji.xyz/gtqsouftbj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtxnioudxo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gttugkkoak.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gteyaplmxy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gttotbfvin.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gttkzmtbop.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtsgvwdufg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigfzy.top/gtgpswsrru.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gttibqvlfu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuanzx.com/gtvnzhuuen.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nwbrower.top/gtzanyvajr.html

[D15] 去重
来源：http://hz.c1oappe.top/gtoxifwkly.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtucvhvxzn.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtappstkcp.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtlzcjppbj.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtdduzouzg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cdnleiting.top/gtijlvfnha.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtdkbjgaxt.html

Ruby: arr.uniq
来源：http://hz.dashuyun.cn/gtdiebeaal.html

C#:   list.Distinct().ToList()
来源：http://hz.yongpay.top/gtxlqaealu.html

[D16] 求和与平均值
来源：http://hz.meibo888.top/gtqhnpbvdr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnqzz.top/gtjtkinjcj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jianghu66.top/gtqmvnneav.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtyxdgzrqt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtrwnxbsjn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shangyingyoupin.top/gtsozmujxg.html

Go:   // 手写循环累加
来源：http://hz.chenzaomai.com/gtxldjplvx.html


<!-- 参考信息 -->