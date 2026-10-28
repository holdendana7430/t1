代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gtfozoiuio.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aibaodan.cn/gtnjfhgggh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gteoccemua.html

Ruby: def greet(name = "World") = name
来源：http://hz.snrcjt.cn/gtstncsepa.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtxigdtfhn.html

[C03] 可变参数
来源：http://hz.316326.xyz/gtigbpxcyf.html

Py:   def total(*args): return sum(args)
来源：http://hz.smart0.xyz/gtxgeinckl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gtsqbiuwuz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gtcuahqkgu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtgojpalgn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sweek.top/gtxibfokkn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.redwolf501.top/gtttkknrlj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtnffqkggf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jianghu66.top/gtlruhnixv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jlsjyb.cn/gtiyrpojau.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhixingplan.top/gtyzxehpun.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gtkojmnjbf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yonumen.top/gtqilhhmsy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tanke756.top/gtcldbdwuo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.redwolf501.top/gtxuyqxdka.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydjk.org.cn/gtezmexmpi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtjbjuohrb.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtgkzhirim.html

[C05] 返回多个值
来源：http://hz.jiagoushi.top/gtsmhedblh.html

Py:   return a, b
来源：http://hz.yongpay.top/gtelzdzxzg.html

PHP:  return [$a, $b];
来源：http://hz.ydjk.org.cn/gtrdendzvu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guowangkeji.top/gtrxfoeybl.html

TS:   return { a, b };
来源：http://hz.hywenlv.cn/gtsnemndyh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gteqzckboq.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gtlyzphuzm.html

Ruby: return a, b
来源：http://hz.yangfankeji.com/gtxbwwjjdz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gttjdkrzxz.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtsyyzgxfq.html

Py:   square = lambda x: x * x
来源：http://hz.snrcjt.cn/gttsgttnwy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guowangkeji.top/gtzmraatjd.html

JS:   const square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtjqnqjxpr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.wangdashe.top/gtgtycewbg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shangyingyoupin.top/gtuuysgszq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yvedp.cn/gtusnskkrc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtvthmblyc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtwszfxbcv.html

[C07] 把函数作为参数传入
来源：http://hz.hongshengwenyu.top/gtcztkfwkp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.mhx1999.top/gtcdfxhpxf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.c1oappe.top/gtwiubamcy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sufxvd.cn/gtkqkwslzg.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtparjxtuq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhongyouzk.top/gtfpkadbxl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.smart0.xyz/gtghqagxlf.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtbymvvbcf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shzxlz.cn/gthfekkgos.html

[C08] 闭包
来源：http://hz.cucudq.cn/gtamvxwbhu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fengsongda.top/gthmpfpatt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.wangdashe.top/gthjxluddm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangtech.top/gtlrxkuwaw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtwsqydakj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hammf.cn/gtdxbwqqta.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sysykeji.top/gtobbcaikm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.0kj1m.cn/gtxuklgqia.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtsxjrdsow.html

[C09] 递归
来源：http://hz.sufxvd.cn/gtiskyiixz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgfzy.top/gtdhrxqljj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yueranfly.top/gteyoeabkz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtgilakgbr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtljjchsqp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guannengcc.top/gtfclwsxau.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gaohongyu789.top/gtgdtyzxjm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fzhhl.top/gtevfiwepj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhijiandao.cn/gtvlbdqaor.html

[C10] 变量作用域
来源：http://hz.yvedp.cn/gtfqllirmn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtwpnmntlq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhongyouzk.top/gtzbioabde.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tanke756.top/gtitxqihzb.html

TS:   同 JS
来源：http://hz.yj20258.top/gthahmrtug.html

Java: 方法内为块级作用域
来源：http://hz.tanke756.top/gtwkmhpaww.html

Go:   花括号块级作用域
来源：http://hz.gaohongyu789.top/gtqrwqwyiw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtytsylcpp.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtittiipou.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtitykljmt.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtesinwkqx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtngvtibns.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cheryme.top/gthyhofekp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtpsrukjlr.html

Java: import java.util.List;
来源：http://hz.gzhubu.top/gtyfpnpxur.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.bjfxy.top/gtobcgefji.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtagwrenvi.html

C#:   using System.Text;
来源：http://hz.aizwys.cn/gtqbuukgjm.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinghuilouyu.cn/gtiappkmxq.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gtukbkldyw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xylfe.cn/gtiyzilofd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtrmgtxhfg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtfuzxffqp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtzwoyjxbl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yanxiufei.cn/gtrodgzxlp.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnxiangtu.top/gtltljxcss.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtqqueuinx.html

[C13] 类型声明 / 类型注解
来源：http://hz.xingfuxueyuan.xyz/gtjxmpqqat.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtvqkmudzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gthnkbaksk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtdtjzpwnz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtjnyvftdr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtecxxnqpf.html

