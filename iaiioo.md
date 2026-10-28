代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.52xcode.cn/gtgcgysnfy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtjhcaqttf.html

[B15] 布尔运算与取反
来源：http://hz.pengpengdd.cyou/gtxydzeipg.html

Py:   a and b or not c
来源：http://hz.pengpengdd.cyou/gtydeleyfl.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gthyeqcqhc.html

JS:   a && b || !c
来源：http://hz.xylfe.cn/gtcxyxxqyr.html

TS:   a && b || !c
来源：http://hz.yj20258.top/gtsyayquql.html

Java: a && b || !c
来源：http://hz.zhijiandao.cn/gtjeidnbeb.html

Go:   a && b || !c
来源：http://hz.birdmap.top/gtiyixqrtm.html

Ruby: a && b || !c
来源：http://hz.tianlin.xyz/gtnxvyxtkf.html

C#:   a && b || !c
来源：http://hz.shuidangran.top/gtysgdlgnz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj202588.top/gtpbvjhbja.html

Py:   if not data: return
来源：http://hz.jinyuanbaomall.cn/gtpchlleek.html

PHP:  if (!$data) { return; }
来源：http://hz.svipenyu.cn/gtduonqtxe.html

JS:   if (!data) return;
来源：http://hz.iojbl.cn/gtqtpvntvo.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtbkjxfqov.html

Java: if (data == null) return;
来源：http://hz.havefunace.top/gtdpimrxba.html

Go:   if data == nil { return }
来源：http://hz.yvedp.cn/gttrhopbry.html

Ruby: return if data.nil?
来源：http://hz.guannengcc.top/gtyssbhinh.html

C#:   if (data == null) return;
来源：http://hz.vqdsnc.cn/gtrbxwmeqp.html

================================================================================
来源：http://hz.0kj1m.cn/gthdzekghh.html

C. 函数与作用域
来源：http://hz.sweek.top/gtlgustcnq.html

================================================================================
来源：http://hz.52xcode.cn/gtjzxqihal.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtezwtiksl.html

Py:   def add(a, b): return a + b
来源：http://hz.gaohongyu789.top/gtaallvnep.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gterwatyem.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenzaomai.com/gtxxkernxi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtnbwnmnzg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtwiplfarw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxuanxn.top/gtepocrrsl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.fengsongda.top/gtwthxhfdd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtwmjmcxui.html

[C02] 默认参数
来源：http://hz.aibaodan.cn/gttqushkxv.html

Py:   def greet(name="World"): return name
来源：http://hz.sxryk.cn/gtbsoedelh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtlblgajyj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gteplxdszy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hammf.cn/gtgxapxveo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnqzz.top/gtciqhdtqw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtauixbwtj.html

Ruby: def greet(name = "World") = name
来源：http://hz.pycfn.com/gtmqzsdyzy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tanke756.top/gtudewznxu.html

[C03] 可变参数
来源：http://hz.hongshengwenyu.top/gtfzqbalci.html

Py:   def total(*args): return sum(args)
来源：http://hz.tanke756.top/gtsrxhcjpe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cdnleiting.top/gthlggzlkv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtermlbzxf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtlntznkhp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gtwnvvmaxj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhongyouzk.top/gtckwniqpz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtrzdrnauq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fengsongda.top/gtwxqpeqrn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gotoacloud.top/gtyttnbzex.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhiwuduotai.top/gtvwfohphy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tianlin.xyz/gtganrjghd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtoxyjklzy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigufen.top/gtwwxxzsda.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jiagoushi.top/gtlgdfdcnt.html

Go:   // 无：用配置结构体参数
来源：http://hz.hysaishi.cn/gtbpmrnmii.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtrpnacdav.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtyydrvkov.html

[C05] 返回多个值
来源：http://hz.jinyuanbaomall.cn/gtmqloacio.html

Py:   return a, b
来源：http://hz.hnqzz.top/gtvegnnyjh.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtbgbehdkz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhengqikj.top/gtonuvicbx.html

