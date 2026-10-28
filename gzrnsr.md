代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtabertvzv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtivxqydxl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtdiupjvtv.html

Ruby: def greet(name = "World") = name
来源：http://hz.yonumen.top/gtpylykiea.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigfzy.top/gteyccjkay.html

[C03] 可变参数
来源：http://hz.shuidangran.top/gtpezlqgkx.html

Py:   def total(*args): return sum(args)
来源：http://hz.ehwqpu.com/gtrfhpnuvi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jqgfzy.top/gtcmsjrivb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtjmopobuq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtrfsdsfea.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yongpay.top/gtuqokwzdz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigufen.top/gtcxptixyy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgfzy.top/gttaakqzom.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guowangkeji.top/gtgbwmxchi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtiaszxxfk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.0kj1m.cn/gtfthpbiwz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtdghngxtq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhoulong.xyz/gtjmlyltyk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangdashe.top/gtnaabzann.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gteshqylaq.html

Go:   // 无：用配置结构体参数
来源：http://hz.daria6918.cn/gtfzpaolms.html

Ruby: f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtlhsftvpz.html

C#:   f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtuwdivgev.html

[C05] 返回多个值
来源：http://hz.mhx1999.top/gtjbggfsdt.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtyxeeeokd.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtbzvjbcns.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.havefunace.top/gtibdglppo.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtfogocnxt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gtjtgxyvmg.html

Go:   return a, b
来源：http://hz.daria6918.cn/gtyskmdwvo.html

Ruby: return a, b
来源：http://hz.zdqjudy.top/gtkwlhlwit.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtoyegyzrd.html

[C06] 匿名函数 / lambda
来源：http://hz.sweek.top/gtdkophrzj.html

Py:   square = lambda x: x * x
来源：http://hz.hnqzz.top/gtcuswieko.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.mhx1999.top/gtzxwewlpp.html

JS:   const square = x => x * x;
来源：http://hz.hfpthk.cn/gtoccvucxn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtxtgmoqmz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtrrgzlfuy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhengqikj.top/gtginobayb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtqogssgbl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ybcxt.top/gtodnczmjp.html

[C07] 把函数作为参数传入
来源：http://hz.zdqjudy.top/gtdiujbaff.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daria6918.cn/gtbeptwubf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangkeji.top/gthcuziwsy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jlsjyb.cn/gtpcbwrehh.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtntbuyreb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.quarkkingdee.top/gtbppirdys.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nwbrower.top/gtlegeyaah.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydzc1.top/gttryoenyq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hongshengwenyu.top/gtjopigpjl.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtavimqztd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtvwbqqsnr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258.top/gtqjvvyveh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtuerwfrna.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gthwzamftj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.haohaochexian.top/gtqvpdxaue.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tanke756.top/gtdguwrimf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sysykeji.top/gtyhqecwdk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtwtegkfva.html

[C09] 递归
来源：http://hz.cashguo.top/gtwbwlhzbv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gtkorsbusg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cucudq.cn/gtkkouoiiw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtzjblzeee.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtocnmmllx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gteezgnkbu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jianghu66.top/gtlomzlgud.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtmwnclrju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtaerminut.html

[C10] 变量作用域
来源：http://hz.gzhubu.top/gtnzdkpsvn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxinkj.top/gtduxpknio.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xylfe.cn/gtkcigubnt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gzhubu.top/gtipkdjpmi.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtwgtmpqpk.html

Java: 方法内为块级作用域
来源：http://hz.yvedp.cn/gtufxqfnua.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtdkyxszou.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gtfzzivsyd.html

C#:   块级作用域
来源：http://hz.dashuyun.cn/gtlywdltzm.html

[C11] 模块导入与导出
来源：http://hz.andypj.xyz/gtobcmjrot.html

Py:   from module import func
来源：http://hz.zhoulong.xyz/gtqwddwmkn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aibaodan.cn/gttzukntxq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gthwxwjiqw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhoulong.xyz/gtusdlzohz.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtrdyyfhzd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.andypj.xyz/gtpbizysac.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hammf.cn/gtxdnanqwd.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gtvvdkjbxy.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtzuvpjneh.html

Py:   (lambda: print("run"))()
来源：http://hz.hammf.cn/gtkdfymgip.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangshuangyany.cn/gtptdfoutu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gthzplkcjv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtuzaptgsl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigufen.top/gtkfrtieej.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuetiantiany.cn/gtsiipghyc.html

Ruby: -> { puts "run" }.call
来源：http://hz.cashguo.top/gtwnenmmex.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.vqdsnc.cn/gtlwidvphq.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtcyhjmsxc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.quarkkingdee.top/gtoopywbor.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtvadgvyqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.birdmap.top/gtlrsvrqoo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtywirxsxg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtphydmnzh.html