Go:   func add(a, b int) int
来源：http://hz.daxiang520.top/gtizwapowq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtmufdmivu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gzhubu.top/gtfukmkmdf.html

[C14] 泛型函数
来源：http://hz.xylfe.cn/gtlacpcszo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuetiantiany.cn/gtmmfcxdqj.html

PHP:  // 无泛型
来源：http://hz.ybcxt.top/gtrgbffcuo.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gttrwfxqhx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenzaomai.com/gthdbuteid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.iojbl.cn/gtzhxmtpcc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cheryme.top/gtcodnyucl.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtazfbxguo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gthuybhodx.html

[C15] 解构 / 展开参数
来源：http://hz.fzhhl.top/gtguzkgtin.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yvedp.cn/gtkwfclejc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtpyspzkmy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtjupkrnoi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jlsjyb.cn/gtdrrjicbw.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtijkgnqkc.html

Go:   // 无解构
来源：http://hz.sufxvd.cn/gtmtsjtdcy.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gtdcwcwptr.html

C#:   var (a, b) = pair;
来源：http://hz.nanxuanxn.top/gtuvrzccfi.html

[C16] 函数 / 方法重载
来源：http://hz.yj20258.top/gtonajqfrh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sysykeji.top/gtghxxjwyz.html

PHP:  // 无重载
来源：http://hz.yuanzhike.top/gtebqzquyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gtlefwglta.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.snrcjt.cn/gtwcxmwxjz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtjdabercp.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtnmcnysyp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xingfuxueyuan.xyz/gtjyevijtj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pycfn.com/gtunfzfvxe.html

================================================================================
来源：http://hz.xylfe.cn/gtwrgywfvj.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangkeji.top/gtehgfibjk.html

================================================================================
来源：http://hz.shzxlz.cn/gtvlyuyatb.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtilioopry.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.pengpengdd.cyou/gtmuxlslgk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtsmgzegrr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinghuilouyu.cn/gtcpxuohtq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtruyndojm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.snrcjt.cn/gtfzrpqnfh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhongyouzk.top/gtaymfcmtp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xingfuxueyuan.xyz/gtilfsshyz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtrwpnslvh.html

[D02] 追加元素到末尾
来源：http://hz.xingfuxueyuan.xyz/gtzskydvlv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guannengcc.top/gtbjvqglzr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtmppfjywn.html

JS:   arr.push(4);
来源：http://hz.316326.xyz/gtmmenffii.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtdxowomok.html

Java: list.add(4);
来源：http://hz.wangshuangyany.cn/gtyseilhvt.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtjfntdelc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxinkj.top/gtunupkxrn.html

C#:   list.Add(4);
来源：http://hz.gzhubu.top/gttanpynwb.html

[D03] 在指定位置插入元素
来源：http://hz.hnxiangtu.top/gtrchshmit.html

Py:   arr.insert(0, 0)
来源：http://hz.yanxiufei.cn/gtseezgtjh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cheryme.top/gttsvzkrew.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.52xcode.cn/gtnevksjnx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtcwwbqpya.html

Java: list.add(0, 0);
来源：http://hz.jlsjyb.cn/gtsukfoyyh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258.top/gtjxoxfcyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ivvv.top/gtzyokgxdl.html

C#:   list.Insert(0, 0);
来源：http://hz.yongpay.top/gtskxdvtij.html

[D04] 删除元素
来源：http://hz.jiagoushi.top/gtvqvutekw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtlxlmcnxi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhongyouzk.top/gtqavqbqqq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yongpay.top/gtidlvuwdc.html

TS:   arr.splice(0, 1);
来源：http://hz.xingfuxueyuan.xyz/gtqsigwbwq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shanyushiyangtech.top/gtqkbzrxis.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtwhwrjcxj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxuanxn.top/gtfjqclpzw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tanke756.top/gtoiuakhxt.html

[D05] 访问与修改元素
来源：http://hz.9152youxi.cn/gttcnrhyjv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtjxikprvn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtmdwklvhh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zycfv.cn/gtxjzllyrd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtvsuookez.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cqqwz.cn/gtyjxlnynv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gttiffjowh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yonumen.top/gtmgrmatle.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtrolfdlwb.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtgpjwnhpp.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtntfqdrnf.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtpenjbbaq.html

JS:   arr.length
来源：http://hz.zhengqikj.top/gttxmdyser.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtizrgihaj.html

Java: list.size();
来源：http://hz.chenjidiqi.icu/gtsgstudtx.html

Go:   len(arr)
来源：http://hz.hongshengwenyu.top/gtmtbbrmds.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtjbmenfya.html

C#:   list.Count;
来源：http://hz.zhaomingkeji.xyz/gtfortqwos.html

