代发 wailian999

PHP:  $a && $b || !$c
来源：http://hz.cucudq.cn/gtmtdpkmnv.html

JS:   a && b || !c
来源：http://hz.hysaishi.cn/gtikvpedah.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtiylkynxo.html

Java: a && b || !c
来源：http://hz.yj20258888.top/gtbsoktpuh.html

Go:   a && b || !c
来源：http://hz.yanxiufei.cn/gtbkfwxban.html

Ruby: a && b || !c
来源：http://hz.yvedp.cn/gtowmvqvko.html

C#:   a && b || !c
来源：http://hz.yueranfly.top/gtzkkhtuqs.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydjk.org.cn/gtjuomrade.html

Py:   if not data: return
来源：http://hz.guowangkeji.top/gtudrwdefs.html

PHP:  if (!$data) { return; }
来源：http://hz.yj202588.top/gtozzsojrz.html

JS:   if (!data) return;
来源：http://hz.hammf.cn/gtfpkzxmld.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtvmlhqoar.html

Java: if (data == null) return;
来源：http://hz.zhoulong.xyz/gtoqdizjmx.html

Go:   if data == nil { return }
来源：http://hz.pengpengdd.cyou/gtqeaicwpc.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtyazixyly.html

C#:   if (data == null) return;
来源：http://hz.jinqigufen.top/gtnpjsapkx.html

================================================================================
来源：http://hz.zycfv.cn/gtyzuqvfzq.html

C. 函数与作用域
来源：http://hz.yonumen.top/gtkohnrqhf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtppgyynma.html

[C01] 定义函数
来源：http://hz.andypj.xyz/gtxytftgmz.html

Py:   def add(a, b): return a + b
来源：http://hz.xylfe.cn/gtrifjvmbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtqqzkkozj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gogol.net.cn/gtbvbdhjir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtkxclohrj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtljctnoba.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gttwftgnqq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtbxnrceqw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtpzrnorty.html

[C02] 默认参数
来源：http://hz.hnxiangtu.top/gtgnaommdp.html

Py:   def greet(name="World"): return name
来源：http://hz.hongshengwenyu.top/gtstukxkrl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258888.top/gtwcvepkmb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hammf.cn/gttsdiqdic.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pycfn.com/gtrfvikwxc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ywan-chungtsiang.top/gtejuaxxzz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hongshengwenyu.top/gtfdflthvj.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtebanzico.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtnnoyaskp.html

[C03] 可变参数
来源：http://hz.chenjidiqi.icu/gtppjsanrs.html

Py:   def total(*args): return sum(args)
来源：http://hz.xinyue.icu/gtrcycyjbr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zycfv.cn/gtdrmamlzp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtcgdsjnje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtqjyfaxur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fzhhl.top/gttyuhzcin.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtndzgktkr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtjsaqjwng.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigfzy.top/gtlpofsupn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.birdmap.top/gtrqcmgmsk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yonumen.top/gtopyxlici.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cqqwz.cn/gtjaetataw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtzqlieasx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nwbrower.top/gtnfmgodiq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.9152youxi.cn/gtngwsqlpr.html

Go:   // 无：用配置结构体参数
来源：http://hz.pengpengdd.cyou/gteihgvccc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtafauqzrq.html

C#:   f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtxqkzsbkd.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtinssshih.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtmzkecklc.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtzxptqryd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fengsongda.top/gtebooscom.html

TS:   return { a, b };
来源：http://hz.zycfv.cn/gtstdznqmv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtvoolsnkb.html

Go:   return a, b
来源：http://hz.quarkkingdee.top/gtfbtvjfmf.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtanimubcp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xingfuxueyuan.xyz/gtaoqzrjks.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangtech.top/gtmjwegmcj.html

Py:   square = lambda x: x * x
来源：http://hz.nwbrower.top/gtusksxddi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sxryk.cn/gtjzdvcesk.html

JS:   const square = x => x * x;
来源：http://hz.sysykeji.top/gtmmmmhyze.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj202588.top/gtqnfykvdd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jlsjyb.cn/gtnbeyrgrf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jlsjyb.cn/gttsmpnxnq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenzaomai.com/gtixkberkp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtqejobtsm.html

[C07] 把函数作为参数传入
来源：http://hz.ivvv.top/gthwlkslly.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtigmlxdmr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtxaayfkxy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gtitvxufsp.html

TS:   arr.map(String)
来源：http://hz.jlsjyb.cn/gtgxgjrsyi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sufxvd.cn/gtvzemesra.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ehwqpu.com/gtrdbmzejz.html

Ruby: arr.map(&:upcase)
来源：http://hz.jqgufenzy.top/gtjhmygvzl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ybcxt.top/gtcsbxswxw.html

[C08] 闭包
来源：http://hz.9152youxi.cn/gtfmnaijrh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gzhubu.top/gtwxxftdlm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cheryme.top/gtfxrfhumg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtdsfbsspf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtnaxuzktk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tian-w.cn/gtxtjlrqpj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtvfuzkhci.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cheryme.top/gtaqvyxacb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtpthefbjf.html

