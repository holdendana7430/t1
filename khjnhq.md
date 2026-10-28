代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtkgtelola.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgfzy.top/gtwajewroa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtzlbbdobm.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gttuwenjqk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtewmszqkr.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gthtxrtxhl.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtqioghcud.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gtvitzilml.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtuomqcrju.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtxqwnkoin.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hysaishi.cn/gtbbytilra.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.dianchejie.cn/gtjhfuvuxx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gotoacloud.top/gtlgmftqdj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ivvv.top/gtolbicbvs.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtdatjowiz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxuanxn.top/gtxqwfonbi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hfpthk.cn/gtaraglrnf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtwzlfjmtd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtkzqpignp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cucudq.cn/gtctsuuccz.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuanzx.com/gtnrkmvwkv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtdiinwxzb.html

C#:   f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtylgnxpxr.html

[C05] 返回多个值
来源：http://hz.feifeiyinyue.top/gtllypocre.html

Py:   return a, b
来源：http://hz.birdmap.top/gthousgsjy.html

PHP:  return [$a, $b];
来源：http://hz.cheryme.top/gthpiwvuhz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gteftnznca.html

TS:   return { a, b };
来源：http://hz.ybcxt.top/gtqggpyzpu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtwqbomkuq.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtnzlywqjq.html

Ruby: return a, b
来源：http://hz.zhaomingkeji.xyz/gtxcmxstku.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gtczqcpnry.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtjeghpjwz.html

Py:   square = lambda x: x * x
来源：http://hz.cqqwz.cn/gtgmtgvfsb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ydjk.org.cn/gtaajwuvxb.html

JS:   const square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtivkabegx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtdxujwxec.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtrtwvzmbz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.iojbl.cn/gtsuilgqbr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hfpthk.cn/gthrvhffen.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtdcjxviml.html

[C07] 把函数作为参数传入
来源：http://hz.yj202588.top/gtrbkikyhq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtmavlvzil.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sufxvd.cn/gtgacamfkh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yongpay.top/gtkadkwhup.html

TS:   arr.map(String)
来源：http://hz.zhoulong.xyz/gtcjpghtkp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangkeji.top/gtjdylgtrx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtufindkxa.html

Ruby: arr.map(&:upcase)
来源：http://hz.vqdsnc.cn/gtusiflbmw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sysykeji.top/gtgzlqyabs.html

[C08] 闭包
来源：http://hz.hammf.cn/gthxpxyjyd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fengsongda.top/gtljjphbjg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgfzy.top/gtyykhlyfh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtsygsjphx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtfhxnsduj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sweek.top/gtwfpfxjbv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinqigufen.top/gtrhmpebrb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtstrvaaay.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtulrgtajg.html

[C09] 递归
来源：http://hz.9152youxi.cn/gtuxbekfcw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtherdsizq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtqvsxoktl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtizmfxdfc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtkphycozz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sxryk.cn/gthepivcoy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gtupdfwrnr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtqgrnjpaz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sxryk.cn/gtnrydqrcj.html

[C10] 变量作用域
来源：http://hz.fengsongda.top/gtrigckfyv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.svipenyu.cn/gtbdtjmeop.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ehwqpu.com/gtfwnwuezp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtipgbcdhp.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtuizdwsun.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtkyjbmcpe.html

Go:   花括号块级作用域
来源：http://hz.bjfxy.top/gttazrmmhu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gogol.net.cn/gtpsmcfmfg.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtasawrduy.html

[C11] 模块导入与导出
来源：http://hz.sweek.top/gtorkhqnda.html

Py:   from module import func
来源：http://hz.ehwqpu.com/gtkmbocfig.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.birdmap.top/gtbhvoxamo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zdqjudy.top/gtpzpaxxko.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtastdcpyq.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtswxnmtbt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gtvstosctb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenjidiqi.icu/gtxzqcbdud.html

C#:   using System.Text;
来源：http://hz.hywenlv.cn/gtxfzrquak.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gttsrgriht.html

Py:   (lambda: print("run"))()
来源：http://hz.quarkkingdee.top/gtpfktcryz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnxiangtu.top/gtolifhudq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gthzzwhyhb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtufixhhsu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gtrpslasds.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gtvuhiigxk.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtnsoulpdk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtbafgvxtw.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangkeji.top/gtikknytdt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.birdmap.top/gtwuivgotr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtoqizthmz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtgetmeuni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtmlzeosos.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtdompfgbw.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangtech.top/gtsufwbjpp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aizwys.cn/gtwbzoshdu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hnqzz.top/gtcfuvqetf.html

