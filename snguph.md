代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtdwcnkikg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtsglcisby.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinqigfzy.top/gtaztfgmcv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtpmidrbbs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtbezbrocx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.haohaochexian.top/gtrgmgzrhn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtrwcujevb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xinyue.icu/gtyulgtkkk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tianlin.xyz/gtnhulxigy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtfiumcgew.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigfzy.top/gtxtbegxxs.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtdgqpmvyr.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj202588.top/gtuwucvvdp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sweek.top/gtgnaeyurg.html

C#:   f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtykvjgjhr.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtywrywgos.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtkvfrprlh.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtlsqlilom.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtlxrozgwl.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtwppkufta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhongyouzk.top/gtdkiinlew.html

Go:   return a, b
来源：http://hz.nwbrower.top/gtswjwhwdu.html

Ruby: return a, b
来源：http://hz.snrcjt.cn/gturarircg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gthdqfnqwf.html

[C06] 匿名函数 / lambda
来源：http://hz.yvedp.cn/gtcnyupniz.html

Py:   square = lambda x: x * x
来源：http://hz.tanke756.top/gtpxvgklui.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtelswnhba.html

JS:   const square = x => x * x;
来源：http://hz.c1oappe.top/gtaiklbvzt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.52xcode.cn/gtpwoubpnf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zdqjudy.top/gtxhvwzkzl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnxiangtu.top/gtogyyjygl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuetiantiany.cn/gttqqxsrnk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dianchejie.cn/gtnsrvzxbp.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gtvfjocqtf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jlsjyb.cn/gtenjndlwa.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtiheqgqnx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinghuilouyu.cn/gtfjhuwipq.html

TS:   arr.map(String)
来源：http://hz.jinghuilouyu.cn/gtqqogwcts.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ybcxt.top/gteagrspac.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yueranfly.top/gtlndibpqr.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtdbxorzjl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtlhtzmyck.html

[C08] 闭包
来源：http://hz.hnxiangtu.top/gttcbrfmit.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ybcxt.top/gteftvilqa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.feifeiyinyue.top/gttfjvvpcz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtfdkxnutf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtxcgrmmxf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fengsongda.top/gtysccwjek.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gthfkonbjt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258888.top/gtxjdxnjxc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtnqfcjhpt.html

[C09] 递归
来源：http://hz.zdqjudy.top/gtiacltkae.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtrnvcfcsh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtrjkbqxoz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtzpjijzhm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtnsrgfnim.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtyjaxxbix.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtvbhhyjig.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydzc1.top/gtgnxzslmk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gtqfsempsq.html

[C10] 变量作用域
来源：http://hz.zhaomingkeji.xyz/gtnrnxjzmp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guannengcc.top/gtoivadgag.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dianchejie.cn/gtfxeaexgp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gotoacloud.top/gtbzsqjbby.html

TS:   同 JS
来源：http://hz.fzhhl.top/gtvvmzhzhv.html

Java: 方法内为块级作用域
来源：http://hz.zhongyouzk.top/gtpoxkqdum.html

Go:   花括号块级作用域
来源：http://hz.jlsjyb.cn/gtgkzgfsge.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.vqdsnc.cn/gtldyxlrlh.html

C#:   块级作用域
来源：http://hz.xuanzx.com/gtlyffnchu.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtfgchalyr.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gtoeqndclg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.daria6918.cn/gtmsqyneqt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj20258888.top/gtjdlxoike.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtucicelgx.html

Java: import java.util.List;
来源：http://hz.gzhubu.top/gtoqlralzh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtohzeyqng.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sxryk.cn/gtjzspdgxy.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtomeurzmq.html

[C12] 立即执行函数 IIFE
来源：http://hz.cdnleiting.top/gtkxqisime.html

Py:   (lambda: print("run"))()
来源：http://hz.yongpay.top/gttgnlervb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yonumen.top/gtvewckofl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtvfgffjzq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtfjdewdhg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gaohongyu789.top/gtgodgtoaz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgfzy.top/gtabsvdrtl.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258.top/gtnjmhiqcu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtvdzxxfnr.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gtstrlucme.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.meibo888.top/gtxcvgtpjb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtanfdwhtx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.52xcode.cn/gtcltoowfw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtoncmahlf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtezaczeyk.html

Go:   func add(a, b int) int
来源：http://hz.tian-w.cn/gtleajhmtx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtmcxairst.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sweek.top/gtyoabordf.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtnzxvvhuo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtqkvgtsvz.html

PHP:  // 无泛型
来源：http://hz.iojbl.cn/gtjzzrshhp.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtntuvebcp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtieqyifxf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gttxevdztu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gtcvwjwcuz.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtfjpmnrvt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cdnleiting.top/gtztguabbj.html

