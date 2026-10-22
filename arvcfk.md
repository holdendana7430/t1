代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hslncpnw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fpqzwpjj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zugrqthq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rjgxogkq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqaslnwp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghbvfieb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yjvqgrwg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rssmligm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgwtnpk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rejhbfeq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pliynmbk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2htqspoqe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2voyxmcir.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ugqyrqlw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cwnyazhm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pftkmezk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qfhllvhw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2adrygjhy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mqlzfpbi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hzdhgcnm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aoaqmqow.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xrwkvdsp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zuelmdqq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kskslfmf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdpptrcw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gloynxly.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2alpbuhgj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cfkgnhyx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ovswaljj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2juijquoj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mgfpfgfl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pmgimqtc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zqtztmzt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ocdomkay.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ihtmvflr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wcscvzjo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2axwvnrxc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wfqrxbeh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wdsyhasx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vdyhkibc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bswmgjua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbsektdo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cquclmzl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2feacgrnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hbzqjmzd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2otvdoffl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2blpqlecq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ebipydru.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pvrsiykt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nchrqlcv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xvlskaho.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qgaxjfju.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2osfuiynd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2btlazcwp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yqsfiaoj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2owxmmqyd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2coctramn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcqqcltn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2neaneoyr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gnocniox.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngvaallx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vnlwboso.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ksluimbu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pysnsxxn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ixboymru.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tzlaxuwg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kqxjtkdf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2awzhyxks.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hvstaraq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2armgevpb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mmxvvuvh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qnnbnybo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ljilxcta.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtzhsqyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2frujhxyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gktibfim.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sqsnoqkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipjaotzo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zgymjbky.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bacekjrx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2djtvobmk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zonnqfeh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tftwvvbf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hmdlmspw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dgdkbgvx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ucxpptev.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mqcgiszc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fwauyrgi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hphvlkoa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vfzmdxjf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fdkvtdec.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wieyovnu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ylabzzrj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ssyhsovc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2knurmxwf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wdirxmyb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qaelejhy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qhymqkvo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vnjqxatg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tcmrixha.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tsgmagsz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lyjdfcfw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pjuglcox.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rlyfdsqy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jtqpoobn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bgywbudf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npvrpcwt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbnnzpsc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ildagpem.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2liemiycw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cxncxelp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uxufmilu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mbqroyrq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvevfdqv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iicjuphs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ucdhpnit.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ljfigxpu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vnrpyqzg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2oaaxfwgz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lghxzjkw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hvwkzgzk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hgzyxmls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pkknvylt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wzuhuobj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2adsknzfi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nbcuyklg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qvmduwsd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tukbehdb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qtainasu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbsyigsj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ikxhfyvz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tlvfwhmw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2iplnghhw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hxwxjvkp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qijtmhau.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hkunneuv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vjwnoujt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2movooswg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ljxufowu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dtyrhhek.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iceyhnjg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gkolqxkb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2shtdwjlu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vondtfat.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sldujput.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hhyomctj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2muutqiol.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yorzbfmb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jkfyyxgz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfqoahpy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wdyjsets.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jfwyvvzd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2cshfhgyn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cpxgjmgg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2chuttera.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2anilezrx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afuxyftr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sdzagduc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mzmqlbda.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2etjquauf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcflpsw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lfadcfkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ljaobmwl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zspimfom.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zohwnqll.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mioyhsns.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pasyradt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2clqjcogs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2szcpmsyt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ppwmzliz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vhtsiwtj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2opvefjtb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ptagjotk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ydxozjgh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wfwesmvp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ucznenuf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ikrqjddx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2axnbglwc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2scimzxbb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtpxhbuu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxiaxequ.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2otbbdowi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mwrirliu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2abfaahgo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxwzuie.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2onwjyzne.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gimezsiw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tozwoajo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vcbfidrp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqzgkoq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zpejcxae.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qdfcieda.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mgjocuwa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfdvslj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mqwdlqto.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fnrwgliw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jtdzyvxo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mfcvunef.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sufyudtd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yqdjljrs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnbmxlse.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pzvqmlnm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebssimpo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugjnrijb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lkmzzmqw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2psaishhr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xnqotwti.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2crmcgjop.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bpstqxcb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2uvkdqubk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gthsqjih.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jtlttdpw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2izxkufqb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nmficcqd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lejitrml.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xfhjvsdg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bpwxakga.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vnoguypc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kswjbtea.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2eyhgnpbb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xmvaksiz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2muykgkru.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dqhcrvgk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vadwvsip.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2axbtfaip.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgqdoaq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahplqoxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kwqtocnu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpbucqdj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hnjigwbf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2iqxpcxwd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2spczhwti.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hifwitbo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qmwvgegz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2onsilrlo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rukshycv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdebjmif.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ovguedzz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lkvcwfmt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tgseapue.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dmbflxmd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcpbywqe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rulbwloi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2swikxayx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jriltcko.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hcrxllbj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qdbfrfuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tvaohgtc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zfddjknv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ccufyfng.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjjzgpti.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ublcruic.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mceegifu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jmgiocha.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2psnkkamb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sjbkvaro.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fyfsyawk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mufaqoea.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2uasggigr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2spwjyjol.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xfiuintx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkeatluo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jupqodpq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olcfgbtf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2smenskwi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuyjdtf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iejnlkqu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uxkgctha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdzykcx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rldeyvay.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sigbhvmf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gzlrglmg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zvduhizr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rzybwbei.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2oohdcxmt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iglsxvsr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hmqgbxzf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhxnnmq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jamkcbyy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xgkvxkya.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2okclsoqs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nfkzcifa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2haeiifjg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pjkarkxd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kuetsfgd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tqjtwodc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dwhvcmle.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qotdmcxb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qqmnavek.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jcsrruzs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hiivogkb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2htenedda.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oyqtgwga.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lowydjtf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cptpppwq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lqlxpzcf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hfykhcte.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdpgduk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ebvnomnk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tljhcqkm.html


<!-- 参考信息 -->