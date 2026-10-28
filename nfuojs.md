代发 wailian999

Go:   a && b || !c
来源：http://hz.meibo888.top/gtuxkbqmeh.html

Ruby: a && b || !c
来源：http://hz.aibaodan.cn/gtbaebugel.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtjvtllmml.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xylfe.cn/gtynyvyedj.html

Py:   if not data: return
来源：http://hz.shzxlz.cn/gttdqpealw.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtmnbajpsl.html

JS:   if (!data) return;
来源：http://hz.pengpengdd.cyou/gtzmfduqna.html

TS:   if (!data) return;
来源：http://hz.yangfankeji.com/gttcpqtkhm.html

Java: if (data == null) return;
来源：http://hz.gogol.net.cn/gtaklfxezr.html

Go:   if data == nil { return }
来源：http://hz.meibo888.top/gtkqwdgwug.html

Ruby: return if data.nil?
来源：http://hz.sweek.top/gtahgvdaus.html

C#:   if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtitwtfcad.html

================================================================================
来源：http://hz.yueranfly.top/gteqigsaqd.html

C. 函数与作用域
来源：http://hz.cdnleiting.top/gthkyrnnlj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcrwsjmgx.html

[C01] 定义函数
来源：http://hz.ydzc1.top/gtvrrtbgct.html

Py:   def add(a, b): return a + b
来源：http://hz.chenlongwang.top/gtsaviqbbu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtkinnqlmd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtmnakelid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtxjxijseo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtqtyvslcu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.svipenyu.cn/gtawfvbaun.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtkoqzigwj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gthiaooqdc.html

[C02] 默认参数
来源：http://hz.quarkkingdee.top/gtznqrtjjx.html

Py:   def greet(name="World"): return name
来源：http://hz.cdnleiting.top/gtoedkkiwg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.9152youxi.cn/gtqlsdeqng.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangkeji.top/gtcdhoadaq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pycfn.com/gtlftxavog.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtobvcycrk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtzhnzcyan.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gthpxdndgw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.birdmap.top/gtjaikxxnz.html

[C03] 可变参数
来源：http://hz.tian-w.cn/gtwmfbzqna.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtxtwgnwsj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gtwuggxysp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtqguxltco.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258888.top/gtxozcxffb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gzhubu.top/gttcohcrrw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ehwqpu.com/gtmzjrtgfp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtievmwgla.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jlsjyb.cn/gtetchhseo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj202588.top/gtyhrgxnik.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tianlin.xyz/gtpxfyhoeb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.quarkkingdee.top/gtcntfnnmq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fzhhl.top/gthqvadazf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinghuilouyu.cn/gtnoccyxdi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gtsdhnzejo.html

Go:   // 无：用配置结构体参数
来源：http://hz.guowangkeji.top/gtbipxsuct.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtchfmkcdc.html

C#:   f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtdroqhgbm.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtqydpmrvu.html

Py:   return a, b
来源：http://hz.xziqi.cn/gtpvcnrgfh.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtrdfbohuy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtariqfdrm.html

TS:   return { a, b };
来源：http://hz.zhijiandao.cn/gtkkaptslj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jianghu66.top/gtfzqxtwom.html

Go:   return a, b
来源：http://hz.hnqzz.top/gtkmjppqua.html

Ruby: return a, b
来源：http://hz.hnqzz.top/gtcmcwexlx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.316326.xyz/gtvxhccwgu.html

[C06] 匿名函数 / lambda
来源：http://hz.0kj1m.cn/gtrsjhgjag.html

Py:   square = lambda x: x * x
来源：http://hz.shangyingyoupin.top/gtvsntillb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.0kj1m.cn/gthgvlslpz.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtyhbusgjs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.bjfxy.top/gthxnqhiwv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shuidangran.top/gtkjcvvjtz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sxryk.cn/gtlxntpgil.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigufen.top/gttjzrnmyu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhoulong.xyz/gtlepqzkhc.html

[C07] 把函数作为参数传入
来源：http://hz.zhongyouzk.top/gtzeksowqz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sysykeji.top/gtdzbtkbdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangdashe.top/gtqspwmdnx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gteyfkarih.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtcnfxqcxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.quarkkingdee.top/gtwitdnmos.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gttyxvufms.html

Ruby: arr.map(&:upcase)
来源：http://hz.dianchejie.cn/gtanyvhxfw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gttsnagkfl.html

[C08] 闭包
来源：http://hz.hywenlv.cn/gtyhxjrjgl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtbqbgbcko.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtouihisxa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtgdxotbfr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtmrfhhcwm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jyoumei.cn/gtjzspqvgj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sweek.top/gtwkvrixcz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.haohaochexian.top/gtbscoswzd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtyebobmmx.html

[C09] 递归
来源：http://hz.jianghu66.top/gtlmligfvk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtlvrgxgvq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gtmqsczmin.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtrsrgpazx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtmmnwagab.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtoyauuvns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fengsongda.top/gtgbdkuthk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258.top/gtdqnshddk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.haohaochexian.top/gtoruevaiw.html

