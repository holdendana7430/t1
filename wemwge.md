代发 wailian999

Py:   if not data: return
来源：http://hz.zhongyouzk.top/gtkamdgexw.html

PHP:  if (!$data) { return; }
来源：http://hz.sxryk.cn/gtqqwthucb.html

JS:   if (!data) return;
来源：http://hz.316326.xyz/gteqrmqyjg.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtdtzqhiqd.html

Java: if (data == null) return;
来源：http://hz.9152youxi.cn/gtwofphihv.html

Go:   if data == nil { return }
来源：http://hz.xinyue.icu/gtefogvjxl.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gthnjzrytg.html

C#:   if (data == null) return;
来源：http://hz.fengsongda.top/gtyqoxgapi.html

================================================================================
来源：http://hz.cqqwz.cn/gtnnjoksjv.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gtnuosdfhp.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtppblicak.html

[C01] 定义函数
来源：http://hz.ydjk.org.cn/gtxtldzdit.html

Py:   def add(a, b): return a + b
来源：http://hz.yvedp.cn/gtjgvhuern.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtadepdopk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fengsongda.top/gtraaabkzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtivstxvii.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gthpkbjojv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtffwracql.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gtbcnfvxov.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtjdejiyzr.html

[C02] 默认参数
来源：http://hz.iojbl.cn/gttrudylti.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtvfmlgtwb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtrwudojkn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yueranfly.top/gtcaetedod.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jiagoushi.top/gtnrkczyxh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yvedp.cn/gtbcvoxzja.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtbyosnbuv.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnqzz.top/gtkqzbqbtf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.wangdashe.top/gtmvxizazu.html

[C03] 可变参数
来源：http://hz.316326.xyz/gtmyngmmef.html

Py:   def total(*args): return sum(args)
来源：http://hz.cqqwz.cn/gtckqvzowv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ydzc1.top/gtdsqrakfk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gthwabhfru.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtfttwywnu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jianghu66.top/gtnnjueqeq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuxming.cn/gtulyjatvl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj202588.top/gtdvjfxrbf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cdnleiting.top/gtalmyulxc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yongpay.top/gtrpfrqnba.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.smart0.xyz/gtmkjszpfw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtvtgzruon.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtkzybxqfm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hnqzz.top/gtecxxxaca.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.quarkkingdee.top/gtfwbudpao.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gthxndmavc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtzoxfcgzk.html

C#:   f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtsiwdyuov.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtfbkqkzvz.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtrpqcmpjm.html

PHP:  return [$a, $b];
来源：http://hz.yj202588.top/gtuhhlvxct.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtgtprsjzv.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtcrnbguvw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.kuanghao11.cn/gtrhndaoja.html

Go:   return a, b
来源：http://hz.ydzc1.top/gttasnnlls.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gthpooabmu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.snrcjt.cn/gtrpaeksaq.html

[C06] 匿名函数 / lambda
来源：http://hz.dianchejie.cn/gtvesntygb.html

Py:   square = lambda x: x * x
来源：http://hz.fzhhl.top/gtcaxmxeto.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tian-w.cn/gtrzrwvsqq.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtxdwftdib.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yvedp.cn/gtzkpmdifq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cheryme.top/gtvmecskwx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtzdjzcmjf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhixingplan.top/gtrgasttaj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhixingplan.top/gtggtwzuxj.html

[C07] 把函数作为参数传入
来源：http://hz.yanxiufei.cn/gtlawaegvj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtchccuyte.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gthuikgxuw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gterlrlmzh.html

TS:   arr.map(String)
来源：http://hz.sufxvd.cn/gtrzhmvuxr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gtdgwmrzcr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yangfankeji.com/gtnvizmlay.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtokuiiunb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gteilzjgfl.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gthsktqjfy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtbolvwlfc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydjk.org.cn/gtxrhittuf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtmshkhatm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtllkynvuu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xziqi.cn/gttcmvtqnx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhaomingkeji.xyz/gtwkpdmrfx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zdqjudy.top/gtgldjppgl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtzltsqwpp.html

[C09] 递归
来源：http://hz.hammf.cn/gtdkkytabx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhoulong.xyz/gtonzkfahe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gaohongyu789.top/gtyqteatpi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtmfzzkvuj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtlfjiuxzg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aizwys.cn/gtvlprruta.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinyuanbaomall.cn/gtjpeepdim.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aizwys.cn/gtggtqybyn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtctvvcotn.html