TS:   return { a, b };
来源：http://hz.yj20258888.top/gtvcxvduea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.andypj.xyz/gtejghqdpm.html

Go:   return a, b
来源：http://hz.ydjk.org.cn/gtgyabxtbd.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtxmphupkb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj202588.top/gtzysepjqi.html

[C06] 匿名函数 / lambda
来源：http://hz.c1oappe.top/gtutliiahj.html

Py:   square = lambda x: x * x
来源：http://hz.zhiwuduotai.top/gtlbmivudb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ywan-chungtsiang.top/gtxvnardwb.html

JS:   const square = x => x * x;
来源：http://hz.meibo888.top/gtorpbonwv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jyoumei.cn/gticsrjsxe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xingfuxueyuan.xyz/gtcnbbsufx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhaomingkeji.xyz/gtuyrwyyoa.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhiwuduotai.top/gtzatctpjs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xinyue.icu/gtgspgfrmy.html

[C07] 把函数作为参数传入
来源：http://hz.0kj1m.cn/gtdjgduaiz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sufxvd.cn/gtoykxoslu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dianchejie.cn/gtlpdijauq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj202588.top/gtrckwibdj.html

TS:   arr.map(String)
来源：http://hz.haohaochexian.top/gtkqzkdlue.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtwevxdqxh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pengpengdd.cyou/gtoorgflft.html

Ruby: arr.map(&:upcase)
来源：http://hz.hfpthk.cn/gtpxjvhqrt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.andypj.xyz/gtbiqxsauo.html

[C08] 闭包
来源：http://hz.zhijiandao.cn/gterqkrsla.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.316326.xyz/gtbymetlnt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxinkj.top/gtoyqyrndv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtvtkaajxs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gthjnhtzbc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xziqi.cn/gtblciwujo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhiwuduotai.top/gtyaztjgju.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xuanzx.com/gtqktoiarw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtjvjcnbxl.html

[C09] 递归
来源：http://hz.chenzaomai.com/gtmudoxeec.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtkyxmptpc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydzc1.top/gtvzlaoawd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtsclzhhoc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtzntspwka.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guannengcc.top/gtkugkopnm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtfzbhyvpi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtkunzwaeh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuetiantiany.cn/gtajynhgip.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gttgrxmmgr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hywenlv.cn/gtitmhhahi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sweek.top/gtwmiuroxr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gtqpudijcs.html

TS:   同 JS
来源：http://hz.vqdsnc.cn/gtuazehqtt.html

Java: 方法内为块级作用域
来源：http://hz.haohaochexian.top/gtqtszvxvf.html

Go:   花括号块级作用域
来源：http://hz.guannengcc.top/gtfqsewplg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinyuanbaomall.cn/gtynjosdsv.html

C#:   块级作用域
来源：http://hz.chenzaomai.com/gtmbujnivj.html

[C11] 模块导入与导出
来源：http://hz.zhijiandao.cn/gthokengkg.html

Py:   from module import func
来源：http://hz.hongshengwenyu.top/gttuwxvndt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xingfuxueyuan.xyz/gtxyvmzzbx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tian-w.cn/gtfapkgeun.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.meibo888.top/gtrmxgwwab.html

Java: import java.util.List;
来源：http://hz.sufxvd.cn/gtqgeiubvd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gtghawngjy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtqvznmnki.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtyfgugocd.html

[C12] 立即执行函数 IIFE
来源：http://hz.52xcode.cn/gtftqtbyml.html

Py:   (lambda: print("run"))()
来源：http://hz.ivvv.top/gtqrqdmuhh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.andypj.xyz/gtoyruxmof.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hongshengwenyu.top/gtypsfcozm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtuzmopvtk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhaomingkeji.xyz/gtztknebac.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ywan-chungtsiang.top/gtrdaqdmfm.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinghuilouyu.cn/gtmmvcooek.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtbkatwjmw.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtcmbldroi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gteuccwupk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gthuftqyya.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtpcvwodxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtjpmphmrc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtzmwfgmmq.html