[C14] 泛型函数
来源：http://hz.jinqigufen.top/gtjmysehtl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gotoacloud.top/gtbluiaxyq.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtzkzjjnpl.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gtmusenbjd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yongpay.top/gtfkamvfhc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gteqyhtzlk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ppjwa.cn/gtcogiamps.html

Ruby: # 无泛型
来源：http://hz.zhixingplan.top/gtahuywury.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gturmljvbw.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtgcwvohle.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtitfehklu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtsmwuzyba.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtsdrrjozu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.havefunace.top/gtrrmdoiee.html

Java: // 无解构
来源：http://hz.jqgufenzy.top/gtsxstkyok.html

Go:   // 无解构
来源：http://hz.jinghuilouyu.cn/gtnlnvpzoh.html

Ruby: a, b = pair
来源：http://hz.cheryme.top/gtqeapeplr.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtsbkubpwx.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtjypwclkg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xingfuxueyuan.xyz/gtvtlaosnf.html

PHP:  // 无重载
来源：http://hz.yuanzhike.top/gtirtetbqh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangshuangyany.cn/gtiufeceez.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gtyhnvzvpp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cdnleiting.top/gtmqzbartl.html

Go:   // 无重载：用不同函数名
来源：http://hz.zdqjudy.top/gtzqcmbiiz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj20258.top/gttuliytjy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.9152youxi.cn/gtmxzhmzkp.html

================================================================================
来源：http://hz.gotoacloud.top/gtphlrxwos.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtomdnhtvs.html

================================================================================
来源：http://hz.iojbl.cn/gtzsybohnl.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtpkaocmpy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangdashe.top/gtftmfjlwl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nwbrower.top/gtctvuankq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dianchejie.cn/gtnasdaniu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ydzc1.top/gtaxushgxu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgufenzy.top/gtfdljvmlx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtesvaokdo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtlzssfyms.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.smart0.xyz/gtfsgzxcus.html

[D02] 追加元素到末尾
来源：http://hz.zhongyouzk.top/gtllitpfkq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtfyiqzqsk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hammf.cn/gtrerxurom.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gtdmiaijjq.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtvtmdzsso.html

Java: list.add(4);
来源：http://hz.zdqjudy.top/gtkydzjmym.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigfzy.top/gtdbqoqznd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtxawzmzuq.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtpnnhqzlm.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtmcpatofn.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gtaavnmwnu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtxbylvkpr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtvhtuzjje.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.snrcjt.cn/gtdjwlneny.html

Java: list.add(0, 0);
来源：http://hz.yongpay.top/gtvdikrioj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtnnirzraf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gtwaarjjht.html

C#:   list.Insert(0, 0);
来源：http://hz.nwbrower.top/gtozahysmi.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtuwnsszze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nwbrower.top/gtnzdxxopg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.feifeiyinyue.top/gtzyzriccu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tanke756.top/gtxiroeorq.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtrrmupjlo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhoulong.xyz/gtmfbsruwc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gtxxpgqbkf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenjidiqi.icu/gtekwptris.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gtcsgilwzc.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangkeji.top/gtteoycyqa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtgdzjgbgy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtcmubyzkg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtkybevgoa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtarxevszx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtzfopsuqy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgfzy.top/gtxwavabcl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gtbgzsyeid.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hongshengwenyu.top/gtqknqhyrm.html

[D06] 数组长度
来源：http://hz.sufxvd.cn/gtsjgtdeln.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtbmdavywi.html

PHP:  count($arr);
来源：http://hz.yj202588.top/gtycpornwt.html

JS:   arr.length
来源：http://hz.hammf.cn/gtukaispgu.html

TS:   arr.length
来源：http://hz.yuxming.cn/gttqnwnqjr.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtwtwfckxw.html

Go:   len(arr)
来源：http://hz.jlsjyb.cn/gtkndcgtjn.html

Ruby: arr.length; arr.size
来源：http://hz.xylfe.cn/gtkqmgiosm.html

C#:   list.Count;
来源：http://hz.hfpthk.cn/gtkkmyycke.html

[D07] 切片 / 取子数组
来源：http://hz.snrcjt.cn/gtasgygxik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xylfe.cn/gtdqsekizw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gtgfgexkgz.html

JS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtkyszrdgk.html

TS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtuekyhvag.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gtjfqlnnzl.html

Go:   arr[1:4]
来源：http://hz.tian-w.cn/gtjkiggexj.html

Ruby: arr[1, 3]
来源：http://hz.guowangkeji.top/gtdjcfjpqz.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtgjjdhirr.html

[D08] 合并两个数组
来源：http://hz.jyoumei.cn/gtxyqrzuhn.html

Py:   a + b;  a.extend(b)
来源：http://hz.gogol.net.cn/gtsjaxkqed.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gtvjoqsyto.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtqzawfmdt.html

