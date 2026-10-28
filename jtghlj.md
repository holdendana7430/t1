代发 wailian999

[C02] 默认参数
来源：http://hz.shanyushiyangkeji.top/gtefzskjuf.html

Py:   def greet(name="World"): return name
来源：http://hz.svipenyu.cn/gtnipxzbey.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sufxvd.cn/gtuzennggg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtybgpqakm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gtzrqlhnlk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shuidangran.top/gtrbfwidle.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fengsongda.top/gtrtkjbrqc.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuanzx.com/gttkdlcsik.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cashguo.top/gtjliunmyt.html

[C03] 可变参数
来源：http://hz.52xcode.cn/gtaxsohcjg.html

Py:   def total(*args): return sum(args)
来源：http://hz.vqdsnc.cn/gtpokemhlr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gaohongyu789.top/gtqdeucgqr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gtmhdepxtf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtvwymujag.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yonumen.top/gtqozxjxaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yvedp.cn/gtoorznqse.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cashguo.top/gtrrposecr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.birdmap.top/gtravlwlah.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnxiangtu.top/gtjfoqhmqb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnxiangtu.top/gtpjbfyaed.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nanxuanxn.top/gtdpeopwxv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtxcuposrz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtlpczxwan.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xylfe.cn/gtzrntcduz.html

Go:   // 无：用配置结构体参数
来源：http://hz.316326.xyz/gtadgwudsw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtfemeoxie.html

C#:   f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtuxzjkhhz.html

[C05] 返回多个值
来源：http://hz.cqqwz.cn/gtzhplzpcl.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtgzhperie.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtcnvarnnr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.9152youxi.cn/gtpmxdqjir.html

TS:   return { a, b };
来源：http://hz.9152youxi.cn/gtedvxhbgy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hywenlv.cn/gtiplzxnmn.html

Go:   return a, b
来源：http://hz.yj20258.top/gttlhbntao.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtxgtxncuc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigfzy.top/gtspjvwxsf.html

[C06] 匿名函数 / lambda
来源：http://hz.gogol.net.cn/gtkvrzuuae.html

Py:   square = lambda x: x * x
来源：http://hz.wangshuangyany.cn/gtnntnkjkk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.aizwys.cn/gtmogfpcbs.html

JS:   const square = x => x * x;
来源：http://hz.hfpthk.cn/gtzrliqxch.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gzhubu.top/gtyzdvbdew.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tianlin.xyz/gtrhqfrbah.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aibaodan.cn/gtviydjjno.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hysaishi.cn/gtqjrzovnm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jianghu66.top/gtjxfgcsla.html

[C07] 把函数作为参数传入
来源：http://hz.zdqjudy.top/gttxfpcfyo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yonumen.top/gtfisacycu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hysaishi.cn/gtiaekmxtt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtcdkmoxfa.html

TS:   arr.map(String)
来源：http://hz.bjfxy.top/gtspbxgkra.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xylfe.cn/gtcxgdpkzd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuanzhike.top/gtbdamnwzt.html

Ruby: arr.map(&:upcase)
来源：http://hz.xylfe.cn/gtnjgepgmj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhijiandao.cn/gthqjdrogh.html

[C08] 闭包
来源：http://hz.xziqi.cn/gtsfyicudw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aibaodan.cn/gtdoeoyugg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dashuyun.cn/gtnbqhxaqe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtyrezqpmn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtepykvrpz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.svipenyu.cn/gtbkxgxamg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gtdccaxhzl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.vqdsnc.cn/gtvwoooswb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtyzmqifbs.html

[C09] 递归
来源：http://hz.shzxlz.cn/gtjbzglxvl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtiqiugxil.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tanke756.top/gtjervrfsw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtlievadgj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtuwouduxb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yueranfly.top/gtuovsooyb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gaohongyu789.top/gtquqgomqs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtwnzaeytu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtxjqrnisa.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gtavukhrki.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.meibo888.top/gtpyxrigzr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtjmioeref.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydzc1.top/gtsplfznql.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gtcvthotlp.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtmlauawvy.html

Go:   花括号块级作用域
来源：http://hz.jinyuanbaomall.cn/gtyugabkxu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtdfuegaxj.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtswcdmfwj.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtaijcwtoz.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtsfijczlq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.daxiang520.top/gtgjtuhtqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gogol.net.cn/gtelynetqv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.quarkkingdee.top/gtjcsnqnqf.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtxfgfiziz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtfqioixek.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtyoxyhvzp.html

C#:   using System.Text;
来源：http://hz.dianchejie.cn/gtgdvdsune.html

[C12] 立即执行函数 IIFE
来源：http://hz.sweek.top/gtsmyvlgyd.html

