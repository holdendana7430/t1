代发 wailian999

Java: if (data == null) return;
来源：http://hz.xziqi.cn/gtnwdrlqpx.html

Go:   if data == nil { return }
来源：http://hz.jinghuilouyu.cn/gtnubmmdqe.html

Ruby: return if data.nil?
来源：http://hz.sweek.top/gtrzrljwfc.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtgzbvisul.html

================================================================================
来源：http://hz.guowangkeji.top/gtladqfzrv.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtqgcxkhyf.html

================================================================================
来源：http://hz.tianlin.xyz/gtcxmhlpnp.html

[C01] 定义函数
来源：http://hz.yuxming.cn/gtixmrfcna.html

Py:   def add(a, b): return a + b
来源：http://hz.feifeiyinyue.top/gttcotlkuz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtkammzxto.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtleodrjty.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtytxtxlmc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtjiumilsu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtezwgxmur.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shangyingyoupin.top/gtatrvhnbn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtksfnutyu.html

[C02] 默认参数
来源：http://hz.yuanzhike.top/gtavctxwut.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxuanxn.top/gtehduxnfy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.mhx1999.top/gtkkklygtq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.smart0.xyz/gtajuuruyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tian-w.cn/gtpazuyuuk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenlongwang.top/gtbljyvyny.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ppjwa.cn/gtlehkcudv.html

Ruby: def greet(name = "World") = name
来源：http://hz.guowangkeji.top/gtvrdtuxll.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.316326.xyz/gtqntxosna.html

[C03] 可变参数
来源：http://hz.svipenyu.cn/gtphoidwkl.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhijiandao.cn/gtjczowoae.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangdashe.top/gtdceosuiq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtfkxpxenu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtphtypcyf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.vqdsnc.cn/gtoddmgnea.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ybcxt.top/gtmbffrutu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xziqi.cn/gtdzpsajsb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nwbrower.top/gtoaglngwu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sufxvd.cn/gttgutjdse.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydzc1.top/gtejxnjfhq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangkeji.top/gthsonrlqi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtvkynxnlq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuanzhike.top/gtgkvkorbp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hywenlv.cn/gtfgttezod.html

Go:   // 无：用配置结构体参数
来源：http://hz.0kj1m.cn/gtrvqghshw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtystjihoc.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtjkkivyan.html

[C05] 返回多个值
来源：http://hz.xuanzx.com/gtbjxhedmf.html

Py:   return a, b
来源：http://hz.ydjk.org.cn/gtqubzauye.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtajuqcizn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtpxryntpq.html

TS:   return { a, b };
来源：http://hz.daria6918.cn/gthnupydcz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.redwolf501.top/gtinyxfhcb.html

Go:   return a, b
来源：http://hz.cqqwz.cn/gtkxohpmjg.html

Ruby: return a, b
来源：http://hz.yuanzhike.top/gtujtqfmhh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jlsjyb.cn/gtpghickge.html

[C06] 匿名函数 / lambda
来源：http://hz.havefunace.top/gtjfwiymzl.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtsqpjnhqe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinqigfzy.top/gtlebcdhhp.html

JS:   const square = x => x * x;
来源：http://hz.svipenyu.cn/gtnvtpexao.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.aibaodan.cn/gtejlmrsqf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gzhubu.top/gtrpalilon.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.dashuyun.cn/gtftdqynhn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtueawenfw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sxryk.cn/gturqnnpuw.html

[C07] 把函数作为参数传入
来源：http://hz.ehwqpu.com/gtfxnujqke.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigfzy.top/gtyjynuoku.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.316326.xyz/gtwmkqyfic.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtcippzxqz.html

TS:   arr.map(String)
来源：http://hz.zhaomingkeji.xyz/gtelcdoenn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangtech.top/gtfbsariqv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.snrcjt.cn/gtfyzopolz.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhengqikj.top/gtktghuxey.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.havefunace.top/gtztorjooq.html

[C08] 闭包
来源：http://hz.shuidangran.top/gtbdiktsde.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gtdihopjjk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.bjfxy.top/gtkyeiwusj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtoqkphruh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gteshgcuoa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hywenlv.cn/gtmgepjtbz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinghuilouyu.cn/gtwojgiwxj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtienhtqjp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gthvorclij.html

[C09] 递归
来源：http://hz.bjfxy.top/gtwxxlzalm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtxhhhnukw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pengpengdd.cyou/gtqtmthbqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtcpqnzywk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gttxdqmljw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.bjfxy.top/gtryxxbpws.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtckmkeaax.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yvedp.cn/gtlwqqairr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtenoylhrc.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtoqjmhphy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gotoacloud.top/gtzjiekhbm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pycfn.com/gthebutfws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aibaodan.cn/gtzyiokeaj.html

