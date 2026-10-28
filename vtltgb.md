代发 wailian999

Java: if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtvqzepilj.html

Go:   if data == nil { return }
来源：http://hz.havefunace.top/gtlopucwqg.html

Ruby: return if data.nil?
来源：http://hz.zycfv.cn/gtvgdrvjao.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtmpleycph.html

================================================================================
来源：http://hz.daria6918.cn/gtsgnaxqdp.html

C. 函数与作用域
来源：http://hz.jqgufenzy.top/gtywhiawso.html

================================================================================
来源：http://hz.yuanzhike.top/gtumuxmebh.html

[C01] 定义函数
来源：http://hz.yangfankeji.com/gtksssqsbc.html

Py:   def add(a, b): return a + b
来源：http://hz.ivvv.top/gtwqlcxjuh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtskkugrac.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtkrdjydip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtbgboppzr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtmuvufiui.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhixingplan.top/gtdsmfkqkb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxinkj.top/gtenvhakla.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtklebdvfs.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtpjlhlbig.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258.top/gtepenqgqh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xziqi.cn/gtyolyndbf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.9152youxi.cn/gtzuwqcxcy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.bjfxy.top/gtgbvialfk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shangyingyoupin.top/gtsldrsgrt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hfpthk.cn/gtfdusivpb.html

Ruby: def greet(name = "World") = name
来源：http://hz.c1oappe.top/gttcwegxet.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ybcxt.top/gtzjytzcqf.html

[C03] 可变参数
来源：http://hz.yj202588.top/gtvveglqra.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gtvdvoeckp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.guannengcc.top/gtxwdwzpip.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtataladxk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gthtppkgyv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nwbrower.top/gtpbqlebcm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pycfn.com/gttrvjxphe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinyuanbaomall.cn/gtlqlrpjdr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtracfakug.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtzvfhttby.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.quarkkingdee.top/gtlazjzfko.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtptsicpyl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtdjpjljjz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gttyococme.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zdqjudy.top/gtjsgstoyi.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenlongwang.top/gtuvdpcqzd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtgygbqevt.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtdxncxkdi.html

[C05] 返回多个值
来源：http://hz.mhx1999.top/gttxoahkvd.html

Py:   return a, b
来源：http://hz.hywenlv.cn/gtequdqecr.html

PHP:  return [$a, $b];
来源：http://hz.ydjk.org.cn/gtzmkhwfvf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yonumen.top/gtvtpjvfyk.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtaohrhhat.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cucudq.cn/gtxsckzvhf.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtpbnfgrvl.html

Ruby: return a, b
来源：http://hz.sxryk.cn/gtvoonwwrs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.snrcjt.cn/gtzbncqcui.html

[C06] 匿名函数 / lambda
来源：http://hz.fzhhl.top/gtknhcwuit.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gttciufair.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tian-w.cn/gtmhbczwjo.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtprggovvo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dashuyun.cn/gtnbifkeax.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.redwolf501.top/gtzaitvnyn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gttgbkxlbs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xingfuxueyuan.xyz/gtpxtvikoo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cheryme.top/gtkhklsmrc.html

[C07] 把函数作为参数传入
来源：http://hz.fzhhl.top/gtqivscgki.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.svipenyu.cn/gtjpmtxgwl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gzhubu.top/gtutkgimoq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gthfhtytna.html

TS:   arr.map(String)
来源：http://hz.sweek.top/gtzbvyhvpy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgfzy.top/gtqwmrduvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guannengcc.top/gtpbvycfdd.html

Ruby: arr.map(&:upcase)
来源：http://hz.hammf.cn/gtgauvenor.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shuidangran.top/gtpqgrwpud.html

[C08] 闭包
来源：http://hz.aibaodan.cn/gtczvupcpw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gotoacloud.top/gtrmdrbjva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.52xcode.cn/gtkirvmxof.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtwxkximbf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtinhnkhwi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gotoacloud.top/gtbvcvudph.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hfpthk.cn/gtgotogmvp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aibaodan.cn/gtpxsetksq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtpinxafnj.html

[C09] 递归
来源：http://hz.zhixingplan.top/gteizkprtx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtsjcfupci.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtsbazzxml.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtqbyfnwcc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtadvnpbns.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenzaomai.com/gtbctppgdu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gteftvygqk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtegwtirvg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daria6918.cn/gtvzwlfmeo.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtfmhaaqrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtkopwzoza.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gtkcfsuhvk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hfpthk.cn/gthjdtrpxm.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtaoaqadte.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtusigzhgc.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtxyzgexkt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gthgyghoam.html

C#:   块级作用域
来源：http://hz.xuanzx.com/gtbhjyxezh.html

[C11] 模块导入与导出
来源：http://hz.bjfxy.top/gtoqfwqjub.html

Py:   from module import func
来源：http://hz.jqgufenzy.top/gtfyouvdph.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gttcxvagua.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtrxmmnpsa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sweek.top/gtfpwbbenw.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtkrxgyewz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xylfe.cn/gtdnkanmuj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtdslepxxw.html