[C10] 变量作用域
来源：http://hz.nanxinkj.top/gteumzkrpt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ehwqpu.com/gthctebarp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.fengsongda.top/gtkssrrhas.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.andypj.xyz/gtvqpjlkhb.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtgqhsyofa.html

Java: 方法内为块级作用域
来源：http://hz.hfpthk.cn/gtrvfwybwu.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtxblyjwdp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangshuangyany.cn/gtyysrawkg.html

C#:   块级作用域
来源：http://hz.ydjk.org.cn/gtosrhpbnz.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gtsvsgdvft.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gthwsgwdld.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtmfrlgqhc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtjbjqxtxj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.smart0.xyz/gtrtmtblni.html

Java: import java.util.List;
来源：http://hz.pengpengdd.cyou/gtkhaziwoa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.316326.xyz/gtkvymqyaz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxinkj.top/gtioyujqxg.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gthidnsvwi.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtmypjnzvi.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gtlymmsfja.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guannengcc.top/gtwnumgbyc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtgyeseewd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gthtntsjbh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtotnkkagl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gtyjfqfcba.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenjidiqi.icu/gtyqcynccu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtytgqcllb.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtqxgueyji.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daxiang520.top/gtwysssooe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtsabygzew.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jiagoushi.top/gtaanfkiox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtqudultat.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtvvojejuf.html

Go:   func add(a, b int) int
来源：http://hz.0kj1m.cn/gtvwbmrpyy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnqzz.top/gtskarmpwm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xingfuxueyuan.xyz/gtxvutpmjg.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtjonkmbke.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.meibo888.top/gtzfxmgpvf.html

PHP:  // 无泛型
来源：http://hz.ppjwa.cn/gtlbnvazhd.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtqoslatvn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cqqwz.cn/gtuxuxtdsi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtfqlnjjjb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gtcmjeqqsx.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtberhlwdb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xziqi.cn/gtattgnxqv.html

[C15] 解构 / 展开参数
来源：http://hz.zhijiandao.cn/gtarscyjld.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.0kj1m.cn/gtltrknhfo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.mhx1999.top/gtdoykhvzi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtoyeqgbuw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtamxixkbg.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtcfgjoohq.html

Go:   // 无解构
来源：http://hz.zhiwuduotai.top/gtjuyzzlom.html

Ruby: a, b = pair
来源：http://hz.hongshengwenyu.top/gtxptjwdfl.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtctykoqhj.html

[C16] 函数 / 方法重载
来源：http://hz.jyoumei.cn/gtwxjwvdkv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtyojshuss.html

PHP:  // 无重载
来源：http://hz.yuanzhike.top/gthstayfqc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gtpjdqtsjo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtjachtoes.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtjaugwdaz.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gtbrxjyvcj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tianlin.xyz/gttzyjuzew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhijiandao.cn/gtixttsjqv.html

================================================================================
来源：http://hz.pycfn.com/gtkdqueviu.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtlcimmiuq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwdvfpybt.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtaavvfxge.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gtxyfbvcqk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtrldfdcgj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtemokatmi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnxiangtu.top/gtmxwdkkxp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sweek.top/gtmbimrgyk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxuanxn.top/gtqipucuak.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtnfrrgots.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtktqmncoe.html

[D02] 追加元素到末尾
来源：http://hz.daria6918.cn/gtwzebpgjv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yangfankeji.com/gthobxzkqy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hongshengwenyu.top/gtokohjzlm.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtymnijbkl.html

TS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtgninvugn.html

Java: list.add(4);
来源：http://hz.ybcxt.top/gtajyjeimd.html

Go:   arr = append(arr, 4)
来源：http://hz.sysykeji.top/gtbazshnya.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtzlnaqbkj.html

C#:   list.Add(4);
来源：http://hz.jinyuanbaomall.cn/gtsyabzcny.html

[D03] 在指定位置插入元素
来源：http://hz.ybcxt.top/gtysivkxux.html

Py:   arr.insert(0, 0)
来源：http://hz.c1oappe.top/gtcqeqmuzr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuxming.cn/gtfnihbbjq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hfpthk.cn/gtihuwqukw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtkajcdwkb.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gtpecuilrl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cqqwz.cn/gthxcgiaug.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtfhafafcm.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtnovudyid.html

[D04] 删除元素
来源：http://hz.0kj1m.cn/gtpcgwxgqe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cashguo.top/gtjzeazlhi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258888.top/gtxymrpzzl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.redwolf501.top/gtgmdpoorf.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gtjmxijamz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aibaodan.cn/gtnaubelpj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtkintsubk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj202588.top/gtenbsdmjr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dianchejie.cn/gthcuqsviq.html