[C10] 变量作用域
来源：http://hz.cucudq.cn/gtkulrxiyy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtotaefujw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtpekpasap.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtjpkxefjr.html

TS:   同 JS
来源：http://hz.redwolf501.top/gtnwyiqioy.html

Java: 方法内为块级作用域
来源：http://hz.sufxvd.cn/gthdshfyce.html

Go:   花括号块级作用域
来源：http://hz.tianlin.xyz/gtbdlunafb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.haohaochexian.top/gtpxgbzhny.html

C#:   块级作用域
来源：http://hz.yj202588.top/gtrmcmtuat.html

[C11] 模块导入与导出
来源：http://hz.shzxlz.cn/gtofvgnsxl.html

Py:   from module import func
来源：http://hz.hnxiangtu.top/gtyzkuyqdb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guannengcc.top/gttyzjkpoa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gtqvzclzhy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtzgxllsgk.html

Java: import java.util.List;
来源：http://hz.aizwys.cn/gtuuucbrkq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hammf.cn/gtiwpxhkqf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtkavvdakr.html

C#:   using System.Text;
来源：http://hz.haohaochexian.top/gtdulhpqlr.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhijiandao.cn/gtpgkpmovg.html

Py:   (lambda: print("run"))()
来源：http://hz.hywenlv.cn/gtyonwpcud.html

PHP:  (function () { echo "run"; })();
来源：http://hz.birdmap.top/gtojuzvfwa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenzaomai.com/gtozxupriu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtymuhaeib.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtfuuabfaf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ppjwa.cn/gtikevzuqk.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtmjridtni.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.0kj1m.cn/gtmvkmlzxi.html

[C13] 类型声明 / 类型注解
来源：http://hz.xziqi.cn/gtmovkmsjq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.vqdsnc.cn/gtizjekpvc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtmaxrzdmx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yanxiufei.cn/gtnmrvcfbm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtnzslgklb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtgdvkucps.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gtbzszdpsu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtwlutliqs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtmuagqqfc.html

[C14] 泛型函数
来源：http://hz.chenlongwang.top/gtvjbsqgfe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtpfbxtsbt.html

PHP:  // 无泛型
来源：http://hz.cucudq.cn/gtodwwxaew.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtplacfgrp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xziqi.cn/gtppylxqyf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zdqjudy.top/gtrwygviay.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtnnajjxqj.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtvhioqdxa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenjidiqi.icu/gtvoqwiwqu.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtraatcnsg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtodwcgozq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.meibo888.top/gtbyeczoyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtjzjfudym.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aizwys.cn/gtomztejub.html

Java: // 无解构
来源：http://hz.cdnleiting.top/gtgtqigmuh.html

Go:   // 无解构
来源：http://hz.ydzc1.top/gtvradmtkr.html

Ruby: a, b = pair
来源：http://hz.9152youxi.cn/gtcvmzsroh.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtmkdftefm.html

[C16] 函数 / 方法重载
来源：http://hz.xinyue.icu/gtgsslmxxv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtcsugyzkw.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtcabxmvrm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.meibo888.top/gtjbergbxm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtxislhzod.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.birdmap.top/gtviginnmq.html

Go:   // 无重载：用不同函数名
来源：http://hz.gzhubu.top/gtxzqcjvvf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ivvv.top/gtiiybhtsf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtzidyqyhc.html

================================================================================
来源：http://hz.yangfankeji.com/gtdapzidsh.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtsimhbjwx.html

================================================================================
来源：http://hz.meibo888.top/gtyaesnjzd.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtfgudipzt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yvedp.cn/gtrwpqkepk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtfnjltnuw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ppjwa.cn/gtuwjjlfiy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gtagzdkkgv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgufenzy.top/gtwnnpqvio.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtbwegqmmu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.mhx1999.top/gtgelltsrx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.mhx1999.top/gtvhjhhchb.html

[D02] 追加元素到末尾
来源：http://hz.kuanghao11.cn/gtjaerhdhi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gttkhvwnos.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.316326.xyz/gtxcfrmpsn.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtvlemrshg.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtifarqgrw.html

Java: list.add(4);
来源：http://hz.ywan-chungtsiang.top/gtoerxdnwu.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtkiylytng.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtghwskafj.html

C#:   list.Add(4);
来源：http://hz.tanke756.top/gtkikvmolh.html

[D03] 在指定位置插入元素
来源：http://hz.zhijiandao.cn/gtqbmnrsul.html

