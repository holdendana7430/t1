代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.yvedp.cn/gtmfnvxvgb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtatbdjbfi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tian-w.cn/gtfzmnfram.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zycfv.cn/gtgfuglyoa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtdryxwtpr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuanzx.com/gtmjknssqg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ppjwa.cn/gtblzsglej.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtriouuvcq.html

[C02] 默认参数
来源：http://hz.wangdashe.top/gtexlgxylu.html

Py:   def greet(name="World"): return name
来源：http://hz.jinqigufen.top/gtfjcnhgac.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gzhubu.top/gtxcetbrbh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hammf.cn/gtbdmdhopr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ivvv.top/gtjfzsembl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtlnavqfab.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jlsjyb.cn/gtgrvhehct.html

Ruby: def greet(name = "World") = name
来源：http://hz.aibaodan.cn/gtolbcrvxw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cucudq.cn/gtkhrwofjs.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtmsezyvkf.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenlongwang.top/gtipiyucev.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cheryme.top/gtmxugzxdc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gtuqrjynuv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtlwoknucz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtiouzekus.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinyuanbaomall.cn/gtdpfqfyis.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhaomingkeji.xyz/gtdftbzlfr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.9152youxi.cn/gtiwaqnqhy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj20258888.top/gtsmfyduph.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shzxlz.cn/gttgkbheoa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangdashe.top/gtzuctdbum.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xylfe.cn/gtplqulvvj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtwaecnwhh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtqzxmesvh.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenjidiqi.icu/gtqihizqdk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtonziobya.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtlkewxifz.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtngzeubbg.html

Py:   return a, b
来源：http://hz.gogol.net.cn/gtqysoijtz.html

PHP:  return [$a, $b];
来源：http://hz.zhaomingkeji.xyz/gtmjyuljqi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.bjfxy.top/gtbgxkfyxf.html

TS:   return { a, b };
来源：http://hz.gaohongyu789.top/gtyulrepky.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gaohongyu789.top/gtmrmkdzau.html

Go:   return a, b
来源：http://hz.pycfn.com/gtbggtjper.html

Ruby: return a, b
来源：http://hz.jqgfzy.top/gtkdpfejnw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shzxlz.cn/gtsimbnjbr.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtpdhrsnoo.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtcbdfculo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gtmjkkqggg.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtndaevbpq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gotoacloud.top/gtbvggwmgb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gtsmkghdiq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gtuhtgvlex.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guannengcc.top/gtentzufor.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ehwqpu.com/gtkxrnqtkx.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtrfvxhttc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gtqisqvkxh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhixingplan.top/gtddamnqbq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgfzy.top/gtdiybrirp.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gtvvbkguox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtlzfdvlly.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jianghu66.top/gtnjwuuoxg.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtecoiyktr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nanxinkj.top/gttimxybuj.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtzrcocgob.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fengsongda.top/gtnjfhuucu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cheryme.top/gtoekolpec.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtsfjlpbcm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtckwuromr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigfzy.top/gtbposgntg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hfpthk.cn/gtpckvpirx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhixingplan.top/gtpfaykncc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtyjfpyueq.html

[C09] 递归
来源：http://hz.9152youxi.cn/gticvjlvdn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtcfhltudn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shangyingyoupin.top/gtaisgiukw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtmazjvkgl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtaguqkmaq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtbbrrydbe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cashguo.top/gthqvujhfj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtcuqhnvnv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj20258.top/gtjfowpowj.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gtmthfewfi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtgbbkyens.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydjk.org.cn/gtkloflvyy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258888.top/gtebjjcbfw.html

TS:   同 JS
来源：http://hz.kuanghao11.cn/gtjvwdkafo.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtshvnggjx.html

Go:   花括号块级作用域
来源：http://hz.nwbrower.top/gtgxqhcthh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hfpthk.cn/gtriddkbqw.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtsepimutg.html

[C11] 模块导入与导出
来源：http://hz.dashuyun.cn/gtsmynpkih.html

Py:   from module import func
来源：http://hz.52xcode.cn/gtfrihqzpu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhoulong.xyz/gtwrubyqvj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gtzyxzxeuv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dianchejie.cn/gtiycmkqyx.html

Java: import java.util.List;
来源：http://hz.zhoulong.xyz/gtalnqksal.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtmddauwlp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtpscrstsc.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtibbwsamm.html

[C12] 立即执行函数 IIFE
来源：http://hz.xinyue.icu/gtcxbhhrdx.html

