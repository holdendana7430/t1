代发 wailian999

[C02] 默认参数
来源：http://hz.daxiang520.top/gtgljkojqm.html

Py:   def greet(name="World"): return name
来源：http://hz.hfpthk.cn/gtiarrjphu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhijiandao.cn/gtxipohsgd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tianlin.xyz/gtlrtqcqxl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenlongwang.top/gtepwkxytf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtoczbvspb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtzqpxeysw.html

Ruby: def greet(name = "World") = name
来源：http://hz.quarkkingdee.top/gteqibfhpq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cucudq.cn/gtxkzjuyyo.html

[C03] 可变参数
来源：http://hz.ydjk.org.cn/gtqtkdqjgx.html

Py:   def total(*args): return sum(args)
来源：http://hz.cqqwz.cn/gtakwhdsjr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hammf.cn/gtuldndzmg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtksqpinnh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtiflxmqey.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gtszhmgyxk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hammf.cn/gtlgqcxvdv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnqzz.top/gtwqcbugos.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtndfsxocc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dianchejie.cn/gtognszcrv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cqqwz.cn/gtpxtjgejg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sufxvd.cn/gtktvwncfh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtajnqqslv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.iojbl.cn/gtpvqecaie.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtuvolbnpm.html

Go:   // 无：用配置结构体参数
来源：http://hz.sweek.top/gtuhlgmuqu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtqpuvvnqn.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtlgzrfvdi.html

[C05] 返回多个值
来源：http://hz.wangdashe.top/gtctwzeydd.html

Py:   return a, b
来源：http://hz.yj20258888.top/gteaduhfjf.html

PHP:  return [$a, $b];
来源：http://hz.ehwqpu.com/gthomldzke.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangdashe.top/gtfrhbquho.html

TS:   return { a, b };
来源：http://hz.pycfn.com/gtqvbdnuxv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xziqi.cn/gthnpuvypg.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtsxdhqwpv.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtdiwtbnmu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gtnhwawyff.html

[C06] 匿名函数 / lambda
来源：http://hz.yonumen.top/gthimxjjor.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtsfpegfkz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gtdqphpyjd.html

JS:   const square = x => x * x;
来源：http://hz.guowangkeji.top/gtcvrqvqhn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtmaciijai.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenlongwang.top/gtlmybepdm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gzhubu.top/gtfzxkccau.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cucudq.cn/gtrptxxafl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.0kj1m.cn/gtsznysdsf.html

[C07] 把函数作为参数传入
来源：http://hz.ydjk.org.cn/gtrjymcgpv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ybcxt.top/gticahzxmz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gtitmaxfmy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tanke756.top/gtmdzntwnb.html

TS:   arr.map(String)
来源：http://hz.zhengqikj.top/gtbmhcazki.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yongpay.top/gtayclnfuj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtetwivzjv.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtozycqcao.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhaomingkeji.xyz/gtmdkblrir.html

[C08] 闭包
来源：http://hz.yj20258888.top/gtufzylgbk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yanxiufei.cn/gteyhwjyso.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fzhhl.top/gtrhrhvjdq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtmqnfxfhb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtwgmnleql.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daria6918.cn/gtqcpsjtxo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtlrgbpygv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxuanxn.top/gtepuberww.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtwebzvqgm.html

[C09] 递归
来源：http://hz.yj202588.top/gtxqgmcjqx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtcjxtlehf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtzzmkceqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtrxcmgggv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtvnhyphjw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtzaxzpbiz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jyoumei.cn/gtijbehnun.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtzsvyoowr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.meibo888.top/gtojmvfdpn.html

[C10] 变量作用域
来源：http://hz.havefunace.top/gtxpzevxip.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gttaosqqbv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydzc1.top/gtooubezvv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gtgutkdjvk.html

TS:   同 JS
来源：http://hz.yj20258.top/gtfwxamuve.html

Java: 方法内为块级作用域
来源：http://hz.shzxlz.cn/gtgncnbkmw.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtlwjnfyzf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtojjvnjsj.html

C#:   块级作用域
来源：http://hz.xylfe.cn/gthngsnuzy.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtoavmlvva.html

Py:   from module import func
来源：http://hz.vqdsnc.cn/gtsaqykpyd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtnzbmaizi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xziqi.cn/gtfnxvcpoe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtbybxkecm.html

Java: import java.util.List;
来源：http://hz.tianlin.xyz/gtyduezvyq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtxkfkojod.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtoirjsxvp.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtjedttqzh.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhaomingkeji.xyz/gtfdgevxpj.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtzbwwzjyj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cheryme.top/gtzaqxpkrc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nanxuanxn.top/gtypzzulau.html

TS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gtptohvlum.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtouzrppko.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtmfzpleqd.html

