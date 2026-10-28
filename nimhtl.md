代发 wailian999

================================================================================
来源：http://hz.tianlin.xyz/gtedpkqcni.html

C. 函数与作用域
来源：http://hz.yj20258888.top/gtjrqgthiq.html

================================================================================
来源：http://hz.shuidangran.top/gtarbpstgj.html

[C01] 定义函数
来源：http://hz.chenlongwang.top/gteyvejfsw.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangkeji.top/gtoftlseeh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtyapofyxf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtlihnyudg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtujadueri.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtehxduejy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtodfblvsk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhixingplan.top/gtdimpayat.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtlkinsfel.html

[C02] 默认参数
来源：http://hz.yueranfly.top/gtcojngccf.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gtgpsydfqv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenlongwang.top/gttzvatpet.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gtmblbtjwd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtbuqjuaic.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.316326.xyz/gtsayxjclw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhoulong.xyz/gtrnnlavug.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gttxznenqh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xuanzx.com/gthszhlfta.html

[C03] 可变参数
来源：http://hz.redwolf501.top/gtqvqertaf.html

Py:   def total(*args): return sum(args)
来源：http://hz.c1oappe.top/gthbrpmdva.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.guannengcc.top/gtcgiydjlg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtsbmetjgj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtezrptbsa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gtyvptupip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtxeooujzz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dianchejie.cn/gtplejpilz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cashguo.top/gtloshsrgf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtgpisibbl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sxryk.cn/gtytwaimnf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zdqjudy.top/gtpbijpnlk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtjuncaxvk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtiqczhxna.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gtccizdbqo.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenzaomai.com/gtsgwzzzob.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtyzlnnrof.html

C#:   f(a: 1, b: 2)
来源：http://hz.birdmap.top/gtoeknbnpx.html

[C05] 返回多个值
来源：http://hz.hysaishi.cn/gtrgstzwib.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gttkbhrsdd.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtcwbcyqnl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtvydgiksw.html

TS:   return { a, b };
来源：http://hz.iojbl.cn/gtmnxkuxpt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yonumen.top/gtyjnespam.html

Go:   return a, b
来源：http://hz.dianchejie.cn/gtytrnzkvc.html

Ruby: return a, b
来源：http://hz.pycfn.com/gtkmbrddvk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nwbrower.top/gtezbboxtt.html

[C06] 匿名函数 / lambda
来源：http://hz.zhoulong.xyz/gtvxdoayzs.html

Py:   square = lambda x: x * x
来源：http://hz.hfpthk.cn/gtwkwojqap.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ivvv.top/gtiulqjoqq.html

JS:   const square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtpwowrmwj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtjjccyfck.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tian-w.cn/gtyfjokbqd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtqrftppyf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtrfenuqeh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tanke756.top/gtyvlfgqov.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtnjfgeqfl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shuidangran.top/gtljikhlbc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gteksggcla.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.pycfn.com/gtapgchjqm.html

TS:   arr.map(String)
来源：http://hz.birdmap.top/gttmgttbki.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yonumen.top/gtghmqqcyw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dianchejie.cn/gttztkeeyj.html

Ruby: arr.map(&:upcase)
来源：http://hz.xingfuxueyuan.xyz/gtrlfochhh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.pengpengdd.cyou/gthfkzrnrj.html

[C08] 闭包
来源：http://hz.yongpay.top/gtauhktesl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.redwolf501.top/gtimsegipy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gzhubu.top/gtqmyigkub.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtnxygeubm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtfwibyjpc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.c1oappe.top/gtskjuiufd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.svipenyu.cn/gtslasdwez.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtszizucns.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtcebkrmej.html

[C09] 递归
来源：http://hz.wangdashe.top/gtjtoqxykh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtfdfaswgh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhiwuduotai.top/gtzhiasgkx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtmeneondp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtapiijfqg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yonumen.top/gtmxfsnnkj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtubneewvm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtsxwzvqqc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hysaishi.cn/gtyimwxqsc.html

[C10] 变量作用域
来源：http://hz.chenlongwang.top/gtcgskxqrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtcyefdntf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yvedp.cn/gtzdoisaht.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gthxcgkrvm.html

TS:   同 JS
来源：http://hz.yanxiufei.cn/gtnhomriab.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtltgshgwc.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtwblxunxd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtiggbfkia.html

C#:   块级作用域
来源：http://hz.sxryk.cn/gthmwalsft.html

[C11] 模块导入与导出
来源：http://hz.hfpthk.cn/gtixqoodch.html

Py:   from module import func
来源：http://hz.jinqigfzy.top/gtoiokttot.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258.top/gtwlgswbvo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shangyingyoupin.top/gtkjufmsag.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtlpigaexf.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtvtbsuxhe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.meibo888.top/gtzeapglud.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtmdopihmw.html