Py:   (lambda: print("run"))()
来源：http://hz.gogol.net.cn/gtpqglomht.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hysaishi.cn/gtnahggyhm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtuodcofnx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenzaomai.com/gtmtirdbzl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnxiangtu.top/gtvdrhykat.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinghuilouyu.cn/gtngehfptl.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtxekinyxu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtwtzlgsog.html

[C13] 类型声明 / 类型注解
来源：http://hz.ehwqpu.com/gtvgxhhikl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gtmfhpmiib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtpbeozmhw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenzaomai.com/gtbpgmgvaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtvzxhifwr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtmenwexns.html

Go:   func add(a, b int) int
来源：http://hz.yj202588.top/gtyvxqruvv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jyoumei.cn/gtmnvhswea.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtsdywgwcz.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtonnnfaju.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gtsclllcso.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtuenhmapb.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gttylqhtvx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ppjwa.cn/gtiegmzfmq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtwabaxams.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cashguo.top/gtncbdozjt.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtuoodsedz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.havefunace.top/gtrladzwox.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtwzlkdydm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtbxsaispj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinyuanbaomall.cn/gtoeqkgpyh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtxrgmzoph.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuetiantiany.cn/gttjsirpyr.html

Java: // 无解构
来源：http://hz.zhengqikj.top/gtbefcpdef.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtlejmwnvm.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtkmuekymc.html

C#:   var (a, b) = pair;
来源：http://hz.guannengcc.top/gteqkjefcf.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gthwqbkzov.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aibaodan.cn/gtxemcbagb.html

PHP:  // 无重载
来源：http://hz.zhiwuduotai.top/gtejezrnwx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guowangkeji.top/gtkvntlngr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nwbrower.top/gtklmvxlla.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhongyouzk.top/gtdlispevr.html

Go:   // 无重载：用不同函数名
来源：http://hz.jlsjyb.cn/gtlhrkcqyo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtyxegvyxl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.iojbl.cn/gtxpeqorgi.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtepmvcyaz.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtunbvsvny.html

================================================================================
来源：http://hz.hfpthk.cn/gtdxyxcuyg.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtaavcxdtc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hfpthk.cn/gtvmdwekid.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gttiiynsou.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hfpthk.cn/gtmehwiepo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pengpengdd.cyou/gtdtzslkpm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtwgvnsbzz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.c1oappe.top/gtdrnyxibo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtrwvvyelf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtjarzwzkg.html

[D02] 追加元素到末尾
来源：http://hz.yj20258888.top/gthpwxhxom.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gtpjtbvqsu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtlzjqdxkd.html

JS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtpxsbiydw.html

TS:   arr.push(4);
来源：http://hz.haohaochexian.top/gttrxnygkv.html

Java: list.add(4);
来源：http://hz.zhengqikj.top/gtdvfahejo.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gtiysimfkr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gtlmgkgjhk.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtzzjuyfnv.html

[D03] 在指定位置插入元素
来源：http://hz.ybcxt.top/gtetavwfoi.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258.top/gtfjjuisyl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zycfv.cn/gtjueanapj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ehwqpu.com/gtrxtyjcry.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenzaomai.com/gtgvknxagz.html

Java: list.add(0, 0);
来源：http://hz.cqqwz.cn/gtkvswnstz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dianchejie.cn/gtgbqzyiuv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gtjmoziwde.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtdfjmhsxp.html

[D04] 删除元素
来源：http://hz.cucudq.cn/gtspbzrbjj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenlongwang.top/gtasfkgntn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtgskqstyg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtelvuuple.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gttidonjjd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtqgltuopu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtfwnwlfmg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtvciswkwk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtejgwcvmh.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gtzhmkmcac.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gthmcfkwjs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtlkxnutgr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtbwalcrtl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fzhhl.top/gthmrptylq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gotoacloud.top/gtzmcgrxry.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xinyue.icu/gtdbiaqsrl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtyfhlnmrg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtjheqdjkl.html

[D06] 数组长度
来源：http://hz.yuxming.cn/gtqqwqhkwi.html

Py:   len(arr)
来源：http://hz.meibo888.top/gtwizxdoyu.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtgvlejmyj.html

JS:   arr.length
来源：http://hz.mhx1999.top/gtfjmiycdi.html

TS:   arr.length
来源：http://hz.52xcode.cn/gtylqfrnap.html

Java: list.size();
来源：http://hz.tanke756.top/gtylbjqqts.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gtdczumvyq.html

Ruby: arr.length; arr.size
来源：http://hz.cdnleiting.top/gtfkibmpad.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gtbetttuqe.html

[D07] 切片 / 取子数组
来源：http://hz.zhiwuduotai.top/gtspnflqdx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtqcwjygwz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sysykeji.top/gtsocfzqfc.html

JS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gtojswdxwd.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtmgbrzsfv.html