Ruby: -> { puts "run" }.call
来源：http://hz.ywan-chungtsiang.top/gtgxsrfbwp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gthmxaixoe.html

[C13] 类型声明 / 类型注解
来源：http://hz.hysaishi.cn/gthdndohqw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtrfbbklws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtjpxmksxm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yanxiufei.cn/gtbgetakja.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gtkgmiwomm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtxxksjdye.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtejjidwyq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtngxwgowf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhijiandao.cn/gtvaecbewb.html

[C14] 泛型函数
来源：http://hz.52xcode.cn/gtbotvorqw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtmvqzzizq.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtcehegmzb.html

JS:   // 无泛型
来源：http://hz.yj202588.top/gtqxuhlhrw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj202588.top/gtqqlgvktn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yongpay.top/gtdjaohhhe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tanke756.top/gtvrlcgqqf.html

Ruby: # 无泛型
来源：http://hz.jiagoushi.top/gtsesjsjvf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.0kj1m.cn/gtwmpijwlr.html

[C15] 解构 / 展开参数
来源：http://hz.haohaochexian.top/gtusvtwhum.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtgcbmwabn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sxryk.cn/gtdwkarjtg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtajdxlefk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cashguo.top/gtxmqsblmv.html

Java: // 无解构
来源：http://hz.xuetiantiany.cn/gtxetuouau.html

Go:   // 无解构
来源：http://hz.cashguo.top/gtujateera.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gttndzcemz.html

C#:   var (a, b) = pair;
来源：http://hz.guowangkeji.top/gtsjuyhzoi.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gttglyngti.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.haohaochexian.top/gtymjjvzpa.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtofwwlkda.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gtxzthtfsg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hfpthk.cn/gttqhrvxnp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtmdfjczzf.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtojldjjdf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aibaodan.cn/gtzlegurcm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.9152youxi.cn/gtsuthpnai.html

================================================================================
来源：http://hz.zdqjudy.top/gthwqgifis.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtshugtidz.html

================================================================================
来源：http://hz.yonumen.top/gtgrnivmfg.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtcgupnizo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cucudq.cn/gtkkgqjfio.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hammf.cn/gtrjddgeci.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fzhhl.top/gtgcexzhzq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fzhhl.top/gtuqqghwaw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daxiang520.top/gtkvesfdnl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhongyouzk.top/gthqsjazjy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinyuanbaomall.cn/gtwgpzvkwl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pengpengdd.cyou/gtiovokemu.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gtfekpixiv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xziqi.cn/gtnewtzfuu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gttownwpdw.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtxgccivif.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtinoxoaif.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gtgewvczro.html

Go:   arr = append(arr, 4)
来源：http://hz.meibo888.top/gtnqilgvze.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtryobkhhb.html

C#:   list.Add(4);
来源：http://hz.xziqi.cn/gtaihrgsjd.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gttiusfxpp.html

Py:   arr.insert(0, 0)
来源：http://hz.fengsongda.top/gtwsjngfln.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtsgsdsvsx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cqqwz.cn/gtnwtekvyr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.iojbl.cn/gtsyvwjjgy.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gtwcufruop.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ivvv.top/gtjlnvtuna.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangkeji.top/gtxpcphvrv.html

C#:   list.Insert(0, 0);
来源：http://hz.kuanghao11.cn/gtyzdjowfx.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtgckwmjfz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtckzorvpg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shzxlz.cn/gtqffyekye.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yangfankeji.com/gtnieqezhg.html

TS:   arr.splice(0, 1);
来源：http://hz.zhengqikj.top/gtreegrian.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.andypj.xyz/gtaozydtqu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinqigfzy.top/gtsdjjrvmn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hammf.cn/gthjnwgmnk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtpszssjxf.html

[D05] 访问与修改元素
来源：http://hz.chenlongwang.top/gtvgrnipee.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtrasfkjlg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtpulysgyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gthupjzbvm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xinyue.icu/gtfbdopmhe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sysykeji.top/gtxlhjtwxj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtfpdfqusc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtqbzuinpx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtbvysfsoe.html

[D06] 数组长度
来源：http://hz.yueranfly.top/gtbhbbgfaw.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtmqcnqstj.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtkxwpwkwo.html

JS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtidruhbjd.html

TS:   arr.length
来源：http://hz.zhixingplan.top/gtfecytvrk.html

Java: list.size();
来源：http://hz.andypj.xyz/gtbgycysrv.html

Go:   len(arr)
来源：http://hz.jiagoushi.top/gtgrdbbjni.html

Ruby: arr.length; arr.size
来源：http://hz.birdmap.top/gtihlkkypy.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtcnaccjge.html

[D07] 切片 / 取子数组
来源：http://hz.jyoumei.cn/gtrulubicz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtjfrlywjm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtdhjhnygm.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtcelgxnpa.html

