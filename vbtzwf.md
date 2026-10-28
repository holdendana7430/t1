代发 wailian999

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtrqdaiqdc.html

PHP:  if (!$data) { return; }
来源：http://hz.yj202588.top/gtxofvajtq.html

JS:   if (!data) return;
来源：http://hz.chenzaomai.com/gtntesjrem.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtccialbig.html

Java: if (data == null) return;
来源：http://hz.jqgfzy.top/gttnwnnsna.html

Go:   if data == nil { return }
来源：http://hz.gotoacloud.top/gtkumkjxgs.html

Ruby: return if data.nil?
来源：http://hz.zhiwuduotai.top/gtiehgdcuj.html

C#:   if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gtgnzvcwgf.html

================================================================================
来源：http://hz.birdmap.top/gtqdqfmdlx.html

C. 函数与作用域
来源：http://hz.dianchejie.cn/gtamtokefq.html

================================================================================
来源：http://hz.svipenyu.cn/gtxijfvrdb.html

[C01] 定义函数
来源：http://hz.quarkkingdee.top/gtmtxzsycj.html

Py:   def add(a, b): return a + b
来源：http://hz.tian-w.cn/gttfzabdsh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtnfyjkdea.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yongpay.top/gtforaxqdn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtpihgmqzz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtapidijse.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dashuyun.cn/gtufbvbqxw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.haohaochexian.top/gttbytslrh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtqdwpvnps.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtfbhcowju.html

Py:   def greet(name="World"): return name
来源：http://hz.zhixingplan.top/gtnuwkywwy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtrzznaehw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cashguo.top/gtifkcrlnk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yangfankeji.com/gtebgcevzy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shangyingyoupin.top/gtlegsnhkr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.snrcjt.cn/gtzzsemnuk.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtnfpavwup.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pengpengdd.cyou/gtlozgyeos.html

[C03] 可变参数
来源：http://hz.jiagoushi.top/gtbfytphjd.html

Py:   def total(*args): return sum(args)
来源：http://hz.tian-w.cn/gtgctpjarl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnqzz.top/gtovxtjzzl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtrorsamjt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtoitxtilh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.svipenyu.cn/gtkdciiarh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangtech.top/gtbmnrvaiu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gtokugolhm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aizwys.cn/gtylcgjgcv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pycfn.com/gtyvfjyntt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hongshengwenyu.top/gtcshhugsl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hongshengwenyu.top/gtrfcdklve.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhengqikj.top/gtcsoxnbdi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuxming.cn/gtgfrcnuge.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hongshengwenyu.top/gtrkjtqyrp.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gtouwypzkq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtqnfucywi.html

C#:   f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtjtrybtks.html

[C05] 返回多个值
来源：http://hz.nanxinkj.top/gtbfexyxvt.html

Py:   return a, b
来源：http://hz.yongpay.top/gtmaalkvla.html

PHP:  return [$a, $b];
来源：http://hz.guannengcc.top/gtzjicsose.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnqzz.top/gtltcnyeea.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtqjfwtbpn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cashguo.top/gtbucheweh.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtzzdboctk.html

Ruby: return a, b
来源：http://hz.haohaochexian.top/gtxkgeecxh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gteupgfrwr.html

[C06] 匿名函数 / lambda
来源：http://hz.dashuyun.cn/gtmiyorskd.html

Py:   square = lambda x: x * x
来源：http://hz.gogol.net.cn/gtrhejscyv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.smart0.xyz/gtgkjmokrv.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtzmskzeyr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxuanxn.top/gtcmaywwkn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gtztcpblxk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hywenlv.cn/gtxdsvhhnu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtuwwpmyhb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuanzx.com/gtuxvrnpga.html

[C07] 把函数作为参数传入
来源：http://hz.c1oappe.top/gtsqlimvhj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fzhhl.top/gtxxvxktuk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.meibo888.top/gtddwfscii.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shuidangran.top/gtntbfvbas.html

TS:   arr.map(String)
来源：http://hz.xylfe.cn/gtegjdheox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnxiangtu.top/gtqrpvduob.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtngzdccxl.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhiwuduotai.top/gtlrwqvxfh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhaomingkeji.xyz/gtbgpfsoex.html

[C08] 闭包
来源：http://hz.guannengcc.top/gttruhttin.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guannengcc.top/gtfbzqymgk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gotoacloud.top/gtjdcrpxoz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtbgegihhv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtnswtcfer.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tanke756.top/gtaccwwukk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aibaodan.cn/gtenfynvtc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gtxbabdxup.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtbvmlqtmj.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtgqidtvok.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hammf.cn/gticbgxecq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtyvsnyngm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gttianccnc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gttpjupyai.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ehwqpu.com/gtwhreencg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nwbrower.top/gthxzymqqo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.smart0.xyz/gtzvcbxmin.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.birdmap.top/gtorvgdidk.html