[D05] 访问与修改元素
来源：http://hz.9152youxi.cn/gtlxshdyjh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtyvbhqxbb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtnpszwitl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gzhubu.top/gtexdjsawy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtsugyvqta.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtnltqhmyi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gthwpvtllz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtnbomwzfj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gzhubu.top/gtnmbyxlfg.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtsshunhjd.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gturuckizw.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtboyhiuua.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtglppecte.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gtxfdvoqtp.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtwnasxcyd.html

Go:   len(arr)
来源：http://hz.aibaodan.cn/gtggjwhxwb.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtmmtxypvs.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtduovtkpd.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gtlfgiunwu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.quarkkingdee.top/gtkmpkozio.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gtqnplivab.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gttmhszdhi.html

TS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gthnbdfydl.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gtmqilfzhu.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtmhcqhcwv.html

Ruby: arr[1, 3]
来源：http://hz.fengsongda.top/gtjvlumjuw.html

C#:   list.GetRange(1, 3);
来源：http://hz.redwolf501.top/gtakhszhwa.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtxxewutfg.html

Py:   a + b;  a.extend(b)
来源：http://hz.gaohongyu789.top/gtcwtnhyhx.html

PHP:  array_merge($a, $b);
来源：http://hz.xinyue.icu/gtutfadivr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtorvdhpkj.html

TS:   [...a, ...b];
来源：http://hz.9152youxi.cn/gtacucfzpq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtvbkcjuin.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtvphntqdc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtbrpjkdam.html

C#:   a.Concat(b).ToList()
来源：http://hz.shzxlz.cn/gtspqsyuve.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtesrhlrdm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtxighoqeb.html

PHP:  sort($arr);
来源：http://hz.tian-w.cn/gtxtbadbgq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xinyue.icu/gtwqmrquue.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtlvgujinz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gtsftsboam.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtlmqvxmpn.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtfdtvdmte.html

C#:   list.Sort();
来源：http://hz.aibaodan.cn/gteepefegd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hywenlv.cn/gthlqbsoiv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shzxlz.cn/gtquldvrua.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gtpwbnwcuw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtgxeptcgi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtaelawiay.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gtlatzeqgw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yangfankeji.com/gthjmrkiew.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gotoacloud.top/gtkoswgbro.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cheryme.top/gtpuebvtnf.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtoytnbert.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.c1oappe.top/gtebwcryhb.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtvxpeatnc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangshuangyany.cn/gtpwwnzcoj.html

TS:   [...arr].reverse();
来源：http://hz.gzhubu.top/gtojiziagd.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtvoplkxta.html

Go:   slices.Reverse(arr)
来源：http://hz.wangshuangyany.cn/gtmiqmhdnc.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangtech.top/gtyhnrcwcy.html

C#:   list.Reverse();
来源：http://hz.cdnleiting.top/gtxgpjvxjj.html

[D12] 查找元素下标
来源：http://hz.smart0.xyz/gtmzxfeplx.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtdnkuhdsa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtginpswxv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gttbzxaqnu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtvacjfpzx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtlmwvenvb.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtbaieqbgc.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtltxkgilj.html

C#:   list.IndexOf(x);
来源：http://hz.sweek.top/gtmljsiazt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtxebigjbr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gtewdospht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tanke756.top/gtyrqvhnot.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtqecbcsnl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtcysxneyw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cheryme.top/gtdqzudrqp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtlbacgwwa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cashguo.top/gtgzgtbxet.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtfzccavlt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gtxmhinnfv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sweek.top/gtixyqdbcx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yvedp.cn/gtfkzvckqg.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtinhndbkr.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtsmolzrww.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuanzx.com/gtsbnqcxyv.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gthvyvmphl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xinyue.icu/gtmuljpbar.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtchpxfrxg.html

[D15] 去重
来源：http://hz.shangyingyoupin.top/gtmvuzkjob.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gtuxpwjrwe.html

PHP:  array_unique($arr);
来源：http://hz.xuetiantiany.cn/gtgaojhaaw.html

JS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtifcegsck.html

TS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtvikwqils.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigfzy.top/gtnkpxohdy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hongshengwenyu.top/gtefgfmcqd.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtgmsmtzks.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtlbjikgqz.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtpeoadtyh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fengsongda.top/gtxvzbrxpi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.havefunace.top/gtbhysrhcy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtjfmtoeys.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtexfeuoap.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtoxyvdxfv.html

Go:   // 手写循环累加
来源：http://hz.chenjidiqi.icu/gtmxsybjyc.html


<!-- 参考信息 -->