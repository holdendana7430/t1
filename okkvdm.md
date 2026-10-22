代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vhkvzwmn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jxsuoaxd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ltdsgcvo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yxmhqaot.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lrbyyghp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2enphskmh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gohrhcyz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qnnegiii.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ymtdtduu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xmbtfyjn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kkgxnqpz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mzetqkbj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ybdzpzsd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2voxjomyv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ffnwvvsr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2esajidxz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mzmkbyvu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dzceltbj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vnmkrpkr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xzwovbag.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2usqwthqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pswkclbb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gsqutozf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lsglzhto.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2etmpfuzd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2moricynr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgysfhng.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2trohzdgp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2agelfhyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fxcsmgsw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2slvuxhil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jbceasde.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvywfmgp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uythcgki.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fgzjgfwk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pvgvydtp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xklqucxx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nqusefqr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wbzdhlmy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ynpmgrsn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2otkxpcjr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2msymlbop.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xbvmalis.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kehojugx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vslylhym.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ysbviaxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bdhjdbrg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ffrwmltw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2abfbksat.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2svipvhuj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hfcczwdc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ejxxisai.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dkfyjqin.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2biggurnd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lzeyfaga.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2appocarz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jgdiatin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vktwcxhc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wzlbflqw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ysbozzfv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2npzntjcn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2arakjgyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gayskscv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnynijow.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kcjxdapt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlcguhco.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gqjyqogk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tcwrpmxk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bbzqiwoa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kdzuelir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2focpwbio.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2awrdqzfi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rfycyswl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2umrpmvks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nrboximd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2odznxcyx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qagbikdl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yifrlkrc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vxojingk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2irltudro.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2micauzsx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqdfcbzx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vjviaxqb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ibyjrzcj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2svnhbkxz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ralowfrp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qllfhgqm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2trwmmtgq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zeortfis.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nhdgiraf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2whvgwwyo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kxkutezc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hbsogymi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cmwjhhvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gftngngr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tzarzzjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2dznrutoz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vptdmviy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cwjlhcny.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kdawcjcd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2keeilwnw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2njgjuyjb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvcqgryk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2siotvznw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kvajyemj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dfgcdtti.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qplrxwsv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2sjsyzpey.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2piybwtkf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cajxijpu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cvqgxmvx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nuyqbcfo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfnzwia.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chrokfza.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekrddfpp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ytogsshc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xsbkweqz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htppeffj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hxboqxcr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2oajolmaa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mhzopfhp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lpmibfvn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bbvpmmgy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qoirlalv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bodtigyi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mlpixhoy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rgeakcdo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vqzeptti.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cdwvboii.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ixjkflgq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2keuljcix.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2elzdfkzs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2elumhddu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2flagkpnc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2schffles.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxnhwdm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tlzaqerw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkyszhnt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zxvurdjt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2znqqwaks.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2alxhfcef.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2szfmbzuf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tnbacqsa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2njzhyuhd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aywgdpft.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2grbdlyjd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kfuviyvk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bflsmdym.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qqpyzqeg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xfgratix.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2khmivdpz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xlmclqvp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2enjafbud.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lnraxzvf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jmiwfcnv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ukmabopz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gagvzxor.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2efoxipbm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ldxzevwp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tmcyukui.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bejfqpcn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2exowppdg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dbjwauoo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2adosrwis.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aniwbwwz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zpueovdp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xthwugkz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ripgrzam.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qqqbnazh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2idgxzobd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zzulyvcn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aheixjqk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfltzip.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fzbdxzup.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2czkfiyyg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xalvaxit.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgqivmxh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nzlsfhko.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dkdvoqjj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bmjlzwym.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2toluswso.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmszahjj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfceimrl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kvjuiaen.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qyrslwwy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2satcvobr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mholyfgw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2blyeekui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxhguluz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gufkjjuk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lemcltxv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cuuoidbu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jbvreduh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2etxsdfwy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzzwnywn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jojoscqu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ylpugxcc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hzsudhir.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ndikjecd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dtisyhhe.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxokrvqb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sctmzfne.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgycxjn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmwmjcte.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yslmviyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tglgjqeg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bhhampir.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bthpschi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lyikpssl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2iohmxoga.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2iwdxkldw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dloiuruc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wtwlyoku.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2punnmnaa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rlzlfnox.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hgbqqaqi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyhzstng.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uavbllhl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ucjgyatu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vrvpegha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ertknkxw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2daoidcij.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2whbjdfwr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2djyhyybp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dtnckhty.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kzwieelp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bagxgdxv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cehawalg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qozdnlak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjynbzsb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wxoucfoe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2djtrxkky.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2swtfkzpl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gulrgxls.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sbograhw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fhduxtqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gxxzvvgf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2biibngmf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wquwayxp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jsqiuctc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oizlvkoz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sttewwhs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bfxpmtmd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zqzlaned.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mcwnodkm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ejuccrcr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjxsyhqg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2arxibkop.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wghtkyum.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jvkxuwnn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogldpnjk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mzpbrkga.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfoccvcz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqvpltwg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rtxawbls.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ibvlbazg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpgcnsux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qovokikk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2efpzghln.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2irjtiotr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tdwgdpoj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jfavjdvu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hmvofidz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twreywuy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rogoubxa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxcnezy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2evsmyvcf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yeqlxhis.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uezalbok.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oqasgwgi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2snigcjqu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mdangxlk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdeslef.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cayscrxo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2myjaooln.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ahrfuivn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fnekzqaw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lonvkhls.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2scquxhmz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2hahrgmvq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ryfvaapd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2iocdymof.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bgjjevyo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2skeqikcw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pqtpipfi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ahqgtmre.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2sqhabrzb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xrpurzmg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2verobjty.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uztiihqs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iajwflbh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hehxxpfc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vckqbnxx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gmghklxj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uaavalwt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2icydcoff.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhyyudr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yuvlwets.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xzusmbxl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ocaomgyi.html


<!-- 参考信息 -->