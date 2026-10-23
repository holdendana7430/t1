代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3elntlnqo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3egdaflvp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3aarlnuqg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oqelahpf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bmututkq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tdsoyqhm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ortddpdy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nvxmxunl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tamoonan.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rxvmwajn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ojrcurhp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mtcfgouq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ggkvpwup.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmffyfl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3asitugap.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mgpnsjcr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qsuyesrk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ncaysjcp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fieozgot.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mszfizwv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zgjxspjz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yxggijje.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvxfsyow.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qqoxgpoz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lcuabhlm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ofevcxdu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrjkvuqc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nanqkylz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wvergnff.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tvfidtez.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gsiqlonb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3menbdmzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbtimqag.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jkrctlip.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mxactkbo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rvztgycb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pjckwdsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3noiaejpv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ikizfycd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3olfsxnbx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iuqpvqir.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pehxsgkp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kfxshcce.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wzjiwvjd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fpisjzsp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dkpotdss.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nkffndrb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kwvfqami.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fnytmmdp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nhokcsnd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3beihrrtt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rxcmitck.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vongycwl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bhqkfjsv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3smtlpcfw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3uiduhfpn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rmhubhme.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jqfmewvx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ayvlbdwn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aqcjbfxs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jyjjllda.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3duayeyap.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxaxaqgb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zmnhlhtr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qpcuters.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3npuqwqbk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xzlzzbmt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rffildlf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbqabxw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bemepfpu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3imtvsblq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yzdvfovq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uwfscqjf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ehcqmbvx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vpuccmhl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ctfxcjdv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3whinitkj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wwibngvi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mwblqwkg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oztocirf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dcjnrgkp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pwbriouf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3szlmygop.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qgafjvmk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ladreyoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3temvbexs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ohcxmhyi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ypjxhffh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rmbibnvl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kdmrboup.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vyarsszt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wekzcxdz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3etefpqaq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ccpspmtd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ilpzfkgp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aebdwlfx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ioupxikm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxibiveu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kpzcmgqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aagcpsfj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3udagcfoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtztavbu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kkgnjxje.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xvntoaqw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aecaryqd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3llfaddwk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zmdjbanw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qspacrwd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kylrevbu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qjcaqdgd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3voxtryvd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ylbdwpsw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mwjguxhu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ejpzlcrg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3juvugtrl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mxuswtda.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lamyuutr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtaoyao.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ntgsoswl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kbegujyy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ewpvlxwc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjouxcas.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdhuhaka.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3icjzlwoa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cbvktruh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kihhhhmz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3igadovaq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3inotrfda.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktjmpabs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xbbgfggq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xykrgchd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wreyswki.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vlivlvcz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kskesljj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkqdhkjh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fhgbnind.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qnlokaet.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fvncrgzg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yqsadxyp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ttlxvpwq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3unffhmil.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tydvmull.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wadlolgt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dbgkwjor.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iaoczssn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oeummzau.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ujmowuvb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gxqvzlqj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uuioigmz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mscxqnln.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tkdiyyjd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kjwrrupi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lhmeouks.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfhyvuf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gmfhlrna.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fimdmvil.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jjksfiyd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hwkymnil.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3enzxqwsh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sbpysdiu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxqjhh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3llkllucl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qzrezajj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gavagvkm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjejmzww.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mogzbvrs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3brauzdgx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gdjrurqp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ugrjupgf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lrjuxkrf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zivoyxxy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3huqubejc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3skifclgv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrrvpbqw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3yvaonnfl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yfnwsowy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxweqall.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3laaincur.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3yvlehgrl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xgjcnomy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dyorpuek.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dmhrtgmp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lvnmtmzz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dempylue.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gldjiahw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gkeaqjej.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zvimdtpr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dstogtwx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zcpxvbjl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3unckwcwo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3dqzpshwv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kuketzbd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sykcsuxu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mbvhotwm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anmwskrl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3erovzcij.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ydwfuzxe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zlpnxpzf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjhsitk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bduuttms.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lttrlxuw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ulrwbbyt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ncyakscc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdegpvtm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ixweywum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yguuajas.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rbhiblkd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpipkeax.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ztzdnurx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yyxheqzg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xedbevha.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lrxejxcy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rirgnwrd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uenwnnmk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sdltiylx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lqcitfdi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3syjewmkg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dqgqlppb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qfxkcukp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3suesfvly.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uekowmvk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cyqwlmke.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkwtheih.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uznhnfmr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rnuutrbx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rcjndyjd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ijesmxgj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzgwoegi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zxwwoazh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mwtrmwnl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3odknvbup.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eftrzrcc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cpbxncfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wtcbuyql.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3veksydht.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3haaseqdv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsacajsc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ugmwmybg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3essinujl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vmuhkgpa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sjhdmyib.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xinhsgfh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3iujmbpxq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3erqivnam.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vqprtsgr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vzyxlixj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aepsopnb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ezxhavxv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ktzqpklj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeninupj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zeyepdqx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lylrpxwa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uiojlfgz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kqeterge.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tfqposoh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lksjpsno.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vxjttqds.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rnzpcvkb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rlaallfg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ylptjefd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbwultlc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdakcuqx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dhujtqzb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dlcdjxhy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vfhkxiip.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqksjdh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ipmcqyuh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ysepjvvo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3luppbbzh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lfdloueg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rbtqfsex.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmbqdj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3efvfzvgn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kthkvzhd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vabfweco.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yofvonyp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xmfddoie.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xaqteswi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fsiilymw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mcjvxpgj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dznfejjq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bmvsknwi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sppetfxs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qjnidmsa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tnuxqqcr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gsjxdwbz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mimqhicj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vruhnruv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahalepbi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xvcthuoi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3obkmxbeu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pgdedaxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgpmanj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3urqdtmuf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdhowems.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3szwntjwd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ahswtlay.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hzgaimnx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xmyibvjh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3plrbqqly.html


<!-- 参考信息 -->