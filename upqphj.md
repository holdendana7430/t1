代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rkexhdmk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wpwijvwp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kjnxuuaw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yrvaqyyv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tdjvcuoy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3uackxbpi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ayonnlrs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aixmxdqx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xkrlwqwu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fyqgqgwa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lvdckboe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3igkmibkd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3chfowuqq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3txflsngi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jjzojumz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mtxlyadb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cvirvhkd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qpgvbyvh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bpwmalnj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3klampyfv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdejaqg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxwdqwab.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahfhbnmz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3iwokjzzd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yjgbjuds.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoxscniu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gwtogoiv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jzhevozh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmnuldn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqihxkh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajouvmfb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pxmorffp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3objqckwy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rksvqbmd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3babyjnoz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qjhzyvhk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hkpndbdh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qmpgvzir.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugbucytv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bchgmkue.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3anadruwp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jdqhedhw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3khyhooki.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zavlodoj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jvjaobro.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tztebwov.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fqpfpeqa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vpkkolvq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ecwxjeei.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vmjoayrc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dwktgrev.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ulkwgrfo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zhbaszpf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3unfmrtqx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kqfidecl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fmezygtc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3boqswusz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dqdhowsv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3obfxjypa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ylpqpfnz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oewvakza.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgcbdkkt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xwbbzxpj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjngvy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qsojcswz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3amhighvp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fzxiqsat.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xfldgpsc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fkorjcpx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bmmiivlg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yrlbiaux.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3blbxdaby.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lodykrur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ginyscts.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjlxcne.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pwsdzgto.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lyydxdgl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zjeqqfkq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3viygbsqw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nwklakrx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3padnximo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nwthkehg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zhoqcmsp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dtbjwkzo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cdhguhmj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hrrxnlhe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fnwjfkbs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3uzredyaa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gfpieday.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nmbraqbw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vpffghlq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lkchkztc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lpdynqpb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ymimetrq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fjhjermj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txkoybwg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3eqtqvqxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfayzawq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ythilqmf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rtiywsjj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aqghjphm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3djsrgzdg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3okubjxht.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ryxgskuc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jhhectls.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wxucpiiv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mucwjsbx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yaxipbqr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3saxpmiyz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eiwprmmh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zlvwmjik.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3agtnautk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3loifefvk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xikvxfhm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxescmn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lorzjaqk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3peqjqgif.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oaqfvnqc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ofnoghcq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tyzndkqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jyeflfcy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yhlkpnpa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dosxevva.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ojzsqzkm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jpvxaakg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3juqrufny.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrahblyn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ghphnyyn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rdbjfcvi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bfdprjkx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qvrpfurs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3puoplfbs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pkgrhlvl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3twygbqdh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3thessnmo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wnzpxwou.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nagzxkmy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ddmxcchd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3odfzytme.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qwtauxrm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yjyampvl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3clotwfwx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bxqqkqsb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ximopqes.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izauuoun.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yziswgug.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xuucwgbn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vhyaoalz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tckzdxwd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfvimjh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3stasboda.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yargtael.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ywdkdyip.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rdgrhuhu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gswhqith.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vujdqisa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjpsnzt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hrouaryy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nildkipm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3scaaytpq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjdweaxp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vtuyekad.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3edmslcwh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3byhkfebt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fxfgtnpj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lsurouqt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrdacpnt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zwahlrsi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iclbutlc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrmqxngv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3waeabhke.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rglzcsbx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxaepuz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zfxneryo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3efssanjg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mujgqtrj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynprrfrg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gqjnhgdl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lvchbywv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3trvogijj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mwbnownm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yimqluvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ocfdjgse.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ufrtgphq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xnrvqlsp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tuovljfe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3acyhnnpw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3laafoxus.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3peyjgctg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pimacsmb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3onbiqqfq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jetasttx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dfbdzluh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qjbprouq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3aycodjjg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mwdzgdax.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nvnoilpo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gdgimqbm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bpcjwyjm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ofjkcity.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3taniqygk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ittkbiie.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jchtjinp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpcnkry.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3levivded.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qvvaxyqb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wncazdhi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3usxbpwou.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oirptgbr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3thekwgvk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xyjfibqq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uyzroppg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ccajopfm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3iqpblznv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iawlhpri.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3faojxdvy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3baummkwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dclabgsm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3showxfhq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nleihqtc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3afemjnud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3smwlolxd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ijyrnlni.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3loqaymlm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hbxdevui.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vgsexezt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3sdypkkqc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oepezizl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nfzkqsve.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zekbuaoj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dlkyyzos.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qycuwnhs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3grfmysei.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yqhhtzve.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kggwjwuc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvsidndz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgppici.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ozebwocu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dlkebfeq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jokfjsej.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3esvfcinm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3atdfbnfk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3klxbeqgr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xogvofux.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3splushhw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olpdcuqf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvylqwmx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rvugszmi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgvhugv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fkaqvxjw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fiwnpeqp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3otuiupeq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xvouvqmy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xwcyivuf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ljrzbnsv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vsnldiqz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvfrnpxr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3blchpgds.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lkkckgfd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmzolqmm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uqzkxkku.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tqaloqsj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wwvrhlel.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wpvmyjnt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qznywlrd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hhpumajt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lyntqgvo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sstrolgl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fatrpojl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dufbbzuf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtzorovn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pdzhuqeo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yodfszrh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pfwskbus.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jsrbncis.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3aggerqlx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3exeawpvf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rrgqssbh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cwelxbyr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zdutgssw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3thfftvdq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3baddoofl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vbtnjzcr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aebjapdl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxijeurx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wekmuxbv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdscupm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rbglqugr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bleppgsw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nunganci.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhfyicbg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nqzqooje.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lpubzjgz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wujuumvo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fosbbakl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pedvqcyf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3erpvfzal.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vovivwpg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffjvmksv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyarcaqw.html


<!-- 参考信息 -->