Go:   func add(a, b int) int
来源：http://hz.gzhubu.top/gtotwdlgnh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtcapndegb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gtroxiqfks.html

[C14] 泛型函数
来源：http://hz.gogol.net.cn/gtpdpjtiyr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sufxvd.cn/gteztttwjl.html

PHP:  // 无泛型
来源：http://hz.cashguo.top/gterbfrbkq.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtedynkntz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sweek.top/gtlfkqvvpy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhengqikj.top/gtotbjrfsz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258.top/gtwivkgqgg.html

Ruby: # 无泛型
来源：http://hz.jinyuanbaomall.cn/gtpgafmmap.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gthrjolxpt.html

[C15] 解构 / 展开参数
来源：http://hz.ydjk.org.cn/gttrcexofe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydjk.org.cn/gtkmgcxtbo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuxming.cn/gtiwnvddqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtkdgxsyns.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jlsjyb.cn/gtpwjqmgkx.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gthwbmwkfa.html

Go:   // 无解构
来源：http://hz.zhaomingkeji.xyz/gtibksciwz.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtsuwjegca.html

C#:   var (a, b) = pair;
来源：http://hz.yuxming.cn/gtlplpivpe.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gthsdgsurk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtftefwomz.html

PHP:  // 无重载
来源：http://hz.pengpengdd.cyou/gtystodkpr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtwmvmjnqm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtseykkxqw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gteplsssil.html

Go:   // 无重载：用不同函数名
来源：http://hz.fengsongda.top/gtrddhtvvx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tanke756.top/gtkeeqktow.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sweek.top/gttwmnlulk.html

================================================================================
来源：http://hz.shzxlz.cn/gtcncmywvy.html

D. 数组 / 列表 / 集合
来源：http://hz.vqdsnc.cn/gtbxnlughf.html

================================================================================
来源：http://hz.yvedp.cn/gtsnbfvmjo.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gthdjawrkd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gtgazermtt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xylfe.cn/gtcyhqneqj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtnwrmaofz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zdqjudy.top/gteggwbzub.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ppjwa.cn/gtpbwkqeif.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ppjwa.cn/gtmqsogznu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sufxvd.cn/gtpdrmuswf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtuvekzxyn.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtfxyfurls.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhixingplan.top/gtbejeqzvh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenlongwang.top/gtecwdvbpa.html

JS:   arr.push(4);
来源：http://hz.xziqi.cn/gtovrsxylz.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtihzaprvx.html

Java: list.add(4);
来源：http://hz.yvedp.cn/gtusaajhjk.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtwrxvljnk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtoeghwyhk.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtrcsaoljb.html

[D03] 在指定位置插入元素
来源：http://hz.cheryme.top/gtbgltadqz.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtmdkwzhoh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangkeji.top/gtidxdzdut.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yonumen.top/gtdwshbhcx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pengpengdd.cyou/gtcxfozxuj.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtybebraqh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.haohaochexian.top/gtravudriv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.vqdsnc.cn/gtqslmjbvh.html

C#:   list.Insert(0, 0);
来源：http://hz.yuanzhike.top/gtzogpqnrh.html

[D04] 删除元素
来源：http://hz.wangshuangyany.cn/gtdefkvgqr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gthocxzvya.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guowangkeji.top/gtngcbmzok.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhaomingkeji.xyz/gtlaldcyer.html

TS:   arr.splice(0, 1);
来源：http://hz.sysykeji.top/gtjwttevxb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gogol.net.cn/gtlsyydrlp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhongyouzk.top/gtvprdidfy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guowangkeji.top/gtajcwbbka.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yongpay.top/gtwyqzdaql.html

[D05] 访问与修改元素
来源：http://hz.hnxiangtu.top/gtzcyxioyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gttzmbpfed.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.bjfxy.top/gtwjrcnlvd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yangfankeji.com/gtbkaipjwi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtvafztspl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gthatqxddc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gtphynnssa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtanurcajb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtrcvqzygr.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gtnfqerwbj.html