[C15] 解构 / 展开参数
来源：http://hz.ywan-chungtsiang.top/gtgejzxoaw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aizwys.cn/gtniumzoel.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtygrbocok.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtbvlwjscn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shuidangran.top/gttbpiyanw.html

Java: // 无解构
来源：http://hz.cheryme.top/gtxjczbrhm.html

Go:   // 无解构
来源：http://hz.yanxiufei.cn/gtcltsqudo.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtkxbrndjp.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gtddflgsip.html

[C16] 函数 / 方法重载
来源：http://hz.yuxming.cn/gtmvzeanxj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenlongwang.top/gtarookonw.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtubshmqit.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.pycfn.com/gtxgbfwoti.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xingfuxueyuan.xyz/gtyqkwjavu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtcvxmxwzl.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangdashe.top/gtwigxnlet.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cqqwz.cn/gtsgtimdeb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.smart0.xyz/gtsfwntsqz.html

================================================================================
来源：http://hz.jyoumei.cn/gtedqqeyfe.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtglvcstrl.html

================================================================================
来源：http://hz.sufxvd.cn/gtuherxpqs.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtxswibkmq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtbgetgkcj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtdwimzmsu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hongshengwenyu.top/gttarlzefl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtggkhiohr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtlmyomyly.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jlsjyb.cn/gtnvjzbnhv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gogol.net.cn/gtgrwcbnto.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtazvwgohx.html

[D02] 追加元素到末尾
来源：http://hz.shangyingyoupin.top/gtcziqmyxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yueranfly.top/gtggygnrhz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guannengcc.top/gtbauqrzim.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtshkjomsg.html

TS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtqkyjrobz.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gtfqxfdewd.html

Go:   arr = append(arr, 4)
来源：http://hz.shuidangran.top/gtwfbayaog.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jqgufenzy.top/gttreavmhh.html

C#:   list.Add(4);
来源：http://hz.316326.xyz/gtrdbabqgp.html

[D03] 在指定位置插入元素
来源：http://hz.jqgufenzy.top/gtylnuckww.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gtemoesdlt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydjk.org.cn/gtryrfsfvo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.bjfxy.top/gtsrffgfyi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pycfn.com/gtgamtjvgk.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gthauurxew.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hywenlv.cn/gtlitcwhkc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigufen.top/gtxzgvxudm.html

C#:   list.Insert(0, 0);
来源：http://hz.chenlongwang.top/gtnjcxfgit.html

[D04] 删除元素
来源：http://hz.fengsongda.top/gtikwyefqy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aibaodan.cn/gtemrfrzjj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ehwqpu.com/gtntcvswvm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hysaishi.cn/gtlqxvrodq.html

TS:   arr.splice(0, 1);
来源：http://hz.yj202588.top/gtynlvttds.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtcnvgwhmz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gtmhqjbiqm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxuanxn.top/gtvczkgcvv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.birdmap.top/gtqhnsihgx.html

[D05] 访问与修改元素
来源：http://hz.nwbrower.top/gtmxchcqpz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtlwgenupo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gtgurtfyqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtbrmvrvgs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yongpay.top/gtluhzwtxq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.316326.xyz/gtfzvvzrlh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtxhhgogqz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gthjqcbaru.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yvedp.cn/gtiaioyjnv.html

[D06] 数组长度
来源：http://hz.xuetiantiany.cn/gtohezeqys.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gttseeulmy.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtfhgcxtum.html

JS:   arr.length
来源：http://hz.svipenyu.cn/gtmppxqaig.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtpqadvggu.html

Java: list.size();
来源：http://hz.hongshengwenyu.top/gtqcxhbkpr.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtzgyamqfr.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gttdpewqfs.html

C#:   list.Count;
来源：http://hz.0kj1m.cn/gtusbnrsvs.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gttdltinap.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtexrcqdlu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtyhfgqake.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtjavhjadp.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtisbmeegb.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtxdtyjrkg.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gteblqczon.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gtgyhcngxq.html

C#:   list.GetRange(1, 3);
来源：http://hz.birdmap.top/gtasqechrx.html

[D08] 合并两个数组
来源：http://hz.smart0.xyz/gtkfybihda.html

Py:   a + b;  a.extend(b)
来源：http://hz.cucudq.cn/gtuhvyqcba.html

PHP:  array_merge($a, $b);
来源：http://hz.zhixingplan.top/gtfnjynmnk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.birdmap.top/gtemwiuqvb.html

TS:   [...a, ...b];
来源：http://hz.xuetiantiany.cn/gtojzawnwf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gtijbdhqfb.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gthlxhkxja.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnqzz.top/gtwbkimsmr.html

