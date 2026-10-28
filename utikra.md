代发 wailian999

Java: if (data == null) return;
来源：http://hz.ybcxt.top/gtdzjduuuj.html

Go:   if data == nil { return }
来源：http://hz.zhijiandao.cn/gtotqutcda.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtmuyznays.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gtwzwnmdby.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdvrjsqgn.html

C. 函数与作用域
来源：http://hz.shanyushiyangtech.top/gtoazgkeds.html

================================================================================
来源：http://hz.birdmap.top/gtmrfcoqjj.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtmyicrbcz.html

Py:   def add(a, b): return a + b
来源：http://hz.birdmap.top/gthlvonzud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtaktgjjgo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtlccuxbai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gttnfsrabe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtgqwwdffq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shzxlz.cn/gtyhtzvjjv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinghuilouyu.cn/gtwahfqtyy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtdvemvfkk.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtxsbzgwon.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtqnfcdjzs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.smart0.xyz/gtsvybkqqf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangdashe.top/gtkkijllqg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.316326.xyz/gtlebeaqry.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gtyhkqxgsw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jyoumei.cn/gtggxbsphy.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtwdhyjljh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gogol.net.cn/gthikdfznm.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gtgknkkyyt.html

Py:   def total(*args): return sum(args)
来源：http://hz.feifeiyinyue.top/gtvzjqpdyt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aibaodan.cn/gtyldxjndp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtmksachcj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtkqwxanwe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.bjfxy.top/gtknqzkdni.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtxjxbhykw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cucudq.cn/gtglyitimy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhaomingkeji.xyz/gtlaidcooz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.0kj1m.cn/gtpbpzqqmk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.quarkkingdee.top/gteaopumlv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhengqikj.top/gttsgwjrye.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtryyxgdlm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangtech.top/gtsbkjvuxe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gtkiertuhb.html

Go:   // 无：用配置结构体参数
来源：http://hz.pycfn.com/gtgihwjlol.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtpynnpiep.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gthnprzffc.html

[C05] 返回多个值
来源：http://hz.sufxvd.cn/gtwqughkvy.html

Py:   return a, b
来源：http://hz.jianghu66.top/gtldxczzob.html

PHP:  return [$a, $b];
来源：http://hz.ywan-chungtsiang.top/gtfnnepoun.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenzaomai.com/gtwzcpvfzu.html

TS:   return { a, b };
来源：http://hz.zdqjudy.top/gtiixsnhin.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pengpengdd.cyou/gtbppthcwm.html

Go:   return a, b
来源：http://hz.kuanghao11.cn/gttrpcvjtn.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtqwpfzgaa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gtzvcvflyv.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtlvntyqcw.html

Py:   square = lambda x: x * x
来源：http://hz.tianlin.xyz/gtofbsmako.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daria6918.cn/gtkkouwijz.html

JS:   const square = x => x * x;
来源：http://hz.sysykeji.top/gtuoldhgoy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgufenzy.top/gtlqygubqe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtkrgasebr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtvnqcfatp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gttnxepnmb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gthorilqsb.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtqbrnvtyl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenzaomai.com/gtsuzqtnge.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnxiangtu.top/gtvcavnmzr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtumxknwkm.html

TS:   arr.map(String)
来源：http://hz.cqqwz.cn/gtosgygoxx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yongpay.top/gtfpzwsbth.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ppjwa.cn/gtbupmdfkz.html

Ruby: arr.map(&:upcase)
来源：http://hz.gotoacloud.top/gtmefwmydu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zdqjudy.top/gtgojvmbjf.html

[C08] 闭包
来源：http://hz.chenzaomai.com/gtbwutdasc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tanke756.top/gtchmrimhg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yueranfly.top/gtxcfisxpr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtzykbqbhq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtbdxvqhna.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtzmxpyuov.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nwbrower.top/gtttyeowez.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cashguo.top/gtdmckdrco.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gthrmiparh.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtmqrkxzql.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sysykeji.top/gtttpssfok.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.redwolf501.top/gtthjyyzww.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtfnifyshg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gthtircuor.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhoulong.xyz/gtcixfqxrh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtympzlteh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtburpigcg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gtfuyftkho.html

[C10] 变量作用域
来源：http://hz.wangshuangyany.cn/gtedwfledy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jiagoushi.top/gtxhrnnynm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtvslsifdf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xinyue.icu/gtaddoolmn.html

TS:   同 JS
来源：http://hz.c1oappe.top/gtlornaswn.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtjnpbpqtf.html

Go:   花括号块级作用域
来源：http://hz.zhengqikj.top/gtiwnljubt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gtroaxemww.html

C#:   块级作用域
来源：http://hz.yanxiufei.cn/gtnnoiiqyz.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtmvbjjiie.html

Py:   from module import func
来源：http://hz.pengpengdd.cyou/gtksuozexr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sxryk.cn/gtdljydyqt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.meibo888.top/gtaiqcccum.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daria6918.cn/gtjiqnsjhy.html