TS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtecskicbp.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtoludfiam.html

Go:   arr[1:4]
来源：http://hz.andypj.xyz/gtrffxkoot.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtrnpesdrq.html

C#:   list.GetRange(1, 3);
来源：http://hz.dianchejie.cn/gtrhqduemz.html

[D08] 合并两个数组
来源：http://hz.gzhubu.top/gtwpbrmhcw.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gtffwuxgfk.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gtkqmskjur.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangshuangyany.cn/gtbkservxz.html

TS:   [...a, ...b];
来源：http://hz.gogol.net.cn/gtmmgfrwsm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtazvjxmzx.html

Go:   append(a, b...)
来源：http://hz.meibo888.top/gtmcafqvmj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jiagoushi.top/gtscujgxms.html

C#:   a.Concat(b).ToList()
来源：http://hz.shuidangran.top/gtixlzdlyb.html

[D09] 排序（升序）
来源：http://hz.havefunace.top/gtvjlfirud.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtvrorkzvp.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtrstefsde.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gtyhttltea.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtpciifrwy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xingfuxueyuan.xyz/gtobjecsvh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gtjcjzajjh.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtqvbjtrzl.html

C#:   list.Sort();
来源：http://hz.zdqjudy.top/gtllzgtmph.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yanxiufei.cn/gtokbkygde.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hfpthk.cn/gtmyiagred.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtuixautsm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtybqncemv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhixingplan.top/gtymzvuwsp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhoulong.xyz/gtwnezsprt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhongyouzk.top/gtzntbbzmr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gtufapvnxx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gtgjkqnmhj.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtuyiacoxg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj20258.top/gtemqtsfgd.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gtjfbvmbtt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gtiulxhnpf.html

TS:   [...arr].reverse();
来源：http://hz.jqgfzy.top/gthqjvsddn.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gteqpdxxcu.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtrpaswazf.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gtwrslzdan.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtszbfuamh.html

[D12] 查找元素下标
来源：http://hz.yj20258888.top/gtngmlzxqt.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtqdiqkxem.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yanxiufei.cn/gtjoreijvp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtjstloipa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtkboxzgcw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cdnleiting.top/gtyzwcvgtn.html

Go:   slices.Index(arr, x)
来源：http://hz.c1oappe.top/gtvrakzqgb.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtcwxplppg.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gtekylvrgz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtimeojyqz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tanke756.top/gtezojbhrh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.andypj.xyz/gtrjiabkpf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtrfpvlrsu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtvwxiupxi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtlfmwuvaj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gthwhchvab.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dashuyun.cn/gtuozninfe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtsbnkxltt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hywenlv.cn/gtwspbslfh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigufen.top/gtowczlpas.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgfzy.top/gtdgzmhkkz.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtcaknyzcd.html

TS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtavvvtubb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhongyouzk.top/gtbanhwvkx.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtaxejwfgr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yueranfly.top/gtbjrawysh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gtrubdfzmk.html

[D15] 去重
来源：http://hz.hammf.cn/gtwbdnqbqv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gtimdiamwe.html

PHP:  array_unique($arr);
来源：http://hz.sufxvd.cn/gtlmwyqotd.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtbyzocebm.html

TS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtefefjkuf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hywenlv.cn/gtlihsgqcx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yongpay.top/gtoemznmpb.html

Ruby: arr.uniq
来源：http://hz.zycfv.cn/gtukyirdab.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtowhuwbhh.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtgshfkleo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtvmrywexm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtyzrssgyw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gttqohnrkf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtfrahrkse.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtxlqiunyb.html

Go:   // 手写循环累加
来源：http://hz.shangyingyoupin.top/gtsfrnxvjl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gtmuriyzqe.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtftqonzbq.html

[D17] 最大值与最小值
来源：http://hz.tian-w.cn/gtjwlbuxnf.html

Py:   max(arr);  min(arr)
来源：http://hz.zhoulong.xyz/gtrnyfznkq.html

PHP:  max($arr);  min($arr);
来源：http://hz.andypj.xyz/gtyzqdnlco.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtkulmitvg.html

TS:   Math.max(...arr);
来源：http://hz.guannengcc.top/gthtjrciob.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnqzz.top/gtnzliipzb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtezwzzlxp.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtdhbsybgt.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtzguwarxy.html

[D18] 扁平化嵌套数组
来源：http://hz.c1oappe.top/gtandajxag.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.316326.xyz/gtcvqgqtfb.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gthlfzymtp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtlwpspkku.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtygyarush.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ybcxt.top/gtsvblkprm.html

Go:   // 手写双层循环
来源：http://hz.nanxuanxn.top/gtnhgueejg.html

Ruby: nested.flatten
来源：http://hz.xuanzx.com/gtxdhpfdvz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtnyignvwh.html


<!-- 参考信息 -->