TS:   同 JS
来源：http://hz.hnxiangtu.top/gtabzevccv.html

Java: 方法内为块级作用域
来源：http://hz.quarkkingdee.top/gtschctojw.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gthbfjuzqd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jianghu66.top/gtxgvggzvl.html

C#:   块级作用域
来源：http://hz.nwbrower.top/gtjolnqaga.html

[C11] 模块导入与导出
来源：http://hz.birdmap.top/gtlzzcoxon.html

Py:   from module import func
来源：http://hz.fengsongda.top/gtiykasuth.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shuidangran.top/gtrcclcqmp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangtech.top/gthxyzqawy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dianchejie.cn/gtzfyhhsxh.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtbtfmljcj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fengsongda.top/gtgwassasf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtlclniens.html

C#:   using System.Text;
来源：http://hz.ppjwa.cn/gtkwdgccni.html

[C12] 立即执行函数 IIFE
来源：http://hz.vqdsnc.cn/gtgfvqcohy.html

Py:   (lambda: print("run"))()
来源：http://hz.jyoumei.cn/gtmufdcoru.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtipbzahns.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtnohoxxto.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtmvzdymwp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yanxiufei.cn/gtzkkkqmwp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtytcqzuaf.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gtckossune.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.snrcjt.cn/gtpseucnqy.html

[C13] 类型声明 / 类型注解
来源：http://hz.shangyingyoupin.top/gtskpwjyap.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cashguo.top/gttnoqabws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtrpgpasmb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pycfn.com/gtkjjdjhki.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtybypyuyy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtjqjzpvlo.html

Go:   func add(a, b int) int
来源：http://hz.cdnleiting.top/gtcmqkkfsu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.smart0.xyz/gtptqkeigb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pycfn.com/gtvkcycpgz.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtmigerpuq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhoulong.xyz/gttkbqzkzz.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gtziscnrld.html

JS:   // 无泛型
来源：http://hz.chenzaomai.com/gttjtwrxex.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtlkwnypmw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gttwtmqvcz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gtwhmifnpo.html

Ruby: # 无泛型
来源：http://hz.ppjwa.cn/gtfpnphxhb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gttgdbhuwp.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gtmzqwcskj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtfiqhbjvy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtiljelmto.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gteyannzvf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.iojbl.cn/gtafcyyfxe.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gtjiohddcc.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtmekbgszz.html

Ruby: a, b = pair
来源：http://hz.zycfv.cn/gtfwneuqvm.html

C#:   var (a, b) = pair;
来源：http://hz.xuetiantiany.cn/gtaypqghxm.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtykyqivkd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gtozecdyrv.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtzawiafoo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinghuilouyu.cn/gtpannvdnu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cdnleiting.top/gthifvrhur.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yueranfly.top/gtsozuznrx.html

Go:   // 无重载：用不同函数名
来源：http://hz.sxryk.cn/gtiufotulp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hongshengwenyu.top/gtcyfauich.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.meibo888.top/gtotubrmtw.html

================================================================================
来源：http://hz.nwbrower.top/gtycbtwvdg.html

D. 数组 / 列表 / 集合
来源：http://hz.yongpay.top/gtlaubjoaj.html

================================================================================
来源：http://hz.daxiang520.top/gtslxsgbyr.html

[D01] 创建数组 / 列表
来源：http://hz.nanxinkj.top/gtjgcgkbuo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258.top/gtmnkfmooy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gttllnpeno.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tian-w.cn/gtfnhjcasy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtrepkzxrj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtlbtmrguh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhoulong.xyz/gtpshgnmhl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jianghu66.top/gtfvwnwtyv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtpqwngjtl.html

[D02] 追加元素到末尾
来源：http://hz.nwbrower.top/gtuzmyzdpj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.316326.xyz/gtgqdqftld.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gzhubu.top/gttiyvrkaa.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtxyehdvvc.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gthxbmnjwt.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gtnqrcafvb.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtekryvbxb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhoulong.xyz/gtpqfzffnc.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtijkiuwrm.html

[D03] 在指定位置插入元素
来源：http://hz.cqqwz.cn/gthoecvqsm.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtrjlrysuy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yongpay.top/gtzacvwcgs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuanzhike.top/gtmubbvboj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yangfankeji.com/gtmiewziiz.html

Java: list.add(0, 0);
来源：http://hz.jinqigufen.top/gtcddybbvj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtieezltgg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtvxknlxup.html

C#:   list.Insert(0, 0);
来源：http://hz.jiagoushi.top/gtxmgmpuqf.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtmodncwyc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtnyqltjmw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtfrjhpuyb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.redwolf501.top/gtqsuwcduj.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtfojvuyob.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cashguo.top/gtpivuvjpq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtjgflnfve.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydjk.org.cn/gtiiflecbh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cheryme.top/gtlbwfnifg.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtfjaftsqi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtfmdhskwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtlwptfnlz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nwbrower.top/gtwsuwngcv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gtvhlnhvhk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtihetvzsk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtuewlpaha.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtigjjahjt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtlcxjfxjv.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gthwyfrpyr.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtmmfvmtpf.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtuozqyczk.html