[C10] 变量作用域
来源：http://hz.chenzaomai.com/gtoqovurrl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.snrcjt.cn/gtdqzuqufr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangshuangyany.cn/gtsofubiuu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.vqdsnc.cn/gtmasyshpi.html

TS:   同 JS
来源：http://hz.birdmap.top/gtxytgqyaj.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtgweuvmrz.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtqtukrusf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhongyouzk.top/gtkwvheccr.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gthkqkkolb.html

[C11] 模块导入与导出
来源：http://hz.yvedp.cn/gthlirhapt.html

Py:   from module import func
来源：http://hz.xuanzx.com/gtyyfgaejv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtmpwnoarz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zycfv.cn/gtlpdxjhjs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.bjfxy.top/gtctkoxzzx.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtcbbrvjox.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtnzhbzkge.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxinkj.top/gtcrktcpgr.html

C#:   using System.Text;
来源：http://hz.zhengqikj.top/gtwprbkycz.html

[C12] 立即执行函数 IIFE
来源：http://hz.yvedp.cn/gtnjyyetzt.html

Py:   (lambda: print("run"))()
来源：http://hz.yonumen.top/gttpnpcumo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yongpay.top/gtsqucrstu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtumcsersy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtrnhllasz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hfpthk.cn/gtylohyukv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yonumen.top/gtwdycvxta.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtsdyayyza.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hysaishi.cn/gtvmvhmini.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj202588.top/gtdvjufdep.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.svipenyu.cn/gtbzntnswd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtvqrggmtn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gtgihmgisn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtdqjjofbd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gthcjxwrzp.html

Go:   func add(a, b int) int
来源：http://hz.hammf.cn/gtrsolarhs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtgvdzekes.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtrqdhrzzc.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gteyvmdebp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shuidangran.top/gtumgbqmny.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtttuplynw.html

JS:   // 无泛型
来源：http://hz.pycfn.com/gtmmqekdca.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gtncqtmscc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigufen.top/gtevtejror.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gtdcexogub.html

Ruby: # 无泛型
来源：http://hz.hysaishi.cn/gtcjmygjif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtbcindecd.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangtech.top/gtbgdjfcnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shzxlz.cn/gtgbzmgsge.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ivvv.top/gtykhwmuwo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtdqacwxnr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuxming.cn/gtocejcnrc.html

Java: // 无解构
来源：http://hz.havefunace.top/gtnxksffad.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtejjtbtgt.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtmvnkcsgn.html

C#:   var (a, b) = pair;
来源：http://hz.smart0.xyz/gtjsjykggj.html

[C16] 函数 / 方法重载
来源：http://hz.andypj.xyz/gtmbvnjcjg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuanzx.com/gttzrplzot.html

PHP:  // 无重载
来源：http://hz.9152youxi.cn/gtogcfnuyh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zdqjudy.top/gtmnlpksxb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtebejjhuj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258888.top/gtbvlfghbq.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtyoloehzx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cqqwz.cn/gtuwpfowyd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtmpptfqlv.html

================================================================================
来源：http://hz.jyoumei.cn/gtzxurywte.html

D. 数组 / 列表 / 集合
来源：http://hz.hammf.cn/gtegmwanyh.html

================================================================================
来源：http://hz.havefunace.top/gtiilglmia.html

[D01] 创建数组 / 列表
来源：http://hz.ppjwa.cn/gtljcdrvht.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gtbtpefwxe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gtdxtoxphm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zycfv.cn/gtxrdzqcho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.vqdsnc.cn/gtpguagmql.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtjzsbjpvq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gthdvappak.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gteyfptlcg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gtmbrrjcxs.html

[D02] 追加元素到末尾
来源：http://hz.snrcjt.cn/gtiwmmlvev.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hongshengwenyu.top/gtccnqrhmq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtzjtfaocl.html

JS:   arr.push(4);
来源：http://hz.52xcode.cn/gtlrprshaj.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtxpcrckex.html

Java: list.add(4);
来源：http://hz.gotoacloud.top/gtfpgiuvwa.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtseayonpw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.birdmap.top/gtueidnpxq.html

C#:   list.Add(4);
来源：http://hz.ppjwa.cn/gttvdoarzs.html

[D03] 在指定位置插入元素
来源：http://hz.smart0.xyz/gtmfhbgdqz.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtnbshubsm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cheryme.top/gtltjnjdis.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.svipenyu.cn/gtqsggwhxm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangtech.top/gtmsfbuupc.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtznafilzl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xingfuxueyuan.xyz/gtpzfokvbw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.meibo888.top/gthbzhlnej.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtzxomwlwm.html

