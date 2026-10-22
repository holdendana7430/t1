代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jpkczufa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lvjkrspe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwgowygf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ljjpangf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mhdmcmfz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dhypevyt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zuedarva.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qfiszdrt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ggkwdnsd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdtahek.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2smnuxryl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tsynqfqq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mwfoiswv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jfnvkvfn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxdcpfib.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hvnpjznd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rdfdtkjw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rxtuktsf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wfvuwnck.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gmniunyc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mtimluja.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwsanjmc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dwhqtbaw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fnkgtoew.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mhsplwmc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kdixmmkt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2brstmtyh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wlikfiyo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nzvdljgj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2veeurnan.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2anzelwyc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sphcljon.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2obhakdys.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2blwgjwsc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2glyhgsqo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2aqqeevpl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2roiqzzbh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wbyrxdaz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2roxatntt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wvzktmaw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rcorgipv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2tvmjnqxy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2inizeudt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kpswkcvt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pzyqiuiq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kcqmmysu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tjvcomjo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2kxyoffyw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jawogdlh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jngfmuag.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qpzobixb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cyyjfgeg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2owwucwvf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nnjkrbtm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jfbwlyrv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fvaiqgeo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uzegjapn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rkssblhl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kkbktuvh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ttwmlehk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsijguln.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2swnzbjmb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ruspnlwt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qwgmrmvj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dxmuffxt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pberqubo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ircqdcym.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gaooahal.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bwyycyhb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fzoqohxw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hkmebsdd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wcxlufae.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scvzdnet.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtoakdpi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ousykyks.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yjkltbbn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mgzeyavk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gzaogjxs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2byiivgvf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jcplujkk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lohmkvoo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tjznszgx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cfduqrjl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rwbjfnza.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dgyswjnt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jxgpjeux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpxvtisb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vghfsuew.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mtidyqhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pafhytoi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hsknyhqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2msuslyrq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bigrgcyg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tkpywgrn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bxbngtiz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2foictwwe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2eyurzvce.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nffrusmu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vvqeccid.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ogoefgzi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gaclvlbj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cpvrvkba.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dfhatoiz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mjqcqksk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ozobyjws.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aphxsazc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vunaxamz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2flmrdxhr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jnepkvle.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jyofkrul.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpecemkk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2epwkhvig.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kaovjmyh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wcgxkaig.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2frltopni.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yaspxvsj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2efgrnjso.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qygeevze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rmgktmva.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ttwjpbqa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vbhncrfx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ajavkfqz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gdvndoug.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ewigiegf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgkmsjs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gofnewlp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ivtvflyi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eulgxass.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nocctxcl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xqxmdvmq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrxuvgsu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fmjzozny.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lpqfewuj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aaubiyxr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jwwcyseg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ketowfap.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksyftnye.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ycszthbz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lxpsjrpa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rtoijopl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wnfbspbh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqdljbvn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tfzepgww.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qobdpisd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fwtyciso.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xqsrmfdd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hgqtmpou.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vtfixpfv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cuuuscxh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jqmmpcrv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2djjwsrjx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2byeedxrb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dazybiui.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nawsikeq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2azuzkbdv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2irgeznkj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2alcjhibz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ovuzrzip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glsugepq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kpbpxltd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzvrtemm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qofbuwoa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2evkxlgae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2joqgiffp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yzdtlqnm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2amrayzdr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zgpnguka.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dmtibnai.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfqlihk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lszqhaqn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ahktyxuh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vkkucelv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aioosxjr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyvmpogd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rqedlntr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2njxyosyf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ngrstpfa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2adsxuind.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fvtocihk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ooimcybx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2trnccuez.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ghhfxoao.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2teyqapwe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2razcpvtg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2povcnjxf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kbbzbnkn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rzdfuwdc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kchtlqfa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ufhunfxc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ygksbegj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2htqiupnz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vrxxbufn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxlysdd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kkopprcd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2brolgcrg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnnkfnu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhjrgst.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hmmknkgy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nxfwzqjj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bltmzqsc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxauwfx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nvrqsumn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrotamu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kmbhallb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ueiplqym.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hjzntkap.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lbicfeff.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2goegaocm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ojyeujli.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcmzhxie.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rxtoauhu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfogvps.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gixpompm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xiaoampr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nxcfargr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2encetoqu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xatrsitq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oxjzquar.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dwatankr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ylschrcs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pfzryfyp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fentkvwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xvgnnbza.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vjsyiynt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pcvxasxj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wzttkewo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2luyfltkj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxhmlgge.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2azncsjxe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2obukfwld.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sbfacyoo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hvhdrysf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cmsncxmo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qwkktkmr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sldvxihg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vykodtuw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qdwubudh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snyrgabf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2svoaooft.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cfsgdwhm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kebzlxhy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2psbswxux.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2uojopyhf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yitwuxmr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xxjkhynl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lauztldo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2tnsihbve.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fiwyjhoz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2glqtxwic.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2timeygus.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2leumzylf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmrhpolu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2niqigbni.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ecjpcrhv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yotecyqc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ztogfupf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ybymkdnq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2sybayite.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rwxnneiv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2oarlgwbt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdlmsv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hmwxtmax.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhdsaubu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwsatzzq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tngwhkni.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cyqyvumz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vmjjaarz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vhnruqpa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cojzjere.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lhbjgcaf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2acivqcuq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mqzywvqk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xgnxbdog.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unedtkmk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zeoojroq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tmsbrqye.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xplwueax.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdtbttc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpykmpvt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zwmligba.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtifznhe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2aetbupww.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwpeesz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hqjwfacm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2juudrqak.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bifflggw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qvoqbaui.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aqpgdedw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nqbtrmkk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2cbbpbhja.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tkfvifvd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yitrxbpx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2quraingn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2akhrrzck.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ggcipudg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xlvvsjug.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uzqwhlaq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xfzwaqzs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ewsmewbf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cnjqknqy.html


<!-- 参考信息 -->