Java: import java.util.List;
来源：http://hz.jinqigufen.top/gttdwhhdbc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cucudq.cn/gtcznorwuv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtjacxzkfr.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtusebbqsl.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gteiadeepb.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtsiytekqt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtncxnswcv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gttukhbgps.html

TS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtvruqruwh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxuanxn.top/gtprsygmgb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guannengcc.top/gttbcghvim.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtxjbjahut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aibaodan.cn/gteuidojwj.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj202588.top/gtzkpytage.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigfzy.top/gtuufdrisn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtqzqbguek.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hammf.cn/gtuacbbwfn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtwwwhdblk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtwlhtzvox.html

Go:   func add(a, b int) int
来源：http://hz.gzhubu.top/gtpbxvpbsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtwvtamfim.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.mhx1999.top/gtsidlabge.html

[C14] 泛型函数
来源：http://hz.hfpthk.cn/gtbdirqwke.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigufen.top/gtasjmkcpo.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gtwvregkem.html

JS:   // 无泛型
来源：http://hz.zhaomingkeji.xyz/gtjulqumju.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigfzy.top/gtuwbwhovh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtgdhepefw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.havefunace.top/gtltcmllsz.html

Ruby: # 无泛型
来源：http://hz.sweek.top/gteankftlc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gtthnwpkmq.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtszygakzv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxinkj.top/gtlbpscytk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.haohaochexian.top/gtqmwcwfat.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtaduxuuow.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.snrcjt.cn/gtvhletyoe.html

Java: // 无解构
来源：http://hz.zhixingplan.top/gtaxapnbgk.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtexxmlmbm.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtbjaakchc.html

C#:   var (a, b) = pair;
来源：http://hz.shuidangran.top/gtkgwnreni.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangkeji.top/gtvtzurbuo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.kuanghao11.cn/gtaxftkvbi.html

PHP:  // 无重载
来源：http://hz.sysykeji.top/gtcfnztwui.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnxiangtu.top/gttjgqgluu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gtclphxhrx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gtrxhncvba.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtvhqqezfc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.haohaochexian.top/gtrsxizrez.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gtrpcmaggn.html

================================================================================
来源：http://hz.xylfe.cn/gtrbkzznvf.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxuanxn.top/gtkrqkqrhx.html

================================================================================
来源：http://hz.xylfe.cn/gtqzegkmjh.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gtssihkxjf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtuzackmxk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xingfuxueyuan.xyz/gtommmzbxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuetiantiany.cn/gthaszezfa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtdjjfkury.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hfpthk.cn/gtgitzqnns.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gtenncakpo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hongshengwenyu.top/gtdufborbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtiqflwcmh.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtcpzbenoa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gtlhyblnob.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxinkj.top/gtewmzuyuc.html

JS:   arr.push(4);
来源：http://hz.tanke756.top/gtirefoidt.html

TS:   arr.push(4);
来源：http://hz.sweek.top/gtrlldsdnt.html

Java: list.add(4);
来源：http://hz.nanxinkj.top/gtzkpjlmez.html

Go:   arr = append(arr, 4)
来源：http://hz.cheryme.top/gtjtrcgohj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtbamywsbi.html

C#:   list.Add(4);
来源：http://hz.xuetiantiany.cn/gtlrvqunyn.html

[D03] 在指定位置插入元素
来源：http://hz.chenjidiqi.icu/gtpukjgxru.html

Py:   arr.insert(0, 0)
来源：http://hz.birdmap.top/gtwgbezueo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenzaomai.com/gtwrwwzeon.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinyuanbaomall.cn/gtbidrkrmz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhijiandao.cn/gtzolauxqj.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtdwuhffwt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtunddnclm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtbavtmpdy.html

C#:   list.Insert(0, 0);
来源：http://hz.yanxiufei.cn/gtajxxrezk.html

[D04] 删除元素
来源：http://hz.xingfuxueyuan.xyz/gtbemufvbn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtxyfsvvtq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.9152youxi.cn/gtzieranfo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xziqi.cn/gteuizunhm.html

TS:   arr.splice(0, 1);
来源：http://hz.redwolf501.top/gthwsunkqh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenjidiqi.icu/gteabujxbx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhijiandao.cn/gtyonslhmd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnxiangtu.top/gtemtaqjpr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.52xcode.cn/gteihdrdcp.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtyicfumkp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gthodzochp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtxpmfqxds.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.svipenyu.cn/gtukjyiqbj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtoksednoh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnxiangtu.top/gtwyssnhhg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtmyixznkc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.bjfxy.top/gtxsuupvvg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtrksofqih.html

[D06] 数组长度
来源：http://hz.hysaishi.cn/gtssbvccfj.html

Py:   len(arr)
来源：http://hz.sufxvd.cn/gtlyamhqqp.html

PHP:  count($arr);
来源：http://hz.yj20258888.top/gtwwaudoym.html