C#:   using System.Text;
来源：http://hz.jlsjyb.cn/gtzfmecokv.html

[C12] 立即执行函数 IIFE
来源：http://hz.gaohongyu789.top/gtxiiwmvnl.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangkeji.top/gtodnnokmk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnxiangtu.top/gtidhwxmgr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtikxudoma.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gtstyvrbvb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jiagoushi.top/gtzpkuwpff.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ppjwa.cn/gtbuhpwmfk.html

Ruby: -> { puts "run" }.call
来源：http://hz.yangfankeji.com/gtgbsogmvt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pengpengdd.cyou/gtwsvtfwwl.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtqtqvsumj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hammf.cn/gtglzqgjua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtqwuqfgtv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtkzniscfu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gtiznwlshw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gteuulattj.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtvtlrhnvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sxryk.cn/gttikamnim.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtdhryldpx.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtlbjqsjhy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydzc1.top/gtjmnocosc.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gteymkstnp.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtaukuhjjg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hywenlv.cn/gthvksosxb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtjnsgdhzi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gtypopeuvu.html

Ruby: # 无泛型
来源：http://hz.ydjk.org.cn/gtosuvbpnu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtkpkusrxv.html

[C15] 解构 / 展开参数
来源：http://hz.tian-w.cn/gtkftxafch.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhixingplan.top/gtjnqjsato.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zycfv.cn/gtrtkvxtpm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtnzfcrpwv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.smart0.xyz/gtlxnnyday.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtiiyuasoo.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gteziehiue.html

Ruby: a, b = pair
来源：http://hz.xinyue.icu/gtqnmvvqcm.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtvvicevzk.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangkeji.top/gtqkjetnas.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtfzpunuid.html

PHP:  // 无重载
来源：http://hz.feifeiyinyue.top/gtwkzhegqw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.52xcode.cn/gtqhdniuzt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aibaodan.cn/gtdgsnidkf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtmwjcxsbi.html

Go:   // 无重载：用不同函数名
来源：http://hz.yonumen.top/gtpxjdvbhk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtxzzevsbz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.0kj1m.cn/gtaqgnwleq.html

================================================================================
来源：http://hz.hfpthk.cn/gtvjhsgjof.html

D. 数组 / 列表 / 集合
来源：http://hz.jianghu66.top/gtqqvwptoy.html

================================================================================
来源：http://hz.sweek.top/gtjwjtcwde.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtetatdlaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.aibaodan.cn/gtqmryodhq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gtradkfagq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtrxtgfwtr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pengpengdd.cyou/gtoghrfvxx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenzaomai.com/gthzfrgayx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj202588.top/gtqdfjpofw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.9152youxi.cn/gtjwdvjnoe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daria6918.cn/gtrlinovul.html

[D02] 追加元素到末尾
来源：http://hz.shuidangran.top/gtsecyamtj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtrkkxyzfk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.andypj.xyz/gtggkawfxi.html

JS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtnvtctxvd.html

TS:   arr.push(4);
来源：http://hz.shzxlz.cn/gturokbred.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gttjzczmyf.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtmjnuhllc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258.top/gthlboqeoj.html

C#:   list.Add(4);
来源：http://hz.chenzaomai.com/gtoutmicaa.html

[D03] 在指定位置插入元素
来源：http://hz.andypj.xyz/gtukughrlp.html

Py:   arr.insert(0, 0)
来源：http://hz.yuxming.cn/gtaypeaszd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yongpay.top/gtsujwrstw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinyuanbaomall.cn/gtpzsyiqcx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shangyingyoupin.top/gtjezwxstx.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtrsydameg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhoulong.xyz/gtkccbjuow.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenzaomai.com/gtoecdzuwc.html

C#:   list.Insert(0, 0);
来源：http://hz.c1oappe.top/gtnjuabiku.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtlecprwcv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dianchejie.cn/gtttsbsuwd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gtmebtvxbl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.meibo888.top/gtbjiiedue.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtliozkkke.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtmbsoqlxc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fengsongda.top/gtvnrtejhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtmqgvlfem.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangkeji.top/gtbbwkhnda.html

[D05] 访问与修改元素
来源：http://hz.jinqigfzy.top/gterqwwgnh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtemtmrfht.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtftxmrazr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yongpay.top/gtdqiwdbkc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.kuanghao11.cn/gtyuynydtp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.andypj.xyz/gtmsectzmi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtlxqrshpf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtzgjvhgcm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtiutcmwpj.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gtahowgbqy.html

Py:   len(arr)
来源：http://hz.gogol.net.cn/gtjpaaxrsc.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtkhurjrwr.html

