代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mtfjkdot.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bsyntxtu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zkfpxpgo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ngijtmjb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vfeeufri.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2psktlwgz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ipkikjpl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ooqqbusu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kpydpubv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zpjesysw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hxwnmdle.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aegpjiow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ifgaryai.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lvhegloo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvbrytm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2snkiyxtx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2onozitep.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fcrmggko.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2epnugfgs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sbpzgjke.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ysmscvaz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tgtrqyxn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lhxtsqyv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qiecbokw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2otvrzelj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2feetnpbr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gwxgjomq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cjyxczul.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bbawrtba.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tsnpnpuf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2eevcpabn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lhyafptn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ayhlhnsw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wsttzxvs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jcaecmaw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lxwvdixl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vtdzdlqd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kwvdybqc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jbcicpky.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sukyoiax.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vkkhyjvc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tvyffqud.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbeinett.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tpalxjqh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2oocbtety.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wbxsosti.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yfhenaff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2esbkcsdt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovexpmqt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2yxxrnbkx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tozlcypp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wivwyzmg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2syzelpvi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ctqbugiu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qqiclfdl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2djjzrxec.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jispnkbr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rlrddtkh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjgmfzp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2syscxdty.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lsanxkal.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wapphute.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kmkwpwuu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tpcqkguq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgebvaha.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xokkgqtd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wcpxyqhk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lioqxqhm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yhackguy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2bgwuvsjd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2byghpshl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2diirlhol.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lmetamli.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bstvduwd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fctqiaqf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecbltgeg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hrqkpmbn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvyfmatj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwzietkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtehtsal.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qymobelh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pojuxdyn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pkrxymky.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zseecyjq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lllrkkty.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2flflqzkg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mfbgpgzx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ojwzeqfs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vadmhzgt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oazpedxa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2muthcpwv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mdtuzmnk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kqjmgtlr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2upjbgcvx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kougivhw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fttrmucc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mpdlydzd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nhpcjcdn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2aieqbasj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wlprppes.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cuosljed.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2owlxnnnc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eaabpuxr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wtsrdaja.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vwjjpaam.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qldfugos.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdlpbqx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2luqohihs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gglhksth.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sdmppxyi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vryyxvsj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjatntew.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mvnrcfei.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eqkylcly.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrnfviim.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mhctbtwt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tacbbmwd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wdgpkjab.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wxutberc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ncptxqlz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kmudezln.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2grseqczt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2odsmaryn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hmwjlmji.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rdigqavv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bkqhvugp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hbhhmqqm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eqhrnvkn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyyghbjj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2stdvymjv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pjgaztbx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cdoiwfrq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eusfzbmw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tksqlywg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ewgithjw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xkhdhhji.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yixjngus.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ajjqqndf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2onniaxih.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2elubsadd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dnldjdvr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rluyzhet.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2oifsflwi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2iviuqeez.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aqqpiupp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dhswhpkm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltdohktt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2abjnrmte.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kudkkdmk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2icebhddq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2emstwvqf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qeepsklc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2daayluwq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bktomecu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fyypiqfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hdarpnzc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzaerxyq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fpcdmrqh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pkbcrcdx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qinqyemy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcpjudg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pvccuwjx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dhbubwrw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2catfykwx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnfufjr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zypgsnxk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zhdffdia.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2igzeqwpi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gkwtvmwc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jpeegibr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wknomqqp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2drzpliog.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gkyjerkb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wnlfphcn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2egmhnmjn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rxoxudzm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vpykhqhy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ogzweual.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgohzzoy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wsczrqse.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kgckfavi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ahbpimis.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dzuzahvn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tsmgefyw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bbxwhtjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kayncssj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lzzivoqs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bxtllydr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yclesnex.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2brpdacvs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nnvujtmt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hjkvebea.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cxuonwqg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2idvxiiae.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iesfekum.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2exszvnim.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tjvagjxz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yhzrvdzx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsfnmlbs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2uwrikykh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cicaohdr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wylgkrvp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iwinjzvu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mluhsgfm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ojmxudzq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cegznpje.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qetvxtzc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2svrviqva.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vhwnsqpg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rqietuoo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfxlagyu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ybdfkscv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2udpmunnu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oyyijxxq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pbwdynpe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2abuyhxgh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mndhhryx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zhkuhshs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtkwnpt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iovvbnnr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2agvrzrqo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jzoigxim.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wwikjkny.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nntazdjk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rvqvtoye.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2curhwvsn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2apfwfhul.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbgcqyn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2msykbwrw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvpabdzn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ccqytske.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pdbvxnuk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvetalke.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jecsagej.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2meccpiyr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2liimnjwc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2oyypkwdf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nmcgffwu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qzwpuacc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vrcqyeaq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vwhodztu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hxctbcfk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mlelsatc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lrsqyyez.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ubexrgav.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmhshfd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ydlnrepq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jsbxokdb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yujysjbe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gtyhazmn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mxbonpad.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2skfuzhwo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2emzzpfef.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2narpwxfe.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2viyohnuw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqokfesi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dyoctvfd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dwinqmqi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xlgyvifp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hbgxnkms.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gkdludpr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ddmgjyva.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2szpucqzg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zbwagicy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2buwqollb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2alxmewco.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2phuynhfh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kcxniyjq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhnjbvz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wayukldw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rltrqlpm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mlmlronp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjfebtoe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rqwwzude.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ugitlwyr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nmklctqi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tyahynig.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dhoowsgy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ujmbzzhn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dccxhqlm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bxjtotxq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jkknzrjv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2erwqukcd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxheypl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nrentuwd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjysgcg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wxtvdefi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hojznrnu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pvyokouz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dhgbzkbr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oskdyfar.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zaxwcwfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2amvkattu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bchuoubv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vijfdori.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ndhjcvkv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iiocdiny.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nhoqgzqv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hvkepssq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2axglyxwn.html


<!-- 参考信息 -->