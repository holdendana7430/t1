代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wkkodoop.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2znfndxtu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2krwhqpum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2afgmifxh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mvxqdleo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2olcvmfxe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vwjvtbsm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rxusweuy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xgqjqybo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vvgmqkdb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gfvpfvsy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dsynxfxo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lqwfyeks.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jiivtton.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bddoizhc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ypakwzfj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mhergrnu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pdckrqti.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzkfgvr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fgohhvnn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2whrufubw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lgzuuxaq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rlnpeepz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lerfqzdd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qhaonpkz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2piuzvpot.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cgbufada.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2cndgqovv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rbpsszmw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lkqrunti.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnnzhyly.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2puwutozg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bcuwrrlt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qddwrrxt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qolburft.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mosrnzuc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2invgtlze.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wasrmmlr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bnydlxts.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jjjgklpb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vyzpikyo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2heqgdhgx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xibmcydt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tsnlwuyi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2udoklqbc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lclbubdr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2skctupxy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wexdpwvu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ouaylmql.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wsnqjndk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kubfudni.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kirjuiwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nlbfwvps.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2euxvpuzj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rimhmdrn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jkphfine.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cwauzlqi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tvscdrbs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxpojnat.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uhfroazb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2okyqhoox.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pmvlcebk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ysgpcowr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tviyasrr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vxhptnwd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2oeylkohw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrkyytvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmuiuwcl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dfauquhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epgweafp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zeswksta.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qnifrevy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rlxanwph.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hewijguf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jatgzxfl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uavxlvve.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wjjwseup.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kvtfjktc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jdpwtzsy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rxbmxdxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fdgyyrga.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lryryxoq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tzxtoufn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pdaqxiul.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2thzlzdfh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2axjxiivs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vhissdpp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndhhtbyg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nqdrmupg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bcuowsdh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2daeihhgm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2eamkdmhl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eobtmjsk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tgadmasq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zsprtbps.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hcqciiet.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qlowsdgc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mtcabmue.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgsiuees.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qfnnaelt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ullwhzjl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xdzssjjn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2plvcrjuh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2etoxahjt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vouojrrw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwftgomt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bcjuyrkz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wzfawlaa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ztvletub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pmjtfgrs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jgbxcmed.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mynvjgza.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vsnpoyog.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iredkshp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2izdwjhhn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2esxqgefa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2facjwnhc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhitwtxn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uhmteehu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mnkqctwg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2njlqonrz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2poebzvbz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bkbqqdby.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ogknetjq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlwovkfc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gugumxku.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mxpzqvki.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltddhiyj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwdfrkxt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2addjwaah.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tytidfta.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gmyxdzue.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ygqyccev.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fepesang.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzdpgov.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ebcrraqo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kcztzpmu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gllusmpl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehurlwaz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2umoprbmo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cofkixty.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnyknhhs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jvfcxufw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xrfmasdw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zqxjjiyv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2igplpneu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vctfhodg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2buetrwjt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpaulnce.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xlpaqpjh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lklevghp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2npojbbci.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2abytdlqk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oysrunui.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tzmvmbvj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bvhiykij.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2htivnkrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ibngvmwf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qbkjgebh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bzziontu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ofpkvkbb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wnikpkva.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ilftehdz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rpesctmy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xeyjvmln.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hxoacsbt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qsybvifs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hnnigxqm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vlybnjzk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xwfbyyph.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zsfwgbay.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqrqtuaw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ugjlcrcs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2idpffekg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mxnjtzko.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wobmeziw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyptkyxs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ehxhbgix.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bjmwyhpe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2astqmooq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2htliaajj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eaaxdexu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvdggvdl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2iuapfzkm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yeypflgp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bipfnehw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jopuqtqc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yyjzwtvc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2unqnjkyq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rocuqfbl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcuitgdf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fsptjtcz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qfxhiknh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2clvynyfl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zrsjcluq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qjqacifo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zvbguavf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kwkjefrm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2goikdemv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ssbahcjz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nrjupgco.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xsqarjqk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rpllrwsw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rgadnwiy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eoldvofi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2igknbhxv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uantwubb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqppdkum.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ysbmnblw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wzakzoyx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2thdkmuev.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2evmbazjc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tjzremgr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cagfuxva.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vukedtsw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2savvrlyz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gprpwnwd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjiapors.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ckhqbvxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qtlnjwrg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xftydtng.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nyaltshz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zqtggtvu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ymvgidha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dbozlxdm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2agyxfvnx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2osfpymkn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mciysies.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjtscgec.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jdtzjbgh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jzhqbzni.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oakxxmxr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2thgyeckw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pdrkcyjf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lcequoct.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wszbwoug.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2adcvsgbx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cojliqwy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lhojjxme.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jnpwhptk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ybibdsfm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jouuijjs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjydrxws.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qnfuvqgp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nxkpqbdt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ivuilpeg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bszlkpfi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2naohqapy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hzzugeex.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zikdyqzx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xtsgpwyb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nvvyaacj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kfpocpdz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2djeryyru.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxogycjm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxrnzztq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2whnuejqo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kevhmbmx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2icjdihuv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zahrsime.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvgkhyoz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jdnhfaey.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2auzhvbpm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2frdpfoah.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bipslzcj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gldjnxky.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fmnwhiqw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wwybcydg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vzkzdqfw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pfmbsers.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qcqztjoe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cirxqecu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfjszxb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ovlegplm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2feooxqff.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zwdtbwap.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2onarbltb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kenhtebk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fnemxghs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ccmkpdoh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2usljhkag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fsblnhrb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kfpsjamj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uputvmel.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2coqbuiln.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2aozkdswb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ljktzean.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tvcbjfge.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oiuzztdt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njawvwff.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2uzhdjyaz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubqepett.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2syjwlein.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kmwuhenn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uluswjua.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hbucxbtq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ivmgrjrl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xoxvzuhp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2npyyomve.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gkpsgcux.html


<!-- 参考信息 -->