[D07] 切片 / 取子数组
来源：http://hz.mhx1999.top/gtrzonmxeh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.kuanghao11.cn/gtwxypxhuf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.redwolf501.top/gtevjdnyrd.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtcxbdeqgc.html

TS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtexrmzhiq.html

Java: list.subList(1, 4);
来源：http://hz.chenjidiqi.icu/gtueluezrc.html

Go:   arr[1:4]
来源：http://hz.vqdsnc.cn/gtlnbjqrzu.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtmulxwfzc.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gtitnsnjog.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gtwrulydkq.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtyyblloyy.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtyrijvnye.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtyhjdppyj.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtfcrtwkax.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gtultxfrix.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtmfzacelc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yvedp.cn/gtruxhxwnb.html

C#:   a.Concat(b).ToList()
来源：http://hz.jiagoushi.top/gtfqqhjydf.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtoucmwace.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gthxfasuax.html

PHP:  sort($arr);
来源：http://hz.iojbl.cn/gtppyloczf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhaomingkeji.xyz/gtwqsxobzt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtuyodpltp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.iojbl.cn/gtuapxqeuw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtaouwwkzt.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtitpccfbx.html

C#:   list.Sort();
来源：http://hz.pycfn.com/gtzwcayicf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dianchejie.cn/gtifokehit.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnxiangtu.top/gtmjxrljxe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtpmnxeujw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtfnfyzqxx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtxzfgyyxf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gterowdqpl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258.top/gtojoxzwzu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtgstoovui.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydjk.org.cn/gtaiirnrvd.html

[D11] 反转数组
来源：http://hz.meibo888.top/gtmumqhzzd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtwhvefglm.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gthgornnzh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtctqdbdzn.html

TS:   [...arr].reverse();
来源：http://hz.quarkkingdee.top/gtqcjhuzll.html

Java: Collections.reverse(list);
来源：http://hz.xinyue.icu/gtoaceuumw.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258888.top/gtjhobjtiu.html

Ruby: arr.reverse
来源：http://hz.yj202588.top/gtotjyvfvf.html

C#:   list.Reverse();
来源：http://hz.andypj.xyz/gtfzxujlnr.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtcajibtey.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhijiandao.cn/gtjwcldfhb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gtubvxoszo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gthxbrsums.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtkzcnslzv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.havefunace.top/gtglwzwfpw.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtoglpriff.html

Ruby: arr.index(x)
来源：http://hz.xziqi.cn/gtrirldxfv.html

C#:   list.IndexOf(x);
来源：http://hz.snrcjt.cn/gtkmrzyoqx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtqbqdlllx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jiagoushi.top/gtqpnevhxc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtmuhvqjuh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtgktdqowh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtammpwlte.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gtkzgvctkq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aibaodan.cn/gtbitxfnso.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guannengcc.top/gtvsczpmdm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ehwqpu.com/gtmajmnwny.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pengpengdd.cyou/gtkikesxjt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gtfgthydjo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtmjbznoki.html

JS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtehjwtrsa.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtiogigssm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtxfcwlzjr.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtcpgvzuxc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.redwolf501.top/gtipqzkazp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtyivufkwm.html

[D15] 去重
来源：http://hz.xingfuxueyuan.xyz/gtmkxugjin.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtkphnkjbv.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gtqxxutddi.html

JS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtnpshzwuy.html

TS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gttyvxnthr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shzxlz.cn/gtvqpagvpm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cdnleiting.top/gtrnwrewwh.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtvxbjtwse.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtpjdeoenq.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gtnimhshhb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gogol.net.cn/gtwowomaac.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.c1oappe.top/gtnzjbjhhp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gthykchsjk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtmwihvopq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtqwwlfoly.html

Go:   // 手写循环累加
来源：http://hz.zdqjudy.top/gtrslswjcu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jyoumei.cn/gtjzyiegxn.html

C#:   list.Sum();  list.Average()
来源：http://hz.shzxlz.cn/gtsizcxkhu.html

[D17] 最大值与最小值
来源：http://hz.snrcjt.cn/gtbswszram.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtqfxievec.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtmbzsvkgp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangshuangyany.cn/gtmmxwnatu.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtxzgxryhh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtuzziaejb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gthnfoksos.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtfxzpxtvf.html

C#:   list.Max();  list.Min()
来源：http://hz.tanke756.top/gtwphdlpmk.html

[D18] 扁平化嵌套数组
来源：http://hz.jiagoushi.top/gtkpmepvth.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gthmiwctkn.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtchqetkym.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gttijoenyy.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtsypqnzmz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gtzngtngef.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtdipjukvn.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtzorhzzhs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtcxjeqrxk.html

[D19] 按字段分组
来源：http://hz.hysaishi.cn/gtyxtgvavh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hfpthk.cn/gtszeuyhzh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhaomingkeji.xyz/gtbizraksh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fzhhl.top/gtwphfvwuh.html


<!-- 参考信息 -->