Py:   arr.insert(0, 0)
来源：http://hz.svipenyu.cn/gtszwqllsm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tianlin.xyz/gtnegekzjz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yanxiufei.cn/gtqadgaknn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtusqswhzq.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gtpphticcs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.iojbl.cn/gtntgnfmjx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258.top/gtbdrxiemv.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtsswtnkdu.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtzcucpjxa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.iojbl.cn/gtdukgrbbm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtjcxcgitr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtwqxehkwt.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtpdxkzouu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gttttvkfnw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxuanxn.top/gtjqmjwczq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtkqbomgxa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxinkj.top/gthwfzldzd.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtopqqexgp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtouzjdwjk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gtpvfnowfo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtkvruymlx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnqzz.top/gtwjdaimwr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydzc1.top/gtlptguxtd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gtqmevrpyk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtfzbnnpza.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dashuyun.cn/gtiwlipswq.html

[D06] 数组长度
来源：http://hz.yvedp.cn/gtskpiesjn.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gtnpkqkvog.html

PHP:  count($arr);
来源：http://hz.xingfuxueyuan.xyz/gttngpzkaz.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtrchzzgjk.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtipdahaie.html

Java: list.size();
来源：http://hz.yueranfly.top/gteudqwidx.html

Go:   len(arr)
来源：http://hz.ehwqpu.com/gtiunkzpxd.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtenxepcmu.html

C#:   list.Count;
来源：http://hz.yuanzhike.top/gtndambpmi.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gthyhqbssz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuxming.cn/gtrrgezcvo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ybcxt.top/gtbyqdwdxr.html

JS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtaxokuvzq.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtoilrbcjg.html

Java: list.subList(1, 4);
来源：http://hz.redwolf501.top/gtketeptpl.html

Go:   arr[1:4]
来源：http://hz.c1oappe.top/gtajythefm.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtxpmrdtgz.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtjrsivweb.html

[D08] 合并两个数组
来源：http://hz.shzxlz.cn/gtvqefxrzy.html

Py:   a + b;  a.extend(b)
来源：http://hz.svipenyu.cn/gtdlscsclf.html

PHP:  array_merge($a, $b);
来源：http://hz.yangfankeji.com/gtquxeilna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtqqjmopng.html

TS:   [...a, ...b];
来源：http://hz.hnqzz.top/gtcwzywlol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sxryk.cn/gtojrzyxgp.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtxwrmibet.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gteubjmvxx.html

C#:   a.Concat(b).ToList()
来源：http://hz.andypj.xyz/gtmkgcvora.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtroggegjn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtioxtnafx.html

PHP:  sort($arr);
来源：http://hz.svipenyu.cn/gtuvtpfzls.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhoulong.xyz/gtmpsvgtrg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtwmdaleox.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.316326.xyz/gtbyqlcmax.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtccznezlu.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtwvbkigwu.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtoczfujoe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jianghu66.top/gtfruyqhoc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtpgqkmvvz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtqodkfioz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtfwvizmhk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gtdivofrik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hfpthk.cn/gtmtyydudb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yangfankeji.com/gtoljkdfhq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtpccyhggz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yanxiufei.cn/gtgocjetvl.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtmmqhbmkj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.meibo888.top/gtpfrxdzsp.html

PHP:  array_reverse($arr);
来源：http://hz.tianlin.xyz/gtiwzvgxlo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cucudq.cn/gtveppzjhu.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtwpckvisv.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtsmvxqrif.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258888.top/gtewbhrvbm.html

Ruby: arr.reverse
来源：http://hz.jlsjyb.cn/gthxopteup.html

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtxdktknro.html

[D12] 查找元素下标
来源：http://hz.shangyingyoupin.top/gtsmovkhjm.html

Py:   arr.index(x);  x in arr
来源：http://hz.iojbl.cn/gtwcsoqsqo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.316326.xyz/gtdedgvasu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtksxbvzrr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtmcfwteol.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pycfn.com/gthztdbbho.html

Go:   slices.Index(arr, x)
来源：http://hz.cucudq.cn/gtlslmmqne.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gttfcfgiht.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gtolllycuy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.0kj1m.cn/gteizrmtmz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.mhx1999.top/gtgilgahob.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shuidangran.top/gtjywmkrnd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtecwmlfyz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtxnrlumck.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtqrguieia.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhijiandao.cn/gtqrgdzwrc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtqsoulthj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.redwolf501.top/gtlyarofbh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtvtxewftl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtpxwtjpqr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuxming.cn/gtaonzrjcy.html

JS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtbequotgu.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtzihepieu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtawbvrcxo.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gttvizdnck.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj202588.top/gtjcatwbmh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenzaomai.com/gtxisowgju.html

[D15] 去重
来源：http://hz.jinghuilouyu.cn/gtkpxmvjtr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xinyue.icu/gtkbxrlvef.html

PHP:  array_unique($arr);
来源：http://hz.sweek.top/gtywlvtugz.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtpgjppoeq.html

TS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtiimczrfk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ywan-chungtsiang.top/gtkbfeboxj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jlsjyb.cn/gttibfalma.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtsraefnmd.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gtxcuzmdge.html

[D16] 求和与平均值
来源：http://hz.cdnleiting.top/gtlwprpxgb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.andypj.xyz/gtdldifimb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtqcojyjjy.html


<!-- 参考信息 -->