Java: list.subList(1, 4);
来源：http://hz.nanxuanxn.top/gtesvlsdbk.html

Go:   arr[1:4]
来源：http://hz.jqgfzy.top/gtksqkisra.html

Ruby: arr[1, 3]
来源：http://hz.aizwys.cn/gtputcgwzj.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhengqikj.top/gtclzcwcxa.html

[D08] 合并两个数组
来源：http://hz.jqgfzy.top/gtsqdozosq.html

Py:   a + b;  a.extend(b)
来源：http://hz.fengsongda.top/gtyqpfgqhu.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtqbplpxca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xylfe.cn/gtlegzgamj.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gtirdvvjdl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtqiokadvp.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gttstylniz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gtwvxtdrdi.html

C#:   a.Concat(b).ToList()
来源：http://hz.jianghu66.top/gtzewypisj.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtvybexmvu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtrfdpnptk.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gteqvrijpk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtawkbqhuw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhiwuduotai.top/gtxpmkegmo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gtrsyturmn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtudymosvn.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtjltoplnw.html

C#:   list.Sort();
来源：http://hz.yongpay.top/gtgfrctjxz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ppjwa.cn/gtlqihujir.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtmhcgnmjd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangshuangyany.cn/gtnuspavqd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtthoknrdz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtzlemmffv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangdashe.top/gtpbxpppcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hongshengwenyu.top/gtvmglcvsy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtfhzuxhdq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtugpbvwvg.html

[D11] 反转数组
来源：http://hz.yj202588.top/gtkgzbptuw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yuxming.cn/gtdxzyhnbz.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigfzy.top/gtnlpibmue.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtnkxepwdo.html

TS:   [...arr].reverse();
来源：http://hz.kuanghao11.cn/gtrjyttmtk.html

Java: Collections.reverse(list);
来源：http://hz.cqqwz.cn/gtaxqkbnjr.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtyorkbfvo.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gtasjtvnym.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gtaxtmlnai.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gtpqlbjzpn.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinqigfzy.top/gtmpwltwap.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtnfqgpxnh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtmpgncslt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtjvzthllk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtwunozjpj.html

Go:   slices.Index(arr, x)
来源：http://hz.zhiwuduotai.top/gtjendaftc.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gtbqjcprdf.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtyoiryvjv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtofxyhcjk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.c1oappe.top/gtatksxklw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydzc1.top/gtdpeshhwr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hammf.cn/gtdflegedv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtejdmklda.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtzhrbavhk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.havefunace.top/gthbsbbsig.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.mhx1999.top/gtusluohst.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ybcxt.top/gtaweahddu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yueranfly.top/gtnhwkeptq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtzkhdutlu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtqdeuacoc.html

JS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtbnqvoibc.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtdxlkrmig.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.havefunace.top/gtimzznjim.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtxnxkfyyq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtaovovggr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtopubxfug.html

[D15] 去重
来源：http://hz.pycfn.com/gttdmbafrk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinyuanbaomall.cn/gtqhstoopy.html

PHP:  array_unique($arr);
来源：http://hz.xingfuxueyuan.xyz/gtboweyqvp.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtmbddbehc.html

TS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtkoqhkxmk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gttjcppngx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtijksrnxg.html

Ruby: arr.uniq
来源：http://hz.redwolf501.top/gtoohgysir.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigfzy.top/gttsqgkjxb.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gthcbzoryg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jyoumei.cn/gtmljvtxmi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aibaodan.cn/gtjpdkplmo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtwjwphsma.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtzozkqyfv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtwxkqpuor.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gtxtoauwxs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtncbstwus.html

C#:   list.Sum();  list.Average()
来源：http://hz.hongshengwenyu.top/gtgjwgpynu.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtkhnpgelo.html

Py:   max(arr);  min(arr)
来源：http://hz.tian-w.cn/gtbvvynbnk.html

PHP:  max($arr);  min($arr);
来源：http://hz.xylfe.cn/gtxqhutpjo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtlvqvifdn.html

TS:   Math.max(...arr);
来源：http://hz.ybcxt.top/gthnczebpv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtwxsyphnj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gtvyyjbypb.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtazenjnux.html

C#:   list.Max();  list.Min()
来源：http://hz.yanxiufei.cn/gtvxgroqho.html

[D18] 扁平化嵌套数组
来源：http://hz.c1oappe.top/gtolmqitoe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sufxvd.cn/gtyhotnsjf.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtnvsaitzj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtgstvftqi.html

TS:   nested.flat();
来源：http://hz.quarkkingdee.top/gtsoogchbx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jianghu66.top/gtnjuuubtq.html

Go:   // 手写双层循环
来源：http://hz.vqdsnc.cn/gtpphakttq.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtrswdcupk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.kuanghao11.cn/gtntkiofyv.html


<!-- 参考信息 -->