Go:   func add(a, b int) int
来源：http://hz.daria6918.cn/gtyudsaclt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gthylncicy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hnqzz.top/gtigznluln.html

[C14] 泛型函数
来源：http://hz.zhijiandao.cn/gtbjkugoum.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pengpengdd.cyou/gteasrmrue.html

PHP:  // 无泛型
来源：http://hz.hfpthk.cn/gtrtktkbly.html

JS:   // 无泛型
来源：http://hz.guannengcc.top/gtselfpajp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gtxiqyxeod.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtivijoaqu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangtech.top/gtnklaggdy.html

Ruby: # 无泛型
来源：http://hz.hnxiangtu.top/gtqziewdpo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yanxiufei.cn/gtzrplmrdz.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtihbfoutz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtqnrfxdqg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtguhejkqk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gttoycdnsj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtekjkugzw.html

Java: // 无解构
来源：http://hz.yonumen.top/gtfsarihnk.html

Go:   // 无解构
来源：http://hz.pycfn.com/gtujzwzrbe.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gtswydghei.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtgrnuvivs.html

[C16] 函数 / 方法重载
来源：http://hz.zhiwuduotai.top/gtfrgjkdvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yangfankeji.com/gttqojzanc.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtaxryonpz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj20258888.top/gtfkcfnazo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sysykeji.top/gtmesuywjg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aibaodan.cn/gtdvjcksng.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtbrgsedok.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtnwrzkisb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtjaufbpxa.html

================================================================================
来源：http://hz.daxiang520.top/gtlultlwgn.html

D. 数组 / 列表 / 集合
来源：http://hz.ybcxt.top/gtcqlrhygc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrtjvahlv.html

[D01] 创建数组 / 列表
来源：http://hz.c1oappe.top/gtbrjhctwx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.0kj1m.cn/gtfvrqdzis.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtukrrifqn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ybcxt.top/gtqvnnblkg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtrwypduen.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtywjxomgy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtqcdjwzub.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtsoyjfzod.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ppjwa.cn/gtezkynsjs.html

[D02] 追加元素到末尾
来源：http://hz.hywenlv.cn/gtiufbmcve.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinghuilouyu.cn/gtzvzjwudl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dashuyun.cn/gttsxzylgf.html

JS:   arr.push(4);
来源：http://hz.guowangkeji.top/gtvzlhzugt.html

TS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtckcaeple.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtuyauntbq.html

Go:   arr = append(arr, 4)
来源：http://hz.yangfankeji.com/gtexncogxq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ehwqpu.com/gtwluovepl.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gttxmmubqd.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtvkakigka.html

Py:   arr.insert(0, 0)
来源：http://hz.zhixingplan.top/gtttmkaizo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtufrigljq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cashguo.top/gtzarffdvs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cqqwz.cn/gtwkvbrlvi.html

Java: list.add(0, 0);
来源：http://hz.cucudq.cn/gtszauktpt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gthlkxfogu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hywenlv.cn/gtjuhgiufa.html

C#:   list.Insert(0, 0);
来源：http://hz.gogol.net.cn/gtwvcuimpb.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gttmvpbfyy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daria6918.cn/gtmwgmkfaq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtfzvuvwpq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gtdmuhikad.html

TS:   arr.splice(0, 1);
来源：http://hz.yvedp.cn/gtwuahclcg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtyyfagjlg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shuidangran.top/gtfrevcryn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gtnujdkwdt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yongpay.top/gtkdgpouks.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtjfleaolt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtnqgnbfdg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtznqudaro.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hywenlv.cn/gtjhqsvugu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dashuyun.cn/gtbasyvrqm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gteieyowsp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtwubwzwpp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtunlapnji.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gthjrcotpx.html

[D06] 数组长度
来源：http://hz.sweek.top/gtsrdpdgvo.html

Py:   len(arr)
来源：http://hz.feifeiyinyue.top/gtlxgwmkci.html

PHP:  count($arr);
来源：http://hz.jinghuilouyu.cn/gtiozdpkvr.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtaxsvwjja.html

TS:   arr.length
来源：http://hz.ydzc1.top/gtsfdzobpd.html

Java: list.size();
来源：http://hz.tian-w.cn/gtzqtoqepm.html

Go:   len(arr)
来源：http://hz.gogol.net.cn/gthittenrw.html

Ruby: arr.length; arr.size
来源：http://hz.ehwqpu.com/gttzyzomai.html

C#:   list.Count;
来源：http://hz.andypj.xyz/gtnbmkbzmx.html

[D07] 切片 / 取子数组
来源：http://hz.9152youxi.cn/gtdwzgzuon.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxinkj.top/gtelroeggg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtyvmvrshr.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtvefxmvhe.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gttzmhrtce.html

Java: list.subList(1, 4);
来源：http://hz.tian-w.cn/gtgoqkvtwj.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gtyefdinpd.html