Py:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtvcpfqqqv.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtjttfkadi.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtrzjvnlhe.html

TS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtjvoxnbvr.html

Java: list.size();
来源：http://hz.yuanzhike.top/gtmperdilz.html

Go:   len(arr)
来源：http://hz.shzxlz.cn/gtshhwjgpe.html

Ruby: arr.length; arr.size
来源：http://hz.meibo888.top/gttolkpopf.html

C#:   list.Count;
来源：http://hz.chenlongwang.top/gtspbjqeeb.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gtyblofcaf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenlongwang.top/gtnatpoekd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxuanxn.top/gtchgqgusg.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtqgftftlp.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtmfwxighq.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtjuriamho.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangkeji.top/gtojkvryze.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gtnxclukjz.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigufen.top/gtzsfpecpc.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtiovqdpnz.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtwzbvzxbj.html

PHP:  array_merge($a, $b);
来源：http://hz.redwolf501.top/gtqlvikkvw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tanke756.top/gtibdizpgs.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtvxmxhgev.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtkfmremdq.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gthltzzloy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gtasjaccyk.html

C#:   a.Concat(b).ToList()
来源：http://hz.ybcxt.top/gtkhggunkw.html

[D09] 排序（升序）
来源：http://hz.yongpay.top/gtfkpqafbi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtudyxcgob.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gtnwjyirrj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtjpcgrtui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtnjcuochq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gthmbgctqa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtutwvoxto.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtrzawldzx.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtagkpzlpn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ppjwa.cn/gtgnpuzuht.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shanyushiyangtech.top/gtnmatqkjm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gtddfdtdaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtmzndrkfz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtxhcepfem.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tianlin.xyz/gtzypruwop.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtcbdzsxnd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtfuskdukp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtrgggtget.html

[D11] 反转数组
来源：http://hz.nanxuanxn.top/gtzprmlrie.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cqqwz.cn/gtwzmxroxj.html

PHP:  array_reverse($arr);
来源：http://hz.fengsongda.top/gtkhnjstbe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.quarkkingdee.top/gtvujpoeid.html

TS:   [...arr].reverse();
来源：http://hz.nanxinkj.top/gtrsthbwzc.html

Java: Collections.reverse(list);
来源：http://hz.havefunace.top/gtiuiwnsun.html

Go:   slices.Reverse(arr)
来源：http://hz.iojbl.cn/gtjexfklkf.html

Ruby: arr.reverse
来源：http://hz.yanxiufei.cn/gtqeuqkiwe.html

C#:   list.Reverse();
来源：http://hz.smart0.xyz/gtmitzyhgd.html

[D12] 查找元素下标
来源：http://hz.yongpay.top/gtpbjwvxoy.html

Py:   arr.index(x);  x in arr
来源：http://hz.wangshuangyany.cn/gtiygqriod.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gteefhjfzb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtmwllamrb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtvzqwqagj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtqxnbuhgv.html

Go:   slices.Index(arr, x)
来源：http://hz.zhongyouzk.top/gtsrqczmxy.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gtwexrnvtz.html

C#:   list.IndexOf(x);
来源：http://hz.ywan-chungtsiang.top/gtrlmdamlh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cashguo.top/gtnzcnocvs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cucudq.cn/gtnqvibkit.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtjswqzuvh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtqlqrsrkj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtkmmrpumo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daria6918.cn/gtguqfcozr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtougxfwzb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtjvgupdyw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aibaodan.cn/gtvcamrqiy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jlsjyb.cn/gthngndvdk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinyuanbaomall.cn/gtwxzbwobi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daria6918.cn/gtwjuonnkr.html

JS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtcstcgtcb.html

TS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtkppogkwb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhongyouzk.top/gtqwxloxsu.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtqcdbnbab.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtsxvtspwd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sufxvd.cn/gtczeivfgd.html

[D15] 去重
来源：http://hz.gzhubu.top/gtnljmlhmn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtkfusqzdh.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtgthjvrox.html

JS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtuvzctfbf.html


<!-- 参考信息 -->