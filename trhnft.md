代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtyspwouda.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nwbrower.top/gtwbzubwve.html

[B15] 布尔运算与取反
来源：http://hz.hysaishi.cn/gtkzninjzd.html

Py:   a and b or not c
来源：http://hz.zdqjudy.top/gtggrxkhqj.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gtbnsknhbr.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtaxwwtdcu.html

TS:   a && b || !c
来源：http://hz.zhixingplan.top/gtshnsyqhj.html

Java: a && b || !c
来源：http://hz.xuetiantiany.cn/gtuqjvcwdw.html

Go:   a && b || !c
来源：http://hz.aizwys.cn/gtxfexwzrl.html

Ruby: a && b || !c
来源：http://hz.ehwqpu.com/gtzhvjsaqn.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtxwjxnkim.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258.top/gtdzjntlin.html

Py:   if not data: return
来源：http://hz.jiagoushi.top/gtdgmfopdo.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtycktsuzt.html

JS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtlxzeifng.html

TS:   if (!data) return;
来源：http://hz.jinqigufen.top/gttbjekwle.html

Java: if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtzypewawh.html

Go:   if data == nil { return }
来源：http://hz.jinqigfzy.top/gtmioodwjj.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangkeji.top/gtitxurxxg.html

C#:   if (data == null) return;
来源：http://hz.316326.xyz/gtzanzvpdq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmguctkqb.html

C. 函数与作用域
来源：http://hz.tianlin.xyz/gtlmlsoasp.html

================================================================================
来源：http://hz.zhijiandao.cn/gtndophmjj.html

[C01] 定义函数
来源：http://hz.gzhubu.top/gthazobdyc.html

Py:   def add(a, b): return a + b
来源：http://hz.ydjk.org.cn/gtnckiwdpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtfwwekpkh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtseqhtwij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtfyhnwtxb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtzkndgnxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fengsongda.top/gtwufzolqw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zycfv.cn/gtswhjodvy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtwqdbxhaz.html

[C02] 默认参数
来源：http://hz.tianlin.xyz/gtsvoezxbd.html

Py:   def greet(name="World"): return name
来源：http://hz.wangshuangyany.cn/gthwjprwgw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.bjfxy.top/gthliuflhp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangkeji.top/gtlxuwobqi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gtdipwqkxe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.9152youxi.cn/gtupbjisec.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jianghu66.top/gthyhihscq.html

Ruby: def greet(name = "World") = name
来源：http://hz.daxiang520.top/gtqzfliptf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nwbrower.top/gthosrdtzo.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtkwjnvcqr.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhaomingkeji.xyz/gtclvbkrsn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangtech.top/gttyorafgw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.52xcode.cn/gtrozzcelm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtvzhuawrt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuxming.cn/gtzqufbgiz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.haohaochexian.top/gtyrtmilpc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hywenlv.cn/gteiithokx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pengpengdd.cyou/gtsiqluxgd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhijiandao.cn/gtjiltzibr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnqzz.top/gtvawbrwzd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hongshengwenyu.top/gtsldhhgir.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.birdmap.top/gtwfnmlbal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jqgufenzy.top/gtaqrscihq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gtzfqkglpi.html

Go:   // 无：用配置结构体参数
来源：http://hz.snrcjt.cn/gtmzmimmfo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtnftqqbvl.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtidvppond.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gtbufuolim.html

Py:   return a, b
来源：http://hz.tianlin.xyz/gtcrkgihpd.html

PHP:  return [$a, $b];
来源：http://hz.0kj1m.cn/gthnjtmfjw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtgyspwono.html

TS:   return { a, b };
来源：http://hz.kuanghao11.cn/gtpyzjvkiy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinghuilouyu.cn/gtulgwetjn.html

Go:   return a, b
来源：http://hz.yj202588.top/gtdqeqmwav.html

Ruby: return a, b
来源：http://hz.daria6918.cn/gtiufmrqmd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gttfekvtmf.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtvmoufial.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtjdhpvufr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gogol.net.cn/gtutkxdgyf.html

JS:   const square = x => x * x;
来源：http://hz.hongshengwenyu.top/gtgmirwmfg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtchcrmujb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtbviwrcqc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtnsyhofim.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigfzy.top/gtiewronnz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtpmqerxpw.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangtech.top/gtaqtfaydm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tianlin.xyz/gthjzsmgon.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gtgkznnuqs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gotoacloud.top/gtgeroedgn.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtfldzkmfx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guowangkeji.top/gtnqiyvqju.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgfzy.top/gtfagbrtau.html

Ruby: arr.map(&:upcase)
来源：http://hz.ybcxt.top/gtoomrlmjp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtkmdykfnl.html

[C08] 闭包
来源：http://hz.yuanzhike.top/gtkqnxbeed.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jlsjyb.cn/gtkvyqbryj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aibaodan.cn/gtrkhtynra.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gttihpvndp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtqrpwlcrb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gtdocyiikg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnxiangtu.top/gtfjpqehvc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hfpthk.cn/gtuaikfqlk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtntlrmzcs.html