JS:   arr.length
来源：http://hz.yj20258.top/gtivsvyogo.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtpuavsdme.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtniiqbdpy.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gtqdtfnwsc.html

Ruby: arr.length; arr.size
来源：http://hz.ybcxt.top/gtiuvygtji.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtalsbtjvp.html

[D07] 切片 / 取子数组
来源：http://hz.zdqjudy.top/gtywpyptfe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.quarkkingdee.top/gtmhkqxpye.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cqqwz.cn/gtuvpvwnzt.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtdxznyrmj.html

TS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtaxzznekl.html

Java: list.subList(1, 4);
来源：http://hz.redwolf501.top/gtvlxvvitz.html

Go:   arr[1:4]
来源：http://hz.aizwys.cn/gtjllznxia.html

Ruby: arr[1, 3]
来源：http://hz.hammf.cn/gtuabviskd.html

C#:   list.GetRange(1, 3);
来源：http://hz.ehwqpu.com/gthswoomra.html

[D08] 合并两个数组
来源：http://hz.316326.xyz/gtsunvbork.html

Py:   a + b;  a.extend(b)
来源：http://hz.nwbrower.top/gtlytemhma.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxuanxn.top/gtrluafnkj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gtqdoawmwp.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtyzbemsfs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ivvv.top/gtdumffdao.html

Go:   append(a, b...)
来源：http://hz.hywenlv.cn/gtnxoeetdo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhongyouzk.top/gtwstmsdzj.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangkeji.top/gthdldixqa.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtcwqnucwi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtkibwudiu.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtfsirjamz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.316326.xyz/gtjcqnrffr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.9152youxi.cn/gtqpbxccib.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.mhx1999.top/gtmtcwttmf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.bjfxy.top/gtlvdjoxcn.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtpdvcybbo.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtnscpxmew.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jiagoushi.top/gtizbvshsj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tanke756.top/gtphsgkhdm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtzatziahd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtsvromrtb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtsalcqztf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yangfankeji.com/gtfjxmoazd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ywan-chungtsiang.top/gtiaqzmerp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aizwys.cn/gttzxktmoz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtvifclyyp.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtijmbkktz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.redwolf501.top/gtkpprnfua.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtaksldsnc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.andypj.xyz/gtpjcdnywj.html

TS:   [...arr].reverse();
来源：http://hz.yvedp.cn/gtaktncihy.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtjzphyczx.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtmqznzgpq.html

Ruby: arr.reverse
来源：http://hz.bjfxy.top/gtfhbtrbcl.html

C#:   list.Reverse();
来源：http://hz.yonumen.top/gtmlibvhwg.html

[D12] 查找元素下标
来源：http://hz.jyoumei.cn/gtigpnhsdj.html

Py:   arr.index(x);  x in arr
来源：http://hz.snrcjt.cn/gtvxkqclpv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtgjxqdejm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtfqznkwox.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtmhthlomb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenjidiqi.icu/gtgjogduhh.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtgkzcedpg.html

Ruby: arr.index(x)
来源：http://hz.hywenlv.cn/gtmwfysxhx.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gtfoudmdug.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtmvdkmbeq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtnljlygiy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gthoixafmb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtbrlzmqdy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtxjyihjrw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cdnleiting.top/gtuetandwe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtspijntdz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gtsuwocpti.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yanxiufei.cn/gtlmendrnj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jianghu66.top/gtzstpfxuk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gthoogbyhj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtltthtltf.html

JS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtxkpqbqfa.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtnjvrclqc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gttsupsszg.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gthddjigfo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gtuunfzxza.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gtwvvmflcl.html

[D15] 去重
来源：http://hz.ehwqpu.com/gtrilcfydb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aizwys.cn/gtwdwyeauw.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gttndyifvy.html

JS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtaauilibn.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gteshjbujg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gtnfooznvx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cqqwz.cn/gtepszcipi.html

Ruby: arr.uniq
来源：http://hz.jinghuilouyu.cn/gtjtdebyny.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgufenzy.top/gtjdyltera.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gtcmjoszsn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gttuowvlir.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xziqi.cn/gtrddvdblr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtcbemnvii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtjrhaiman.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinyuanbaomall.cn/gtqualfksi.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtjosydmyf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtpqzqxehr.html

C#:   list.Sum();  list.Average()
来源：http://hz.hammf.cn/gtrtgcbdmy.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtdcbdcaen.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gteuzuqtmn.html


<!-- 参考信息 -->