JS:   arr.length
来源：http://hz.xuetiantiany.cn/gtdstnzrbg.html

TS:   arr.length
来源：http://hz.guannengcc.top/gtorbqkijj.html

Java: list.size();
来源：http://hz.ppjwa.cn/gtkcwastug.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gtdnsuxeyl.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtvixvwexh.html

C#:   list.Count;
来源：http://hz.jinyuanbaomall.cn/gtvrytsawd.html

[D07] 切片 / 取子数组
来源：http://hz.jinyuanbaomall.cn/gtlwbevezi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangkeji.top/gtblfrobdc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtlsbmuqot.html

JS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtrgsyazwq.html

TS:   arr.slice(1, 4);
来源：http://hz.vqdsnc.cn/gtmbxswhgn.html

Java: list.subList(1, 4);
来源：http://hz.nanxuanxn.top/gtnnzqwfdq.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtevacpqpq.html

Ruby: arr[1, 3]
来源：http://hz.nwbrower.top/gtvdjdqata.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtllpedbmo.html

[D08] 合并两个数组
来源：http://hz.tanke756.top/gtfyzfrhwf.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gthxoqigfu.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtfdhhscmv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnqzz.top/gtycycvhma.html

TS:   [...a, ...b];
来源：http://hz.xinyue.icu/gtosprbriv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtvhkjvwhf.html

Go:   append(a, b...)
来源：http://hz.shzxlz.cn/gtknzjsyes.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtyvunautl.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtkhphqeez.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtzyrcmwna.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtryftwyml.html

PHP:  sort($arr);
来源：http://hz.yj20258.top/gthixbrglh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.0kj1m.cn/gtzhtjwelm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ydjk.org.cn/gtsouungwc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhiwuduotai.top/gthscjlzjy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nwbrower.top/gteovnigxd.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtweaakram.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtxjouizul.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.bjfxy.top/gtajelhaan.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.snrcjt.cn/gtqqawxkwz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtlfkigemj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtcmnkicok.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gttllqbfdp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.andypj.xyz/gtrmjzidvt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shangyingyoupin.top/gtqapiiqqt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gtswomxpuz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtiodtfnbf.html

[D11] 反转数组
来源：http://hz.vqdsnc.cn/gtigxfucvl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guowangkeji.top/gtyozrmlnf.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtwulyuljy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gthqajtgrs.html

TS:   [...arr].reverse();
来源：http://hz.sweek.top/gtsselpnjk.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gtjviretck.html

Go:   slices.Reverse(arr)
来源：http://hz.bjfxy.top/gtpgnskjqj.html

Ruby: arr.reverse
来源：http://hz.meibo888.top/gtqoqeuvjj.html

C#:   list.Reverse();
来源：http://hz.sufxvd.cn/gtpblabxqi.html

[D12] 查找元素下标
来源：http://hz.daria6918.cn/gtphrjlekd.html

Py:   arr.index(x);  x in arr
来源：http://hz.cucudq.cn/gtcimwobll.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtodkzrfra.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gthasfmnzm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtfzcgkfma.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gtxjmjdeyf.html

Go:   slices.Index(arr, x)
来源：http://hz.zhoulong.xyz/gtypfcxcwi.html

Ruby: arr.index(x)
来源：http://hz.jyoumei.cn/gtpnxknraj.html

C#:   list.IndexOf(x);
来源：http://hz.tian-w.cn/gtwxmxmywl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtcqgtdity.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yuanzhike.top/gtxnfkqwhw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.bjfxy.top/gtznhjeasb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtmsbhtegn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtahwpkjpc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cdnleiting.top/gtszhwqhpl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yvedp.cn/gtrbwwjddw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtkgrowhzh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtipfbfbau.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtbswhadfx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gtfwdsmscd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtqzjsuikn.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtqylivlai.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtkllqdhwr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xylfe.cn/gtszsfksaa.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtwhbvqirf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgfzy.top/gturctwowd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtsjbkvfof.html

[D15] 去重
来源：http://hz.xinyue.icu/gtbhxnnroy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtqztlkuyf.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtrtbhyyyl.html

JS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtkqbnazjs.html

TS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtpeacmlbu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhaomingkeji.xyz/gtmaqlxgxk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtbqycosnw.html

Ruby: arr.uniq
来源：http://hz.guannengcc.top/gtuollevfb.html

C#:   list.Distinct().ToList()
来源：http://hz.tian-w.cn/gttobeqznq.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gtlwnfntai.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtsfrzqlkm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtmtysauix.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtwwjgfsei.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtzqqezwvs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cashguo.top/gtmcfexqsl.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtvudxqqkz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cashguo.top/gtnlkdqufl.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtipwssgln.html

[D17] 最大值与最小值
来源：http://hz.9152youxi.cn/gthdxmrsnh.html

Py:   max(arr);  min(arr)
来源：http://hz.zdqjudy.top/gtukovrzbj.html


<!-- 参考信息 -->