[C09] 递归
来源：http://hz.chenjidiqi.icu/gtcqstuxfj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtsthtxhsz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gtjbafsgqy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtpswyewai.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtnasxsuir.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zycfv.cn/gtzagiijqb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtmyadiiss.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtyxzexugv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cheryme.top/gtoirvwnhc.html

[C10] 变量作用域
来源：http://hz.snrcjt.cn/gtyskwqctf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dianchejie.cn/gtmijazken.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtcjoncsnl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gtmkheagfe.html

TS:   同 JS
来源：http://hz.mhx1999.top/gtkpuarxtt.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtfzstexlv.html

Go:   花括号块级作用域
来源：http://hz.xylfe.cn/gtakbmabrp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtckmnycgx.html

C#:   块级作用域
来源：http://hz.chenjidiqi.icu/gtwncczcpg.html

[C11] 模块导入与导出
来源：http://hz.xziqi.cn/gtqenluutg.html

Py:   from module import func
来源：http://hz.ehwqpu.com/gtokukfrrz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tanke756.top/gthgczumrp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ehwqpu.com/gtiiqfktlr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydjk.org.cn/gtrlfixmke.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtwfdfwbvy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenjidiqi.icu/gtdrggaymc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pycfn.com/gtezlrcnjl.html

C#:   using System.Text;
来源：http://hz.svipenyu.cn/gtfkcjarib.html

[C12] 立即执行函数 IIFE
来源：http://hz.sxryk.cn/gtlgjtlydv.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gthruxjksa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hongshengwenyu.top/gtxqyojotu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtyquesdyo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtoishfxuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinghuilouyu.cn/gtuxpgicng.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.andypj.xyz/gtomfwfsto.html

Ruby: -> { puts "run" }.call
来源：http://hz.xingfuxueyuan.xyz/gtonafygbd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtziwcntbq.html

[C13] 类型声明 / 类型注解
来源：http://hz.tian-w.cn/gthppftmaq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgfzy.top/gtpjshgfol.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtpimnrkah.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hammf.cn/gtixuxbqwy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtjomnhsek.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtcustusxp.html

Go:   func add(a, b int) int
来源：http://hz.xingfuxueyuan.xyz/gtezflqxeg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtgmwqhozr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gtwjluerow.html

[C14] 泛型函数
来源：http://hz.tianlin.xyz/gtyoidnvyq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtcbgafiws.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtfmxwharh.html

JS:   // 无泛型
来源：http://hz.iojbl.cn/gtlctevkuq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dashuyun.cn/gtxcaaqzlb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.andypj.xyz/gtewxcxvjz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dianchejie.cn/gtkakbhtjl.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtofahawzm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gtwczhxucr.html

[C15] 解构 / 展开参数
来源：http://hz.shuidangran.top/gtsccltlgr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtscymmiaq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.quarkkingdee.top/gtcezdokqc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gtvdhreexz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhiwuduotai.top/gtihtnhqom.html

Java: // 无解构
来源：http://hz.snrcjt.cn/gtbboukbzw.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtlnksghys.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gttkxygjfz.html

C#:   var (a, b) = pair;
来源：http://hz.shangyingyoupin.top/gtemcapjlw.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtuwxvxkaa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtguzqinpo.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gthgutwhya.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtijgjdbdz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtmaawqyay.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.bjfxy.top/gtczzvnxim.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtyusisqyn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtviphakoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxuanxn.top/gtcpvvcbwj.html

================================================================================
来源：http://hz.wangdashe.top/gtnrmreuvj.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gtgqipsyze.html

================================================================================
来源：http://hz.yueranfly.top/gtumvwytpt.html

[D01] 创建数组 / 列表
来源：http://hz.quarkkingdee.top/gtgxbkurgm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sxryk.cn/gtrpyqjumr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gtabkpzljq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangkeji.top/gtnsfudoik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtdamrllbg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pycfn.com/gtkjpfgnne.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangdashe.top/gtefiiprhe.html

Ruby: arr = [1, 2, 3]
来源：http://hz.birdmap.top/gtlkxsvuoo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cucudq.cn/gtmtmfzhko.html

[D02] 追加元素到末尾
来源：http://hz.hammf.cn/gtulebxixz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xylfe.cn/gtvtahbqtj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtbeblvttt.html

JS:   arr.push(4);
来源：http://hz.hysaishi.cn/gtkhabbrqz.html

TS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtxamctndi.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtsdocsqqp.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtmqrtsegb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtleymioal.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtrzbftwvr.html