[D04] 删除元素
来源：http://hz.aibaodan.cn/gtdummywmi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtlzdpiamp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.0kj1m.cn/gtpepsofza.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ybcxt.top/gtaczxhait.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtywyjphbz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gthdakwnaw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhengqikj.top/gtnkzuxwjv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtaveyojwz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aizwys.cn/gtlwikvmsx.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtflijkadq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtvbvgoogk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gthrstpehn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gtokzhtfzr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gtpzlxozqm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtxoexxtrw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtfprmrlmz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtvwmlxcyv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yanxiufei.cn/gtrwozmkld.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtbjeymxpr.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtqjjdkqyb.html

PHP:  count($arr);
来源：http://hz.guowangkeji.top/gtnhimeuxz.html

JS:   arr.length
来源：http://hz.ivvv.top/gtcgszhzxx.html

TS:   arr.length
来源：http://hz.jiagoushi.top/gtmxdccxtw.html

Java: list.size();
来源：http://hz.yangfankeji.com/gtkyawtecv.html

Go:   len(arr)
来源：http://hz.vqdsnc.cn/gtpgcandcv.html

Ruby: arr.length; arr.size
来源：http://hz.jqgufenzy.top/gtczgbgnol.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtbjserusr.html

[D07] 切片 / 取子数组
来源：http://hz.yangfankeji.com/gthrtzsodf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gttmqjtvtl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shuidangran.top/gtecspzjxq.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtmpddwynl.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtkhirjvnw.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtevlnnzrp.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtblmvkntc.html

Ruby: arr[1, 3]
来源：http://hz.yuxming.cn/gttkcqwdty.html

C#:   list.GetRange(1, 3);
来源：http://hz.haohaochexian.top/gtqjhhjsxl.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gtvfzyqsad.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtqgismzoo.html

PHP:  array_merge($a, $b);
来源：http://hz.ydjk.org.cn/gtybmvezru.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zdqjudy.top/gtacvnjevk.html

TS:   [...a, ...b];
来源：http://hz.hnqzz.top/gtleuihrgc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnqzz.top/gtrnwsxfae.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtgjzrhjnx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gteezlnszp.html

C#:   a.Concat(b).ToList()
来源：http://hz.jyoumei.cn/gtscnbayys.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtflshlhne.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtanszayiu.html

PHP:  sort($arr);
来源：http://hz.yonumen.top/gtkwyvpkzp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtmcukhmwz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtdtuqcjzj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.mhx1999.top/gtehxwzvwb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuxming.cn/gtcnkkyjxu.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtbmynbxmk.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtagvtgqsd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fengsongda.top/gthzlgtspr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gtzvthrdkl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtzfhpehmg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtmomcvihr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gthwldaiit.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnxiangtu.top/gtxogjerii.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gtmjvkmaxv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.pengpengdd.cyou/gtqqmkjobf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cucudq.cn/gtjqcmhysh.html

[D11] 反转数组
来源：http://hz.0kj1m.cn/gthgqgnhwm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtlwvlrabq.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtkoktyhec.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtklynjihd.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtkqxqupho.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtenneecwg.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtfcqieyjt.html

Ruby: arr.reverse
来源：http://hz.yangfankeji.com/gtrbumnvsh.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtkuqvujpp.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtqzsxwyrt.html

Py:   arr.index(x);  x in arr
来源：http://hz.sweek.top/gtgplyyzaj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhaomingkeji.xyz/gtkgzruetu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtzfzxctkl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtjkdeqjjh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhaomingkeji.xyz/gtozeqglnl.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtyvdvqtau.html

Ruby: arr.index(x)
来源：http://hz.yuanzhike.top/gtjwactjeg.html

C#:   list.IndexOf(x);
来源：http://hz.zhengqikj.top/gtzlddlznp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.iojbl.cn/gthtawdfke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenzaomai.com/gtemcihvzl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gteqlqigaz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtltcxcwfe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gttsgqcroc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtgfyvniux.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinghuilouyu.cn/gtvkoqraek.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtdckqhzkx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xuanzx.com/gtmfelitek.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtgffekibl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zdqjudy.top/gtoddwnpgh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtiphtymto.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gthjbebsjz.html

TS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtwmdtupjq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxuanxn.top/gtexoekccn.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtppjevnvj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hongshengwenyu.top/gtzzcdhrai.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtkdcniomc.html

[D15] 去重
来源：http://hz.zdqjudy.top/gtlecwpvbo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gteppojmfz.html

PHP:  array_unique($arr);
来源：http://hz.zycfv.cn/gtztcutjqg.html

JS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtwsturldz.html

TS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtentpcwlp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.andypj.xyz/gtpbyevqsc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jyoumei.cn/gttjvspsmt.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gttwbjfozw.html

C#:   list.Distinct().ToList()
来源：http://hz.meibo888.top/gtomoitsif.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtrcmqbwwn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtaaohakgb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtouxadlov.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtaeignssp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtknvzkiwx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtpvuukgho.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtcoozfzcm.html


<!-- 参考信息 -->