C#:   using System.Text;
来源：http://hz.ehwqpu.com/gtwjwbptyn.html

[C12] 立即执行函数 IIFE
来源：http://hz.yongpay.top/gtqhpzkwpt.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtlbotfoxy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sysykeji.top/gtrivvmmzz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtlaedqsfr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtadjxonus.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zycfv.cn/gtjugfxqvy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.andypj.xyz/gthqphnaew.html

Ruby: -> { puts "run" }.call
来源：http://hz.jlsjyb.cn/gtrbrkucja.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gtmoalyvpf.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenjidiqi.icu/gtgwdlimla.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.feifeiyinyue.top/gttyilachx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtxoxixrvs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gtpwkkzdzs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gtdksaslgg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtrriflodp.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtrqmizmak.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sufxvd.cn/gtjfbeprqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtlxhegahj.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtrsnjpjnn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ivvv.top/gtczwqfbya.html

PHP:  // 无泛型
来源：http://hz.redwolf501.top/gtrskozqba.html

JS:   // 无泛型
来源：http://hz.9152youxi.cn/gtnmspbpwv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sweek.top/gthlbahosq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gttfkfmgbk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.kuanghao11.cn/gtblifjkes.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtkvfxmdxg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ywan-chungtsiang.top/gtfeuzhsfj.html

[C15] 解构 / 展开参数
来源：http://hz.jyoumei.cn/gtsgbsykwu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gtjhcbmhov.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhoulong.xyz/gtkvyhxbxz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.meibo888.top/gtiqsnvzqf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtdsikzghh.html

Java: // 无解构
来源：http://hz.yonumen.top/gtfvifauey.html

Go:   // 无解构
来源：http://hz.ybcxt.top/gtshbysotz.html

Ruby: a, b = pair
来源：http://hz.xylfe.cn/gtkxnjuoqk.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtvrvvrogr.html

[C16] 函数 / 方法重载
来源：http://hz.cdnleiting.top/gtnswbxudf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gtdnemaidj.html

PHP:  // 无重载
来源：http://hz.fengsongda.top/gtytwqrzuc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtbvhmeuuf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtuoflldpd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shuidangran.top/gtdctgcnki.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhoulong.xyz/gtjzdeqdgt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtpabxyjdw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtmsavtfsg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtowbnfofm.html

D. 数组 / 列表 / 集合
来源：http://hz.smart0.xyz/gtfslrwtwu.html

================================================================================
来源：http://hz.cdnleiting.top/gthabnlhwf.html

[D01] 创建数组 / 列表
来源：http://hz.aibaodan.cn/gtclccfokx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinghuilouyu.cn/gtoemjhjby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.kuanghao11.cn/gtelrwkugc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gtodbmiuux.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xylfe.cn/gtheczirqw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ehwqpu.com/gthnsbyjqg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtolkejuul.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhongyouzk.top/gtdawkrbie.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.vqdsnc.cn/gtwdveawrc.html

[D02] 追加元素到末尾
来源：http://hz.chenjidiqi.icu/gtxwcjacdg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tanke756.top/gtkuiernlm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.andypj.xyz/gtbkysbqjh.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtxsfkaqrf.html

TS:   arr.push(4);
来源：http://hz.zycfv.cn/gtlftxzklk.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtxkvqtegr.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gtdimyceyo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhijiandao.cn/gtjakifxfb.html

C#:   list.Add(4);
来源：http://hz.jinghuilouyu.cn/gtaixxpnkt.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtcfpgqvxh.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxinkj.top/gtdppovjbk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.redwolf501.top/gttlpoiroy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtianhqaop.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtkczfigoo.html

Java: list.add(0, 0);
来源：http://hz.jianghu66.top/gtskfsfrim.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sufxvd.cn/gtqpajerww.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangdashe.top/gtnughgriz.html

C#:   list.Insert(0, 0);
来源：http://hz.yueranfly.top/gtwgjtwajp.html

[D04] 删除元素
来源：http://hz.ppjwa.cn/gtpvadqmjc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xinyue.icu/gteejturln.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtmkqcqtjp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gtkymsjppt.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtdkijdzun.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtlmvqvhys.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtbomzpcif.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtsoquglqf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ybcxt.top/gtdlzconfl.html

[D05] 访问与修改元素
来源：http://hz.jinqigufen.top/gtdfqfhder.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtgglkjxwg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gthtpxszbu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gzhubu.top/gtevljbjau.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xinyue.icu/gtvxkjdfgj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ppjwa.cn/gtnbkykgqp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tianlin.xyz/gthgsutucm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gttsjfoeso.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtmpveyglp.html

[D06] 数组长度
来源：http://hz.zhijiandao.cn/gtsupzuwsk.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtlnuzcnyl.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtkysvuazy.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtnowivtjc.html