Ruby: arr[1, 3]
来源：http://hz.guannengcc.top/gtloyuzusl.html

C#:   list.GetRange(1, 3);
来源：http://hz.mhx1999.top/gtpgcvzaty.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtsgcyngau.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtmmybxeih.html

PHP:  array_merge($a, $b);
来源：http://hz.chenzaomai.com/gtvknbgtjj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtgjlsegow.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtqtltmpjz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhiwuduotai.top/gtytsindri.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtgrkihrle.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aizwys.cn/gtuufhdwjc.html

C#:   a.Concat(b).ToList()
来源：http://hz.ehwqpu.com/gtvipeycdp.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gthydcmtum.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtvwvjejmi.html

PHP:  sort($arr);
来源：http://hz.ybcxt.top/gtcesvnhry.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jlsjyb.cn/gtnzokgzhu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xziqi.cn/gtczosuqci.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tian-w.cn/gthlnemrdw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtescrfele.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtimnplfcg.html

C#:   list.Sort();
来源：http://hz.yvedp.cn/gtkjodrqgz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangdashe.top/gtjmflxtip.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shangyingyoupin.top/gtqgjsqfdr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtqddbicid.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtwozrjokk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtojhxxghx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gteqsrqizm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jiagoushi.top/gtcbpwzphp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jyoumei.cn/gtmpwxunpg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuetiantiany.cn/gtqbhhlehf.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtyorqbsfk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gteuolutuw.html

PHP:  array_reverse($arr);
来源：http://hz.cdnleiting.top/gtwsuijbpc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aibaodan.cn/gtaxqhpmzd.html

TS:   [...arr].reverse();
来源：http://hz.pengpengdd.cyou/gtrldribhd.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtisgaexwe.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtbzjeocus.html

Ruby: arr.reverse
来源：http://hz.andypj.xyz/gtloodaajw.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtthgwhlhe.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangkeji.top/gtdrkzzwyj.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gtuzzbcbck.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hywenlv.cn/gtfqplafig.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gteofpojgq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtxjwrhhcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.andypj.xyz/gtvpcexejy.html

Go:   slices.Index(arr, x)
来源：http://hz.fengsongda.top/gtilymrloe.html

Ruby: arr.index(x)
来源：http://hz.dashuyun.cn/gtuzsnaoam.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gtpkotyyon.html

[D13] 过滤（保留满足条件的）
来源：http://hz.mhx1999.top/gtiuireszg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgufenzy.top/gtongvorsp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtjhxnzhdm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtrucgedwl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtfqklotqz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cqqwz.cn/gtsnhcvqdh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zycfv.cn/gtmounddgy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtnwruejbu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sysykeji.top/gteuvselrk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pengpengdd.cyou/gtvbtieyhy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hongshengwenyu.top/gtnfxftrsm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jiagoushi.top/gttvqsdatj.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gteojhggoq.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtnbfdhcks.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydjk.org.cn/gtxtvtsvpy.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtivosuznu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ehwqpu.com/gtvylehwkc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtgvdzfcpf.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtxhmbzyvv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtvztiqxor.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtxcpkdnbw.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtfsxybgbm.html

TS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gteqzgvppv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtiaigopba.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xziqi.cn/gtoqtgaeef.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gtuklzthvt.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtbcydfqvh.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtxakrjjpx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtkwtfrdvn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinqigufen.top/gtuqcgyejq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtkwpaigaf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtfpepiuwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cdnleiting.top/gtdbtoteyp.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtkusrwxrv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.haohaochexian.top/gtivgmhyvs.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtntnqemgp.html

[D17] 最大值与最小值
来源：http://hz.ydzc1.top/gttskpawff.html

Py:   max(arr);  min(arr)
来源：http://hz.ehwqpu.com/gttcwczvam.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gtrrrrmixn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtsvrqgrcn.html

TS:   Math.max(...arr);
来源：http://hz.ydzc1.top/gtbsltlfrk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtzfdxpdcc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gtmagujnsn.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtiopjzwio.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtjdkoblou.html

[D18] 扁平化嵌套数组
来源：http://hz.xuetiantiany.cn/gtydrkxdgg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guowangkeji.top/gtoaauqfof.html

PHP:  array_merge(...$nested);
来源：http://hz.xingfuxueyuan.xyz/gtpbvdrmwa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shangyingyoupin.top/gtcndgolpq.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtuxvwsbsb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtuuremcas.html

Go:   // 手写双层循环
来源：http://hz.svipenyu.cn/gtsipojakc.html

Ruby: nested.flatten
来源：http://hz.jinghuilouyu.cn/gtxgpupuqr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jqgufenzy.top/gtxeggmnzs.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gtnytkpxlu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gtwzrvdtuz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.havefunace.top/gtogzfzffv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.birdmap.top/gttncdyuxf.html


<!-- 参考信息 -->