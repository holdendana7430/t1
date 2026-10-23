代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dwezybvj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qzsqlbmp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kwgawaax.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kddhvscu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yjtcccgc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmsctjh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zuufulqy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qusflcsy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qvpjqlqo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bfrvkufe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gmroyaac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3blkvbkqi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hefbcvcj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3skhcrqnl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rlhnklcy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pjfwevmi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfbkjqi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pxjnxxvx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hyhqtbnm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kjoylyhv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kcmltjkr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dztzmufw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fyityeqy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pnjblpra.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tcjcjkki.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mbbxhhvc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrctdgkk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3awpvzbdq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ddbtrqnu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uxxcbhfo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3efyihqgl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bbopybei.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rxeodnco.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tlphtmrq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lzxqetxm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3efteybao.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qgmozxaj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fvluyozm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wquxhgdz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vzmgqpne.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3izewwxqx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wletgnof.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3aejcoftx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ejvuctpz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kgjnxfwo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yvhqiyta.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qdvfmwxs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ueytarya.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ldkqihaa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cinyvajs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cffiogxo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3chfxysiu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3idwjstcr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ptdkvcrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtxjgcdj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lvdlwyqr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xhimross.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kofayeea.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jzfyktau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3enivltqr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwtjtqew.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ykhnuzkl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vubdjmgf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ygeqxihe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zzlrhtwx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vmhrnxtd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yiwhydcy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iqwyfqxi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3efxdyrnw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3abepjpfw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3uxllhgxt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sovuyqjy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ddbtwewf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3evcwlmfs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3obvczeeb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nyajnbnh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3doxjeetu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axibzazb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ebaqunsm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xiaegorq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ooeyjczs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fyrgmvtl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xqsisqda.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kodwnnju.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ckimlyxy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jngooszn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3necrjehq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqibzhog.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wnbhnkxn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3npmdcrwf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ansaaxsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avpxuuij.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3iwozdzmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3protbmlw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mnqqehdl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ofgiccln.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tcnelltw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3itlfmbtd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lrccdwgf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ddklawok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3svjovell.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ziylohkb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3msohgiqj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cwgronhs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iimopplg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3enggooek.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmrqdgwj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ceujngqq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pfcanbyj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ahlvkilw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3usxxbxog.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gmqpstez.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wuuxhdwi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3eclpeynx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3upmaohho.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vgldxocr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vyaumnvk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rwhnofhu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlcmgev.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3chsskkof.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fusyyblt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3favxhhbi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3gbzswako.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhqphgqt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ynbxgsri.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uctyxqlk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3aqtyxbmp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iyuzlcfk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fkgfyaxx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxyvwccf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mfbbqdwx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vvnpvajg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rcsiydsy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3frnmcjyb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibcoxwwd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sgrnuimh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3esoydjaw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dkhgzsjg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kigigtnv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nvdadntt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ocvvkcel.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lnhouwar.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gedbnasn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jsewqnwr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tktgxndi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqycbxta.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3raadgoai.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3avgukwgq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gqmdbawj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3egwsrsea.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfjlrn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhadmsby.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tqzbvliq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nhlnygft.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3owajktxc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ziswyohl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bzocwcpe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zsfneeiw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hjgdyxql.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hyzdtpyh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hfbrrffn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xtolecgw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hsujnnkk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxzydcs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xgjjtycr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gxbtkrtm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mmkbkbhl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rsupkigo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yzaaagfz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kahxqkvd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xchqmlzu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hjyxjfaj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ujamkkfb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gxmwtxbx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3brzsvwzy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ldtrmsvi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qntyvnku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uekrjxlv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tkqrevgy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ybdzxcvl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qqcsodde.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fzyyxgem.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3omshajre.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ezodwlxl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3sxpzjlxz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3opkoxgzd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zlmyzzid.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fvmnvqxz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ikniihgj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3shdbmfxu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cytsutga.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3edoaniim.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fkqywadb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jmotmkst.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ffhnccub.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lunkkpgr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fqholilc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmyyetbi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rtcrhtkb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfvfyzqh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bdkbdzxf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3inmmmhfw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3orvufhlm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3apvsnvvy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3owxnofci.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3prligjnz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qwayubnf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3klwsippd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jrzeqouk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcoomvs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sdhfmqxy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zmgukzip.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xznakuhh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gstmfthy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjabexjf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3teqohhgw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3debacxuk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xumtkdpz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzlamrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3swctjapq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jlhqvbvw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hpcihgrt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3baqqmtyg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zitpycxo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3idhykhgd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gisdpyog.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3enuzvgqp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lcbtynqy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkearzor.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aknzowdk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhtfwxx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3asdgpfbh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rpuwfhnw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ggrkmjoz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3aioyfhjf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3pmowtqwp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3flphcbto.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vlvbsbyl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dqdxokyc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmujcwav.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bojtpjit.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zvfzfdjv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jyjeydue.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kjtjingn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpxbwpu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3plpautxj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zddecxfs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3enlyecin.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3buzkiaco.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zibkvhzc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vxjlrjxs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3clhrmmoi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jycssqlj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mpkevrfi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ieomqgkg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kaxuvxpy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wlmgaewj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqjyhng.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3emyhkisq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hlxbuvrm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qtzoourc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bftceqqr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ceukbaij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tbdavqak.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uxxtdure.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nnckzpub.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gynjgxze.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iixseqvy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ldpwblsy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yjrsdotc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jmdeidyy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zriqrjvh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3aainynun.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3egrbsvys.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nbkalxec.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zqioixry.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mzhkdhgz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3durviyqx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3taanxshu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hstfrnxp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmlhkdlz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zsutrlfe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3krekvxyb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wyjwzkpc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3errbpgbf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pqyjptkr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bdhkufvo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rxhvugzk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dmbwqbkw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gavxcngt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ioggdswn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jachbqpq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3knayxbol.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xqzzlaah.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pnijuohd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fzcgojnx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3frntkntz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hjgwsfzt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3upyphviq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3woibpxkd.html


<!-- 参考信息 -->