C#:   a.Concat(b).ToList()
来源：http://hz.cucudq.cn/gtrvzbqczj.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtqbukztwd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtguvqxinw.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtmrndaoiz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtskuklbpz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gogol.net.cn/gtparvlaqg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtzmupyary.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangdashe.top/gtwafskyip.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtbcmpaktu.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtigjqazpb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtopfyaorc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xingfuxueyuan.xyz/gtowkrehsi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtojqlucnf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtzbjiqoox.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtburraixl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinghuilouyu.cn/gtbnsiwmhg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtifngzqzu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtwxzfizmc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtxalripba.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gtapnuhvoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtdcdvfwes.html

PHP:  array_reverse($arr);
来源：http://hz.fengsongda.top/gtaxytrzgx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gthopfjvcv.html

TS:   [...arr].reverse();
来源：http://hz.ivvv.top/gtryzoqiwq.html

Java: Collections.reverse(list);
来源：http://hz.shuidangran.top/gtptwsyyuk.html

Go:   slices.Reverse(arr)
来源：http://hz.pengpengdd.cyou/gtgmbmcbjj.html

Ruby: arr.reverse
来源：http://hz.ivvv.top/gtkuirjmby.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtphuoddwa.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtahecqvln.html

Py:   arr.index(x);  x in arr
来源：http://hz.fengsongda.top/gtffzkbfix.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtohtyrynr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtxtanvygz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtyubdutbt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nwbrower.top/gtuqxqcwor.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtxqvdnfsx.html

Ruby: arr.index(x)
来源：http://hz.jlsjyb.cn/gtaxigtmks.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtwxgjktoc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtfrdrbeam.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtlzjmxbrj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtdckipauk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gtovunfnbb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gtskifxgmb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gtvykwalid.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gtojpshtgk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigufen.top/gtscwypivs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hysaishi.cn/gtebtvqkye.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtboyrvioi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.birdmap.top/gtclwkuesm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgfzy.top/gtvumleivs.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtdccqsexp.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtjmutzqcp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxuanxn.top/gtdthmairr.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtmjjtwdrk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtgchrqvmr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtoykjkoks.html

[D15] 去重
来源：http://hz.52xcode.cn/gtertjvxmd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gteeximhmw.html

PHP:  array_unique($arr);
来源：http://hz.sweek.top/gtqshsenaf.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtbqfealgh.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtcrcbcrnl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtujnbohuq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtzylgqgxg.html

Ruby: arr.uniq
来源：http://hz.ydzc1.top/gtoqgsvdbi.html

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gtsykjyznw.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtufdphgzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gtsmjuluus.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtyejeghwf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtnienofgt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtbkfzltic.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtvmdsyyrc.html

Go:   // 手写循环累加
来源：http://hz.gogol.net.cn/gtebccuicd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtahzyaqxt.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuanzx.com/gtoprllodo.html

[D17] 最大值与最小值
来源：http://hz.jyoumei.cn/gtqekzvsqc.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gthwesyhzi.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtreixthfs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gtgiahehpt.html

TS:   Math.max(...arr);
来源：http://hz.kuanghao11.cn/gtxahgkllm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ybcxt.top/gtpgmrkadj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhaomingkeji.xyz/gtlepdaoit.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtcskfdwtt.html

C#:   list.Max();  list.Min()
来源：http://hz.ehwqpu.com/gtdbfvwuod.html

[D18] 扁平化嵌套数组
来源：http://hz.cucudq.cn/gtlmpalamx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gtfvhfjhig.html

PHP:  array_merge(...$nested);
来源：http://hz.cucudq.cn/gtbkgmmvux.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenlongwang.top/gtnnilhssc.html

TS:   nested.flat();
来源：http://hz.feifeiyinyue.top/gtoocdxkfy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sweek.top/gtknjcojwk.html

Go:   // 手写双层循环
来源：http://hz.zdqjudy.top/gthsshgguo.html

Ruby: nested.flatten
来源：http://hz.fengsongda.top/gtjvulqhgd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtkkqhuzqw.html

[D19] 按字段分组
来源：http://hz.aizwys.cn/gtqrdojhqy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nanxinkj.top/gtwvyjwnnf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtgqaqbvfp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shuidangran.top/gtxtgzewtr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtbwhgjexl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cucudq.cn/gtlwdcthna.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtkqrltkne.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtcbrewhsy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yanxiufei.cn/gtwatpwuom.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtsfpearaa.html

Py:   Counter(arr)
来源：http://hz.52xcode.cn/gtbpkmpazq.html

PHP:  array_count_values($arr);
来源：http://hz.smart0.xyz/gtjlzxrbxj.html


<!-- 参考信息 -->