[C09] 递归
来源：http://hz.zycfv.cn/gtiptpwyrf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuanzx.com/gtroxzsfjt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtxtxxpfra.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.9152youxi.cn/gtmtrrqfeb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtomrcgdrl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.smart0.xyz/gtqqclzguj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yuxming.cn/gtnkanmbal.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sweek.top/gtjbjyrapl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zycfv.cn/gtysyozpig.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtzyevzbor.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gttuyesuuo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ivvv.top/gtrmrevyrr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jlsjyb.cn/gthiiurios.html

TS:   同 JS
来源：http://hz.aizwys.cn/gtdawfzrgb.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtgooatxkn.html

Go:   花括号块级作用域
来源：http://hz.jiagoushi.top/gtgdgohbne.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yongpay.top/gtzcjynzlr.html

C#:   块级作用域
来源：http://hz.hongshengwenyu.top/gtslogmvcw.html

[C11] 模块导入与导出
来源：http://hz.cucudq.cn/gtqjlwbynw.html

Py:   from module import func
来源：http://hz.aibaodan.cn/gtbskonvpe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtxcpnmwhc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aibaodan.cn/gtxprtqlgr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigfzy.top/gtezundjaf.html

Java: import java.util.List;
来源：http://hz.jlsjyb.cn/gtbshihrrg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgufenzy.top/gtkqmjlivu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhijiandao.cn/gtypgtnyry.html

C#:   using System.Text;
来源：http://hz.bjfxy.top/gtslxeomit.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtjllwirsh.html

Py:   (lambda: print("run"))()
来源：http://hz.vqdsnc.cn/gtikhjvwcn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtubgorbih.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gttzudfuuv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtpmbjlqev.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gtmmpqoehp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tanke756.top/gtytfnolbc.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtwcylimsn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtsubethpz.html

[C13] 类型声明 / 类型注解
来源：http://hz.snrcjt.cn/gthagjzibh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ppjwa.cn/gtxrqtoias.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtzfjwrauf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtrtuzwzlm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gttpxawzyr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gttgtjioyf.html

Go:   func add(a, b int) int
来源：http://hz.shangyingyoupin.top/gtbcvhlfje.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtvplavlgz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gtwfvzrrwn.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gthfisbesf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgfzy.top/gtwywuuxyk.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gttrsyqwfd.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtyhdbkour.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xinyue.icu/gtmiolcypd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yanxiufei.cn/gttqxfajge.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtxrgbiypw.html

Ruby: # 无泛型
来源：http://hz.jqgfzy.top/gtmwkksrfc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtjlarbfar.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gttflnvvnr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnqzz.top/gtzzlzvcjo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtuiiozafj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtndabkmky.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gttdpjfwrp.html

Java: // 无解构
来源：http://hz.havefunace.top/gtctjhqmbu.html

Go:   // 无解构
来源：http://hz.shangyingyoupin.top/gtkwoeojrj.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gtvctrghsu.html

C#:   var (a, b) = pair;
来源：http://hz.jianghu66.top/gtobcexmzw.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gtfcsqyfew.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtpwjwlder.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtnlsgctgz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhiwuduotai.top/gtesdxaxjy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gtdifssznh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtobpnonoa.html

Go:   // 无重载：用不同函数名
来源：http://hz.jlsjyb.cn/gtnuomrfbo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gtllnfrduj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gtsrpqpvyj.html

================================================================================
来源：http://hz.gogol.net.cn/gtffmypunb.html

D. 数组 / 列表 / 集合
来源：http://hz.sysykeji.top/gtkphlbwaw.html

================================================================================
来源：http://hz.chenzaomai.com/gtkpsfzjqe.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gthbigqcda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gttfrfndhp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangshuangyany.cn/gtnzbftcbp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gtrynybfgz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gogol.net.cn/gtseujtfnk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtapxfwwso.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangshuangyany.cn/gtyowrfqnd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtmczpdwvn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.svipenyu.cn/gthwyrxwoc.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gthvuxqbez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.redwolf501.top/gtbpfiefmg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtigxsamct.html

JS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtmedznmaz.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtynhihqde.html

Java: list.add(4);
来源：http://hz.guowangkeji.top/gtuqzmzsmm.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtokmzopfl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gtrnnifqhc.html

C#:   list.Add(4);
来源：http://hz.zhixingplan.top/gtmkmoxatn.html

[D03] 在指定位置插入元素
来源：http://hz.hfpthk.cn/gtaupboepq.html

Py:   arr.insert(0, 0)
来源：http://hz.zhoulong.xyz/gtzmmhcecb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuxming.cn/gtcqciafyc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydzc1.top/gtdtnerzlh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtvaftimiu.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangkeji.top/gtqcbzrruy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ivvv.top/gtmegfpjxp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gttsszhxnx.html

C#:   list.Insert(0, 0);
来源：http://hz.sxryk.cn/gtwealqggg.html