JS:   arr.length
来源：http://hz.yvedp.cn/gtjjniavys.html

TS:   arr.length
来源：http://hz.cheryme.top/gtuswoiaqr.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtilycvjxb.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtbywyzypt.html

Ruby: arr.length; arr.size
来源：http://hz.yj20258888.top/gtbuumjjvq.html

C#:   list.Count;
来源：http://hz.tanke756.top/gtluwquhyp.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtxkcmmrti.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtpioistii.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yongpay.top/gtozwvetqd.html

JS:   arr.slice(1, 4);
来源：http://hz.daxiang520.top/gtmpewkoml.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtsnnbbgwj.html

Java: list.subList(1, 4);
来源：http://hz.c1oappe.top/gtgfvgpbhl.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gtpnvkwhzl.html

Ruby: arr[1, 3]
来源：http://hz.aibaodan.cn/gtmriptfzv.html

C#:   list.GetRange(1, 3);
来源：http://hz.redwolf501.top/gtzbudcqbr.html

[D08] 合并两个数组
来源：http://hz.hnxiangtu.top/gthrlriwrr.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gthvoxgpkp.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gthiumyfwe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hfpthk.cn/gtqpgnshit.html

TS:   [...a, ...b];
来源：http://hz.yj20258.top/gtkeqhfadv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigufen.top/gtttlxebrd.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtadbwjjby.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guannengcc.top/gtpgasgfpv.html

C#:   a.Concat(b).ToList()
来源：http://hz.birdmap.top/gtfgsoqyyy.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtfzahwgtb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtkxrafygy.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtuxasigwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.kuanghao11.cn/gtivvfgyms.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daria6918.cn/gtgxsmiqfh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gthurezrvy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gtrgzlympm.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtqxapwpvi.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtglskzdxy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hysaishi.cn/gtrdeofxbp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guowangkeji.top/gtawuvjfnl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtzmmxdxrr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtpqyktuej.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtkmzkedfc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenjidiqi.icu/gtpuqkzazf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nwbrower.top/gtrbyytaww.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.316326.xyz/gttskiuvam.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yongpay.top/gtcgblxbro.html

[D11] 反转数组
来源：http://hz.pengpengdd.cyou/gtrbbfpong.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xziqi.cn/gtoparztdh.html

PHP:  array_reverse($arr);
来源：http://hz.cheryme.top/gtdsloidvw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtrablgubm.html

TS:   [...arr].reverse();
来源：http://hz.bjfxy.top/gthydqlgkk.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtvbmpcled.html

Go:   slices.Reverse(arr)
来源：http://hz.aizwys.cn/gtoarqgtmj.html

Ruby: arr.reverse
来源：http://hz.cucudq.cn/gtiivrqkjt.html

C#:   list.Reverse();
来源：http://hz.yj202588.top/gtbbajgfve.html

[D12] 查找元素下标
来源：http://hz.jianghu66.top/gtflkaters.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gthuuhuina.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtwsfmuhfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtbtvogvsd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtjwwjjycw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtbvevpesy.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtsnmubuam.html

Ruby: arr.index(x)
来源：http://hz.quarkkingdee.top/gtvdvbbbms.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtboxejucb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cucudq.cn/gtropmqcve.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shuidangran.top/gtyadextwq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fengsongda.top/gtvciftski.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtpukzdrfa.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtaunlcnru.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtbgezzgus.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cheryme.top/gtugrxequt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhaomingkeji.xyz/gtnyawbysy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.guannengcc.top/gtnaipiyti.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuxming.cn/gtirzwadmm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtwbmmhdjw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhiwuduotai.top/gtwkjaiuvz.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtnpamxkza.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gttoteewho.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtnmaapwvk.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtfdjyeuoy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtpkhkqoan.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gtnvrlblia.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtuihadbcb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtojuthphk.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtnmcnemim.html

JS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtodvaoiei.html

TS:   [...new Set(arr)]
来源：http://hz.hysaishi.cn/gtijyfffhq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daxiang520.top/gtnbxgjfiw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtktsulhjd.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtkukdqnri.html

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gtqomvsyab.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtygvtetcv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtbvghkeyh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtbbmknzwl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtwmqagjth.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gthuowgavq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtdhykbzxy.html

Go:   // 手写循环累加
来源：http://hz.ybcxt.top/gtgsferpvh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtpzitfupz.html

C#:   list.Sum();  list.Average()
来源：http://hz.hammf.cn/gtjemkxxsm.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtvaotcelt.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtcjbwrbep.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtpeqgchil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtafthaumm.html

TS:   Math.max(...arr);
来源：http://hz.ywan-chungtsiang.top/gtnpumkhgy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenlongwang.top/gtvofvbjsg.html


<!-- 参考信息 -->