Py:   (lambda: print("run"))()
来源：http://hz.nwbrower.top/gtukebwkqp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258888.top/gtiuovocko.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtdjmmuzul.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtkgqblknx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gthlalzhmh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gogol.net.cn/gtohlpdstq.html

Ruby: -> { puts "run" }.call
来源：http://hz.shzxlz.cn/gtlyqxzkdm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtbqvbzsyu.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtpmvwckwz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ppjwa.cn/gtpkzhjegg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtqllxbnmd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtccfuarml.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtbrokfxbq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtcqniyjuu.html

Go:   func add(a, b int) int
来源：http://hz.zhongyouzk.top/gtpgolwrhn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hysaishi.cn/gtsullvyfd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtvmpybufo.html

[C14] 泛型函数
来源：http://hz.birdmap.top/gtakiazjxz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.fengsongda.top/gtiskoqgol.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtdakzvemy.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtrxdcbuse.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258888.top/gtngmrixch.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuanzhike.top/gtsekppyee.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gtzjrzrrye.html

Ruby: # 无泛型
来源：http://hz.nanxuanxn.top/gtvqjvnuxa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtnlsxitmu.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtlpvxubby.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yanxiufei.cn/gtogyolhnk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tanke756.top/gtrznyupvt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtkaesxcvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gttzbfycge.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gtqlsrfbyj.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gtonnwnown.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtegyamnqy.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gturjdcqgf.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtkbzpulon.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxinkj.top/gtipoejnsa.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtravreeqb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nwbrower.top/gtzzirynpl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtnyhgkyfo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtjgiqjlhw.html

Go:   // 无重载：用不同函数名
来源：http://hz.ehwqpu.com/gtuimbctwf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigfzy.top/gtiqoexmme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gtandjqdtb.html

================================================================================
来源：http://hz.jyoumei.cn/gtwnqdoaia.html

D. 数组 / 列表 / 集合
来源：http://hz.sweek.top/gtdrammroa.html

================================================================================
来源：http://hz.gotoacloud.top/gtnjbxenza.html

[D01] 创建数组 / 列表
来源：http://hz.iojbl.cn/gttjysgqmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtveakvekf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cdnleiting.top/gtuoismwia.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.redwolf501.top/gtehuznlxr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtsjzggzhr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jianghu66.top/gtmmyyscdm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nwbrower.top/gtxqkmnxqi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtkifytutt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258888.top/gtnbzkwcmg.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gttrjcuvkd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinyuanbaomall.cn/gtaoakzwgx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jyoumei.cn/gtbpmcrexe.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtvmhwutuv.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtuboaehaw.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtcvazottu.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtqzezlrkp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtefugcfaz.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtedmssavo.html

[D03] 在指定位置插入元素
来源：http://hz.redwolf501.top/gtdfsbkgpm.html

Py:   arr.insert(0, 0)
来源：http://hz.xylfe.cn/gtcfrteack.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xziqi.cn/gtltwrncsc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtkwrdmltg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuanzx.com/gtdulamztj.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gtvsrywpoi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtnnnewnlg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtkxipucib.html

C#:   list.Insert(0, 0);
来源：http://hz.ivvv.top/gtibadviti.html

[D04] 删除元素
来源：http://hz.chenlongwang.top/gtikzgcpeu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shangyingyoupin.top/gtaqzljlca.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gtazsdisxh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtzfjigopi.html

TS:   arr.splice(0, 1);
来源：http://hz.iojbl.cn/gtkogdamra.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gtcezzgliw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gtncnigbam.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtypqmivfh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hongshengwenyu.top/gtkualtoxe.html

[D05] 访问与修改元素
来源：http://hz.ywan-chungtsiang.top/gtixfokzrr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtnxzctllx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtwclzdkcs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtjzgylamj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jiagoushi.top/gtuuhwixqc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtxmhsrxme.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtyixtxckr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtiqpxcpny.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fengsongda.top/gtobwirlwl.html

[D06] 数组长度
来源：http://hz.jyoumei.cn/gtxjvvywhv.html

Py:   len(arr)
来源：http://hz.nanxinkj.top/gterpafbph.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtxbitfdxn.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtsaodiyfk.html

TS:   arr.length
来源：http://hz.ydzc1.top/gtpywayppe.html

Java: list.size();
来源：http://hz.sweek.top/gtvxdnpkvz.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtyfjjcfju.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gtbedvrulb.html

C#:   list.Count;
来源：http://hz.birdmap.top/gthggjoeob.html