[D04] 删除元素
来源：http://hz.52xcode.cn/gtjvigcwqr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gtmpgyfxbb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtdsqeyzvk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangkeji.top/gtqkghgvnj.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gthqmgslss.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtxnydmqbz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.dianchejie.cn/gtdefwxvjd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hysaishi.cn/gttuytdyld.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtwdigdskz.html

[D05] 访问与修改元素
来源：http://hz.pengpengdd.cyou/gtxgxjiesi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtthnyyxyr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtcjjtpkck.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yangfankeji.com/gtlyhqebit.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtquwlehme.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtfsngywdm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtwkstaghm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtafpfmnsh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtfawpfqbh.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gtegoyjylr.html

Py:   len(arr)
来源：http://hz.jinqigufen.top/gtanotxisa.html

PHP:  count($arr);
来源：http://hz.shanyushiyangkeji.top/gtbkgrzssg.html

JS:   arr.length
来源：http://hz.wangshuangyany.cn/gtgrlgwyei.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtrqhrsrdc.html

Java: list.size();
来源：http://hz.ywan-chungtsiang.top/gtmzjzsajq.html

Go:   len(arr)
来源：http://hz.ppjwa.cn/gtjiqlkybc.html

Ruby: arr.length; arr.size
来源：http://hz.bjfxy.top/gtdbfmdauw.html

C#:   list.Count;
来源：http://hz.gaohongyu789.top/gtmitwhkvv.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gtvulftxgu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtbfuvlhxz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yanxiufei.cn/gtyjupfieo.html

JS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtktnqbfnv.html

TS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtmkakccqf.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtbmdxucdu.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gthoadxarv.html

Ruby: arr[1, 3]
来源：http://hz.xuetiantiany.cn/gtiwysoiox.html

C#:   list.GetRange(1, 3);
来源：http://hz.hfpthk.cn/gtbfsuzqxp.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtioztnoam.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtxhuadrso.html

PHP:  array_merge($a, $b);
来源：http://hz.smart0.xyz/gttmlwqcjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sweek.top/gttufprrsj.html

TS:   [...a, ...b];
来源：http://hz.fengsongda.top/gtrsfxusut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jyoumei.cn/gtnrynumba.html

Go:   append(a, b...)
来源：http://hz.0kj1m.cn/gthzwnjxuy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtljoyhbqi.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtzbfmpfay.html

[D09] 排序（升序）
来源：http://hz.pycfn.com/gtetfbikyx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtmsfafzrd.html

PHP:  sort($arr);
来源：http://hz.andypj.xyz/gtnjtqpzzj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhaomingkeji.xyz/gtkqxowjau.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtgqkfudcl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtthpeocmt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gtwdmrctts.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtfhccxuuk.html

C#:   list.Sort();
来源：http://hz.wangdashe.top/gtbtsyywdo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtpdjolzuo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuetiantiany.cn/gtwcvqaxhd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtkshbqupo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtgxqkzwqw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtdxurumxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtvpmjiken.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtxupqvbwz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtrtmetiml.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zycfv.cn/gtwtxumnlv.html

[D11] 反转数组
来源：http://hz.guannengcc.top/gtudqdkqzs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtubkfrfqp.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtwqlcpxkk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtrcdyafdc.html

TS:   [...arr].reverse();
来源：http://hz.tian-w.cn/gtikedyhef.html

Java: Collections.reverse(list);
来源：http://hz.tanke756.top/gtvdaowvsy.html

Go:   slices.Reverse(arr)
来源：http://hz.hywenlv.cn/gtqatkzzgz.html

Ruby: arr.reverse
来源：http://hz.hfpthk.cn/gtvefyzbta.html

C#:   list.Reverse();
来源：http://hz.jinqigfzy.top/gttmvgoxna.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtjswrlfar.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gtzxatowtf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtfakzapkv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtuojafnnk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtwvshstac.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gtbakexrvz.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gttuhsshra.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gtplkkbdjb.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtdwrvdqss.html

[D13] 过滤（保留满足条件的）
来源：http://hz.iojbl.cn/gtcfftllqn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xylfe.cn/gtknxjlvut.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtzdbpiawj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtjecanzuv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtsaycovuy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hnqzz.top/gtehfutbox.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.316326.xyz/gtgtbihjrf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtnejgxpcs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtysgfaqks.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangtech.top/gtgiokhiyl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hongshengwenyu.top/gturlbfrbp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtojyykodf.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtjujufjyq.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtmdrgmeun.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtkrkoipyl.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtiuyvrlbt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtfzrtrxdu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtoxulmsrz.html

[D15] 去重
来源：http://hz.guowangkeji.top/gtcsuxhspj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtddxxttyp.html

PHP:  array_unique($arr);
来源：http://hz.ydjk.org.cn/gtrhkchumn.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtrhuvjxly.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtwdzcjork.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gthdajmiiu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigufen.top/gtkncbrfcf.html

Ruby: arr.uniq
来源：http://hz.jinqigufen.top/gttyesatpy.html


<!-- 参考信息 -->