[D03] 在指定位置插入元素
来源：http://hz.jqgfzy.top/gteokqmzhq.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtlgzshuba.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nanxinkj.top/gtmdehjutk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zdqjudy.top/gtcyhlnszo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtficixwvu.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtqphlgfrc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigfzy.top/gtrkxbfcqm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigfzy.top/gteyvempzg.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtfmfqocbq.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtlgyxdbyd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gtebbagfby.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtbvjoovav.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gttrbqeqgg.html

TS:   arr.splice(0, 1);
来源：http://hz.tian-w.cn/gtffgggqap.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.c1oappe.top/gtqdhhawub.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangdashe.top/gtrgjkkhhg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gttgfiirvi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtpmorries.html

[D05] 访问与修改元素
来源：http://hz.ywan-chungtsiang.top/gtkutszcdg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtahannzei.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tianlin.xyz/gtvwsscoin.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtkxtewsii.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cqqwz.cn/gtebdfnjch.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.meibo888.top/gtqscnvhma.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gtybhlazpb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtwsudtjai.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtcqikxoju.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtxuvebnuk.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtwzwoylri.html

PHP:  count($arr);
来源：http://hz.52xcode.cn/gtdflerowq.html

JS:   arr.length
来源：http://hz.pycfn.com/gtbijltigy.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtvtglpsdv.html

Java: list.size();
来源：http://hz.dianchejie.cn/gtjrzbswxu.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtaudeqign.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtdelxiklb.html

C#:   list.Count;
来源：http://hz.yuanzhike.top/gtxiksbdei.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtciiequwt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenlongwang.top/gtpsueqcoz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yanxiufei.cn/gtqjdmxxdl.html

JS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtbkvmebkz.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtjauhnbpo.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtbnolsypm.html

Go:   arr[1:4]
来源：http://hz.jinqigfzy.top/gtrmmwmwhn.html

Ruby: arr[1, 3]
来源：http://hz.yj20258888.top/gtddzaxqso.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtnlyqbpdh.html

[D08] 合并两个数组
来源：http://hz.nanxinkj.top/gtysztlahi.html

Py:   a + b;  a.extend(b)
来源：http://hz.yonumen.top/gtlizpdpcx.html

PHP:  array_merge($a, $b);
来源：http://hz.meibo888.top/gtwhragywz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtarhcbswg.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtdvjvazwy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtcvxppgib.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtczqghstt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gtkrqjvgzb.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtytdusuhr.html

[D09] 排序（升序）
来源：http://hz.jqgufenzy.top/gtbsygziyw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtnkasstpl.html

PHP:  sort($arr);
来源：http://hz.hammf.cn/gturskfxhj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yvedp.cn/gtnhahtnay.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jqgufenzy.top/gtevujhszi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgufenzy.top/gtwvjjrpuj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtghrldwnm.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtczfiuafn.html

C#:   list.Sort();
来源：http://hz.aibaodan.cn/gttbdygvxm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtmkxcujvb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.316326.xyz/gtwvdzjquq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtutojadrg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gtumrynnwj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtowseydgj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtirqctvvp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tianlin.xyz/gtrbhevihf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gttzoqgszc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenlongwang.top/gtwulitezt.html

[D11] 反转数组
来源：http://hz.nwbrower.top/gtpecqvjvo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtgxiwparw.html

PHP:  array_reverse($arr);
来源：http://hz.tanke756.top/gtdkzydjzy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jianghu66.top/gtdthksycl.html

TS:   [...arr].reverse();
来源：http://hz.vqdsnc.cn/gtsvlpqrmb.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtootrybiv.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtuoecudcf.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gteyhfypgq.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtexzvnqkl.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtwsvefxlx.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtuhfgyeby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.bjfxy.top/gtirriwyje.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtnobgdcjw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtkvpjedjl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtzzewgthy.html

Go:   slices.Index(arr, x)
来源：http://hz.tian-w.cn/gtydrotnzk.html

Ruby: arr.index(x)
来源：http://hz.hfpthk.cn/gtecknlwdb.html

C#:   list.IndexOf(x);
来源：http://hz.shzxlz.cn/gtnsqelmjp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shanyushiyangkeji.top/gtwifuorha.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fzhhl.top/gtfpqwolun.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pengpengdd.cyou/gtewtczttf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtzncunigw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtfxivpqgu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtpkwarimk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtbwiikjml.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigfzy.top/gtkfvjxecj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hfpthk.cn/gtsircneif.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenjidiqi.icu/gtciaeffix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj202588.top/gtayrxpplt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtyzqsmuoe.html

JS:   arr.map(x => x * 2)
来源：http://hz.pengpengdd.cyou/gtimbmcshe.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtbtyeintp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhijiandao.cn/gtmfmjsfog.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtgitnyrkn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtbetammic.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gtjzcbfhrs.html

[D15] 去重
来源：http://hz.gzhubu.top/gtslscjrqw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.c1oappe.top/gteknyphpq.html

PHP:  array_unique($arr);
来源：http://hz.yj20258.top/gtfvqelcba.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtgfunvtmq.html


<!-- 参考信息 -->