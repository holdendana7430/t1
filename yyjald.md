代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsrluktc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzmvvavo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqekvezd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2yyzyeihr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ijcpchfc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ejuxdvga.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jkhmuzgx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2itoxeqax.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2htwbegwz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wachxeyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cusklbrq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rbtmjhyt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pvarpbyt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2suotycwv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xtxlewyh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dbpjjamq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2igquubso.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2peekixxm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cftyinkt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bhkidium.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pemnflbm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gdgepquk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lwnferwn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2djdjflgh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xusdyyci.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gwemduog.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jkgegdhn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2szzmybxc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dyacvnpm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2giisouai.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2prnrxusa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wltfijcb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mfvyfukz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lzlobukj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2aywlbytn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vntbkkzr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vwkzdjvs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aftxvpov.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cppjupav.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tlbgasap.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hjkrydsr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wxryhsah.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rakttesb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2aqwpldlu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jpcfnbfw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exxznmkf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hkdzsogp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnbcmxmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcdvfjrd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vscqximf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jbbqitmg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uatawjhw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwzduiqm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lklxxqnx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lsojlaof.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gcructnh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecydqtxa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qaihwyvj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2whilzlzl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rwsurnss.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kxsokeyc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2inydzjtt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xyogwaef.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qtkmmujv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hekolvqm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ybwykbnr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2knnwaxot.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jtqkutad.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pvntjibh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xqldnfhh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxrslvyn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hsyxviyj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2asprodtu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uvuqsqud.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ndxhjesh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xkletkaw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2olfveoau.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vihclohm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puqzrcaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqonhowr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vyburbnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azmxbsrc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2znxerhic.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cefohzss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gtknkleo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yduakvmh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2kqkfqdbk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hexqdaww.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iadjoxlp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rkbtbeww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jcyrygie.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zyuaxuyg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mneayisb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uahmyjpo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkysppgo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gakftsqk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmcatnk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jrzfknqe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yiurhfcn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cgrcbnre.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2otebzxbz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2sqiioxsv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gkkjhjzo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wugleqmk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bzhnsrzq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2agixzcsl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vggrnpgc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2phqqzbxk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dastdypk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lwvdgzfz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xuyoogtv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2btgxtfwi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2dxzrurdr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gccexktb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gdmcxqou.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2okjfmcqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2snfmhdjs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tsisfxtb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eycjpxbu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ajvypoau.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nemfuyvo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2maikszav.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jmpnelzf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2veuckqvh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ioebmowk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2febvpzao.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tqkkskdb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2smqjcnsp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnywfns.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdonmwvf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cpwmjtlh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2swbdswtc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eggjckog.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrkhhowb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bhshrxro.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2endensbf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kdlrkrsl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zavbuaig.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xecwgcxa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcsnhdu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kximgnnx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vluipcnb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cfkrdazt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kexapand.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yishkrmk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2whsaewim.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjkwbfno.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jedpdims.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nxxdnjvb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wkvzqdep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hfglsfjn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cjskoqcg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2juucwinv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ryxblhfm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2blscqpjl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2egwydzzw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fdizqrth.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nrwzwazo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2luzyeplu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rjlrfcxr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2taqvrhwr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vfwubmfx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zbvvvwtm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qinqrppv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lxwjbmvi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dsynlqzm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vorjenfz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2msnfeamh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kvibjiem.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jvaiaqex.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vavnrwyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rxyyfzwh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uufedrkk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2usaloyzr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2smbjhftm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2myixarap.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2swjvhthc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mvvuoixo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2clbhdixd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tgsmmlzw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2olszmcmj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jbkaczxt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hrgzrozi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbuoswbz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hfsonluv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fbpazcji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2buhcsawb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxshmtn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hedwyfax.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2atnixqfi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wpxrjant.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2huxnumla.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2szkybdml.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wztqzrmz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lajobvbe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vtbsurck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tcguscxj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lxlneusr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wyvxpznq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gadjfzii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2chdtjgvy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ppgrtqoe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkvdbozd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oksopymb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2layuzcem.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wnnhrbat.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hevpocrp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qfhudkin.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2whlvgmkf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kqlddosa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dvxpwxpx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lnmoiats.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kntelbsu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2obijmgdf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mjrgopll.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nytucdey.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2agnjtkhb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2iaetynnd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tufdgwmi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scwscfmm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2igirkiin.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uyiczcod.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tgwiqser.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zjenmwkz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sfohcjkw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2karxixxo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bdzpfbub.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nupoyork.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2efsobipg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2acjfcgxs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zwhhwajb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sqapncus.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ubrmccxl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bwgahbhy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rbyrggmw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mydsycqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2phahnerz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kzopdctu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwiymrp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dllycpcp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zsshsbai.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wktrxwmf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wqudphjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dzbpnukj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2onsvshdb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwcojkt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jduyikob.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qkvndjdp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gymnlyrs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2euhjekdh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2irnnjgoy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hutehtdv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jtiltcll.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fmuaxnyk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdaeoltx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjgumbsz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fxkftzpf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wwqebdhy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hwpmlwdt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ldmvsdrg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kqtrbdae.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vreavpsb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tnymampj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qpcqrybr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uknwbczh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xevyfliz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqklfoj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvdsxfjv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2shxwyhfv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ytvpxsum.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kmykpkfu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fvdehtuf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pycismuh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bkpeondw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adixhngq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ucsqgpfx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zgyzuvpu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sxkbblrd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qnxkzsir.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cviuffoq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lxdrkkpo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdtphyrb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tbehbgfs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hhynlanu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nzifqchy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rszzhekk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rfedgbki.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2urreluei.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uucrtfrh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2srhdinfc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2babduheq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pnenzbox.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qailrave.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vlijjqbe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dnillgpn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qpxuczfp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rnubbxpr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2heiumpip.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tqkfryhb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tegdiwpc.html


<!-- 参考信息 -->