TS:   [...a, ...b];
来源：http://hz.tanke756.top/gtkfdumtsn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.mhx1999.top/gtlrwktavy.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangtech.top/gthfyeyymw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fengsongda.top/gtusscdebt.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gtdcthwuso.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtuylydqal.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtelyvhkhh.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtppptyxgl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtzbjzugci.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258.top/gtpxgansps.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.feifeiyinyue.top/gtchhjezke.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtfckjeknm.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtuibmdkqd.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtyeanfevz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangkeji.top/gtgkoylgdr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tian-w.cn/gtviswysut.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gtosjjzvbu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtslgodgyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gthqobwmpe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.52xcode.cn/gtqbzwjwwq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtxivspxqt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtiitqvgpw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ppjwa.cn/gtjmzhfzti.html

[D11] 反转数组
来源：http://hz.tanke756.top/gtvmkginfm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yuxming.cn/gttwtrjezu.html

PHP:  array_reverse($arr);
来源：http://hz.gotoacloud.top/gtbirbexqo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtdrpeaihr.html

TS:   [...arr].reverse();
来源：http://hz.tian-w.cn/gtululubav.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gthzsfmfgq.html

Go:   slices.Reverse(arr)
来源：http://hz.jinyuanbaomall.cn/gtczzzwscw.html

Ruby: arr.reverse
来源：http://hz.jqgfzy.top/gtzbbeoyhl.html

C#:   list.Reverse();
来源：http://hz.yonumen.top/gtsnlmizfq.html

[D12] 查找元素下标
来源：http://hz.yj20258888.top/gtrrnaemfo.html

Py:   arr.index(x);  x in arr
来源：http://hz.aizwys.cn/gtlknbijep.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.c1oappe.top/gtkonsjhzv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtzwjdyecg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtuslavowh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hfpthk.cn/gtjkpgbazz.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gtdsgtaiev.html

Ruby: arr.index(x)
来源：http://hz.hywenlv.cn/gtrhunvknl.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtvrzufwuc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtvemzcnnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hfpthk.cn/gtpekofmsa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtfgqmylqb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtlwovxhko.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtzfdmtvmq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gttepqanzh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258.top/gtktqshytu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zycfv.cn/gtntcravsd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.mhx1999.top/gtvolixxbs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtqxcvenvo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sxryk.cn/gtyuutfsoh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sxryk.cn/gtwcpdnsen.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtgmtbomrf.html

TS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gthjnrniqa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.316326.xyz/gtanfmguxo.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gthxnjgmii.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sweek.top/gtvhyohvju.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xylfe.cn/gtbwekcnsz.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtwcjgtinq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtevgcmjst.html

PHP:  array_unique($arr);
来源：http://hz.quarkkingdee.top/gtawtwxlif.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtzdoffepa.html

TS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtejzpxknw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangtech.top/gtmvmmpfpq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhiwuduotai.top/gtqmhyandu.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtyrzhnvbx.html

C#:   list.Distinct().ToList()
来源：http://hz.yueranfly.top/gtacypydjc.html

[D16] 求和与平均值
来源：http://hz.yj20258888.top/gttqzaaslw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtvfnwvvky.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sxryk.cn/gtpbwesape.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtburjweeg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtyluodzsq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtstilculv.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtmmktgufd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinghuilouyu.cn/gthnhcjigk.html

C#:   list.Sum();  list.Average()
来源：http://hz.aizwys.cn/gtkffxztdn.html

[D17] 最大值与最小值
来源：http://hz.gotoacloud.top/gtkkbsibqo.html

Py:   max(arr);  min(arr)
来源：http://hz.haohaochexian.top/gtafzndytb.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gtnxbkqjia.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtctuaoyhr.html

TS:   Math.max(...arr);
来源：http://hz.jqgufenzy.top/gtzogmtpwt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtwmlnkodf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.kuanghao11.cn/gtrkqhfxji.html

Ruby: arr.max;  arr.min
来源：http://hz.redwolf501.top/gtwzwqncgc.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtkprvqvbj.html

[D18] 扁平化嵌套数组
来源：http://hz.zhongyouzk.top/gtttqiaipw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yanxiufei.cn/gtethtopua.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtmxfttuno.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtfijzlrrm.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtwrroteqp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xuetiantiany.cn/gtwooohsqy.html

Go:   // 手写双层循环
来源：http://hz.jinqigufen.top/gtstjrqakf.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtlgmeifer.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhixingplan.top/gtuceuzmki.html

[D19] 按字段分组
来源：http://hz.pycfn.com/gtqdoifdrl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gtnedglgte.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtiwnldmrx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtyikniavt.html


<!-- 参考信息 -->