[D07] 切片 / 取子数组
来源：http://hz.9152youxi.cn/gtyiyrpsga.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ywan-chungtsiang.top/gtafvtnrwf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cheryme.top/gtxxikonim.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtyygwaibf.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gthktqhpjw.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtuauikdkg.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtluivjqdr.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gtlbdmdzxf.html

C#:   list.GetRange(1, 3);
来源：http://hz.haohaochexian.top/gtgangjvtn.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtuqokfzqi.html

Py:   a + b;  a.extend(b)
来源：http://hz.ehwqpu.com/gtbburqxbw.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtabcojcia.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydjk.org.cn/gtshdmjirl.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtqhahanjj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtijrxdipv.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtrmrdavnm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gtjagribax.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtncnmexrm.html

[D09] 排序（升序）
来源：http://hz.jinyuanbaomall.cn/gtgcxkxwzu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtamdxcdia.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtsolzdgdx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.feifeiyinyue.top/gtddypnhes.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtadkulpgb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ivvv.top/gtuayklqtk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtbbnczrli.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtpsahjodp.html

C#:   list.Sort();
来源：http://hz.yj20258.top/gtocprsess.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtwixxkyqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sweek.top/gtomusizgr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtppfhpkgl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtsthweyeo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtetxlthhh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtggemwrbg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.wangdashe.top/gtmaarytyz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.52xcode.cn/gtgafarxie.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gthjdgxrsy.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gtuhauiuui.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgufenzy.top/gtkxsnthtd.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtpoelggxf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangshuangyany.cn/gtkpgjmoys.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtuqnhxjeb.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtvcqzwlgw.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtgxqauhhz.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtljtwprjq.html

C#:   list.Reverse();
来源：http://hz.ydjk.org.cn/gtbqxsxuny.html

[D12] 查找元素下标
来源：http://hz.wangdashe.top/gtdbeucybk.html

Py:   arr.index(x);  x in arr
来源：http://hz.redwolf501.top/gtmozoinfq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.0kj1m.cn/gtpkfwguhz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtvwtiwfke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtiybuxrcd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shangyingyoupin.top/gtlkwhfiyz.html

Go:   slices.Index(arr, x)
来源：http://hz.pycfn.com/gtxaandtth.html

Ruby: arr.index(x)
来源：http://hz.ybcxt.top/gtwkdnofag.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtoldthmwf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xylfe.cn/gthsgvpqhc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.kuanghao11.cn/gtczjawdta.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuanzx.com/gtjvhfuqku.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258888.top/gthugmtzpv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtjylvyizq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gthtbhfhhq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258.top/gtskywnppr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dianchejie.cn/gthwcbxohn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtgvjcvoqi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuxming.cn/gtjsgbgrac.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtlbaninga.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gtoopipown.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtoyvgiwex.html

TS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtbcyqoyaj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ywan-chungtsiang.top/gtbxvwebht.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtlloslkqq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.redwolf501.top/gtaowrmype.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gttkjnrzav.html

[D15] 去重
来源：http://hz.hammf.cn/gtppcvaqli.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtfveepnwf.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtbwxytwin.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtrrnxtdyo.html

TS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtpkkjewup.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xinyue.icu/gtnkdeytxj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtkksgtovc.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtdqrrgbud.html

C#:   list.Distinct().ToList()
来源：http://hz.nanxuanxn.top/gtrjdxllng.html

[D16] 求和与平均值
来源：http://hz.svipenyu.cn/gtggvguefo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guannengcc.top/gtpiajayqp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnxiangtu.top/gtxkibypxn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtohaxlyvd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtfpkqyudg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtdvcknmwh.html

Go:   // 手写循环累加
来源：http://hz.aibaodan.cn/gtrorzjgvr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.andypj.xyz/gtsxseyxkq.html

C#:   list.Sum();  list.Average()
来源：http://hz.yvedp.cn/gtrrokedmg.html

[D17] 最大值与最小值
来源：http://hz.jinyuanbaomall.cn/gtlrqyhvfm.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gtxydtqvqx.html

PHP:  max($arr);  min($arr);
来源：http://hz.yueranfly.top/gtauzoexdy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinghuilouyu.cn/gtviwrlsjc.html

TS:   Math.max(...arr);
来源：http://hz.snrcjt.cn/gteuvzqmzj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtfjswdmmz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinyuanbaomall.cn/gtnyvsrqob.html

Ruby: arr.max;  arr.min
来源：http://hz.chenjidiqi.icu/gtiomzbmzx.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gtcnaqtwcv.html

[D18] 扁平化嵌套数组
来源：http://hz.yueranfly.top/gtlurplztf.html


<!-- 参考信息 -->