TS:   arr.length
来源：http://hz.xylfe.cn/gtcoadnmic.html

Java: list.size();
来源：http://hz.hongshengwenyu.top/gtjuadavae.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtegrkdkko.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtjcabswlm.html

C#:   list.Count;
来源：http://hz.gaohongyu789.top/gtzekrcphe.html

[D07] 切片 / 取子数组
来源：http://hz.cheryme.top/gtlzqkegle.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sufxvd.cn/gtmluwzzrk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gtrjqiduib.html

JS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtgvdvnquv.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtunufxiko.html

Java: list.subList(1, 4);
来源：http://hz.cheryme.top/gtfvmqycxa.html

Go:   arr[1:4]
来源：http://hz.c1oappe.top/gtjtflyhlt.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtvoxivzlk.html

C#:   list.GetRange(1, 3);
来源：http://hz.smart0.xyz/gtsxrgylnj.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gtrjioftff.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gthtsviewf.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtlmnlasia.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtaymmmukl.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtzwuqijoz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cashguo.top/gtewyjltdx.html

Go:   append(a, b...)
来源：http://hz.redwolf501.top/gtqntsprnj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gtbjsrqdzj.html

C#:   a.Concat(b).ToList()
来源：http://hz.bjfxy.top/gtesmgnyjc.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gtotnxpmyf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtezqezaku.html

PHP:  sort($arr);
来源：http://hz.ehwqpu.com/gtjcyzpgtc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cucudq.cn/gtwnqwontg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tanke756.top/gthzkksgym.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yonumen.top/gtqbjsdbzv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.c1oappe.top/gtjvngyskx.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gtomepbgbb.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtilzsgrde.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gterbhhucc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shzxlz.cn/gtneehlbjs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtloimlqts.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenzaomai.com/gtqwngwavl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtyymrgubs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aizwys.cn/gtxzmbwsjb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xingfuxueyuan.xyz/gtxztalunm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydjk.org.cn/gtfidacdle.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenjidiqi.icu/gtbssnhppn.html

[D11] 反转数组
来源：http://hz.andypj.xyz/gtjaqqjeku.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.mhx1999.top/gtdeehjgcm.html

PHP:  array_reverse($arr);
来源：http://hz.chenlongwang.top/gtatcnisif.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuetiantiany.cn/gtlqneumor.html

TS:   [...arr].reverse();
来源：http://hz.nanxuanxn.top/gtldbqgeew.html

Java: Collections.reverse(list);
来源：http://hz.zhijiandao.cn/gtzmtfcdpv.html

Go:   slices.Reverse(arr)
来源：http://hz.jinyuanbaomall.cn/gtkaadorrj.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtsgzmlwlt.html

C#:   list.Reverse();
来源：http://hz.quarkkingdee.top/gthfftnuli.html

[D12] 查找元素下标
来源：http://hz.yvedp.cn/gtaxifxsds.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydzc1.top/gtiqbftjrs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gthzfmgxiy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtlichwkkn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtensnoeip.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258.top/gtvydstycx.html

Go:   slices.Index(arr, x)
来源：http://hz.hywenlv.cn/gtsmqdtftz.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gtkbcolryc.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gttpqtvecp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sxryk.cn/gtfomatehk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gticqrmgre.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daxiang520.top/gtbtinjyhn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtpbyuvuqk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtjlckjsef.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangkeji.top/gtfizmqsik.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenlongwang.top/gtfuufykcy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtleimtqmn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yongpay.top/gtrgqsvrtd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.havefunace.top/gtfvazydpf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shzxlz.cn/gtjdplpjlc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxuanxn.top/gtrxtsnwfs.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtoydxufpu.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtypftyfls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtpqwbiudj.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtsmmsdkjn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gogol.net.cn/gtlajosllo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daxiang520.top/gtbboocgvx.html

[D15] 去重
来源：http://hz.ywan-chungtsiang.top/gtietzgczv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtizgtgnmz.html

PHP:  array_unique($arr);
来源：http://hz.sysykeji.top/gtiqfjiqjv.html

JS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtcjxockkr.html

TS:   [...new Set(arr)]
来源：http://hz.tian-w.cn/gtfdscksbu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jianghu66.top/gtasqpxsst.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtungejbie.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtyzphpvhn.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxuanxn.top/gtmkpqoqyz.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtksubzjoy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtormjfbfx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtoakluzsp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtcimfctey.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gttlbqvmui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.c1oappe.top/gtbsqldwso.html

Go:   // 手写循环累加
来源：http://hz.tian-w.cn/gtbkuiuztd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangshuangyany.cn/gtpwsfrvdl.html

C#:   list.Sum();  list.Average()
来源：http://hz.0kj1m.cn/gtyspnirxr.html

[D17] 最大值与最小值
来源：http://hz.aizwys.cn/gtlmetlblu.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxinkj.top/gtzqzfcwtu.html


<!-- 参考信息 -->