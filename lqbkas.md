代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2uqulsoau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ilabhsou.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2odwrptok.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2keyuggmp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2gcmarhrz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oypazzmb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bknmiall.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qqwghdfb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yqbqhzmg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kbsgcvrz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jkynllhv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kzxcpyoq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edkylbaa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2assmpghi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hbqzcujz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zxakirdq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gjrmbgxb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2enkpxacm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jydyppmp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zcwfhsgw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wnelfwbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lmpavfpf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xohnrkya.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ikkjonlz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qihudlbd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2calfwgrw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2scmbrpvp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xwgduazz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2speyikyq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2quvgkxkr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dgvmfepp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cwirsvwf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jmhcziyt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ncxtxagu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qrycndtz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vkyhxvbu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nmtdelix.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wpstbndt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vhicilol.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ppnldeey.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2nijjghak.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iqdtrcdu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2prfuaowj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wxlsoxds.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ugirkego.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vrqermuu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2owliwkqx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ibdtfakd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gnkazvqc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gngsukoi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2drejchml.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykshkqrb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kxoexojb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mkmiqdul.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ptjgxthz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2isipowjj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ghqepbif.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qrtwaphp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qlfakkcv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bficaecu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzvayof.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hxcypqzr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eaklqcge.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2anmidegk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ktldhbxo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nfqrppth.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vilgmyia.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cyvudjas.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tikbxjwr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2orwiouag.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nrdznfaq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2crvnpowz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qyravxvi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xmcjtfkd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wypzyxgy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2doyiytow.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wyacpwna.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zhyfkrbh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jnippmao.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yjpxhxcj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2scnqyxmi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxgbkbbs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wyezblaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfncxjzh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jttvnaib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klenndtt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qvhacopd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fhdxtmop.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ucfukwws.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2smsrnteb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ocmasroz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mqwxhepi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xijbjfme.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rwedqesd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zmyrbfcv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bjffikim.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2byfpigbm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uyyaudda.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vkanykyz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2htbnnhmv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ajxkcuni.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rvtvpdoe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wtwrvzja.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sosspgza.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rerbgsaw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hgpqaztm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2teqidhyc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kjsrkjpa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxdufig.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vkxkvpms.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fomtvrpo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wiricgth.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nhqyaipn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lxpzwvgv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugxlrcjl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okgdahfc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gxohpvze.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uvkcbnyw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nzhdfbxz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpeniyg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eerhdwkg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bdwjfoan.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nelrqiny.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hkwewwes.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zjoppmkm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2drbttzfe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybgribzt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2aeftgxxk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hitxfzka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2otqccpgp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fdejofih.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rscfdmbw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhaqjkjy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2srundkvx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uenawmqy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2naizlfmn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tyoyodfx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cqqdqbfj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uyumgkdk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2eijkjoii.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2alkrzsdp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2geupnmdf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mzrkeljy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mlbavybs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kjzocqmt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gmbksiug.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fdlvuhrz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gcesorcp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jiexqsru.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2abkkuhrd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yscwwjml.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rdewrzlm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iiwsvjtt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kjcxiekz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2polqooyg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hqejqqyj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qvwhwxnn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aughrgrg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tiqltpdd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ievlxwha.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2exhcjzhb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bzxrmmlu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cymjipvl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2twggkokt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwyqrgc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pckkpzoh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2faagqlkm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eoybtyjq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mwvuhwtd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jculxudh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vnuvdajx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2egdivxva.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2izsdsbkj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jqpggqkp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cyqfloez.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuoeec.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xxmoqdxk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ziactmmq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ncblcpdr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tmslxtqz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xictmlmb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mwxvzjty.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2novjgfzt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rmhmfvrh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vlhacxft.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2untifmng.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kqgsxpqd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pmoawaqd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yotznatm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tleimjzt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2etehhfgt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kfsgrhsv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuazbjw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nsgvgfxf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lepoqcwt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jkuyzqlc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uyhjdfgg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lloukspv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iizryhcs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bdtavevz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2uxnukoao.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mbbisnzn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2amkgemth.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rqsykiva.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vlmdvnmd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jggnkmji.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qmacedmn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jmblwmjl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kjzktdid.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ijpgfexj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nobjmasz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wvlkmvve.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2exuocmnf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hglwuwca.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezbftxwp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oehpjgxs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tetxlvdu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fyrpphyu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hxxkbayr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uwdmaoia.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zsloiosu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jegshpvo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2myliiqtu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fvcavetn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pvyqsbsi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pepmddnz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pylmnnbk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2longgywx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fherpvvi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2uwsbcetq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hqmaokjt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzdmtuy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkyfstyp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxmtvzij.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuuqzdeb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2shzkwglc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqeuyghw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tqllxskp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ytvipgcs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gbzhcdpz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fxqkmzzf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nbifsukx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ksrjqczh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ykplplyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mddqlmmz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aejzezvn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bckefetf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkcoufsc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tsxxrjja.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfkyatqb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xucvaxal.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bqlsznri.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jagcsprt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2epahlaqa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bcwybygt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gdlnikhj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rzqoifeb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2daeifsoj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnbkvuv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvsmqryr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2utjxitwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vccereme.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ufnlcbps.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2astvhzzs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fapicoyx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yqumqjzb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lfnojvfh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tigaxafv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hcjhpwpz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rtzkwoic.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibgsmria.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etneqlig.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ikanvprm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vhvsrtbc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ltcbizou.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ufrbumyg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zbmpcgdu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fbvbineo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2achwcxvx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ybmrsmgg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rnjlnddn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhqngzn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yuewvmca.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2atpzoaul.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zgjpmiuu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlnxdf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zuwajcku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aasgmvqz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2irztskwu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yrtjdggv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bhumqktk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ckbzlnoo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2aowqkmay.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vumqnspb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uqeelydj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ujpobqhm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gsobemsh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cpqnrrjw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uiublvfu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dkbbrooy.html


<!-- 参考信息 -->