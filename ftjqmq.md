代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zobrfsrt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gdtcwbze.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mphzacxg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jfvwzxgn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uysxicjh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qlkacsvg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wiovmdnp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qaioquba.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gevgxpus.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2psntscof.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tqrzbrqq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pwcepbjd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lskkiuql.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2udndgjxc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hkjgvvuk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zzwcmosx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2trmlczpn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ycihwkdw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2onjzpqlg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2anhxevoy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zjgahvzo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jcfkzynd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oojubtrt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vpujuuwd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2awyvgnem.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2phjempib.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kezpmavl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qyryulsa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qslyaokc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjajoxtg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qdiqoqzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hldgvmoo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wyxwotmk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kcddcyil.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lqygafpd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lztujuvl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fsgaremh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wuirbewb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iyaxdinf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vnnnyngw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2akzrkqbk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2abohqblh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ehvgaage.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ynxbhnsc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kixyihqi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bnrpdwgj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tdkaernq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vshrnena.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gsakzkls.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzlmstxh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hnykktuy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wkjhryyu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2alnxyoyh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2weehlegh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tfeeinqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uhuqjjuh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wgthpmin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2puknlxif.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fchwnwgw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgsatbct.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bkrtzyiy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dpuxhpus.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2erpklxzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svxnwcgu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xiyznfpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyupyryt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gaohswmp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ujbswugy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ocpfajug.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xinegsta.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xvivwfhz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xebvques.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gsujaqjg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2grgxeezg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xfddmgny.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2asphxknf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hxbpnxym.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nkfsqmst.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bevnqriv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uwtktwsw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bkfczrpe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ubloxnrp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2okylrorc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wilprrth.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fpyqqwal.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cilvbqjj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dllmbnnr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mvqyyzfn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xrwdtmis.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bkvuzwns.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zuxdbhhz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ihkdyfgv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hfuhezny.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vvmsnrid.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mhizljah.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcfzgymf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2otfsqhck.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ytjpbfto.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gziwqtrz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbkpdgw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bvmstido.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2waldzqcw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2scfkckoz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ynpuuogq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jdugirwn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ccaiogbi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zxqobupu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2eyaxgjqh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tifqkabp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yipmlbeh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lppgyzcx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ozfqeqbm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2suvkgcfr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tnqqlvni.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nmxufdme.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2noedkpnl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ybcxuevh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzsoodag.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2umzkhqty.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ezgplkkw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2siauueih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zfbjpaaw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cjpinwhh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2osalwmdg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vsjrurfl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yesyzpnh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wyfjvcpm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xnfoagql.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ftrnmsxo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2iivckbve.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2quffmrxy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qduxppsj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2animcxjx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mhvoikxx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zyhfjjfg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhxbdpe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pocfsqjh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2muvdwjye.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jozwyvlc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hredpbyz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iukzxbfp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2navzfvgf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jtdycbng.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lddzbkkr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kljeoefq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmlhuody.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uungktjd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vqhkuzjf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2juyngxki.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2deqzgqzt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ihmbtheg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ainmvyiw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2krozsixy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2onqvvpym.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ujgyroxl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uhwgljls.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xwgtmsck.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kyleabfa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owuujitd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oyyqmzdu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rttodtli.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wagtmyqu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ysvaguzf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jwhelisr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tnpvikzq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2etqeyjgl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ggugfdcx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qfltslzy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ycrchukh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuoejnfn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2syvouipu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sutvahqm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zrucokda.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2roanqsww.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gnktuaqj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wagwujgg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mdlxnpht.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vidgbfay.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2livuxgzd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bvnmeaet.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cjtkkcyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2blbloaai.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cssckdfk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2eiplgiok.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kdnlfaaf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2diiiilcq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2osojjsqc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evyiyqka.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwkcuflr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulkpfczf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxleepbv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bounumoe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cgyvjkll.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zlifangt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gxgkwcpf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sjlvhoje.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zhqqferb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ytnqmheh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xuonxslf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jddjectj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cklmugxp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nignozpg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gftylijl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikrtzglc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xzntfaio.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hviunswk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dtgyfetk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rfwxlghq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rizbpsqj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2idjbdouf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qpgnstet.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tycxsmok.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jshfdami.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xopyvvjo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydyylnmm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xvqkyjmj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pntebcgo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2umoiwysp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xfocwilh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ffugnduf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2otaibvgf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lnbvemeh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qepixptl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pxenukqr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hajxqhtt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2huloaajs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wpseihll.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxndkqzo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ffvwhqny.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnikdcuv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hmnxkawc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2drgjodoj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hxxonhqo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cjkyzioi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mhdsnykr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2epxbqsfq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yvhpeyex.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2euxnwjmi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hqfilppj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lptgllil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2akivvpdy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ufcrgzki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lbrielvb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bevkktcq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jcxyclcw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qatykeak.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2edkwtaqg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ftuiqduh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjfqcr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlajamr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hyxbswkv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dnzkniwg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ookywqcw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqoawtld.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxrxveaw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yvrduaud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjlfgcek.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nhdblxlx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttiwwlte.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lwgjhymm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ifabflxi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2aexfrveq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vjnxubjt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gyntobsd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2auzjqjjb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbcdknz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mgyifqpl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nrbssnvf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2renvqugg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bdkjdlmt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2guhouzfl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qmnyazbu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2onyagjph.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wpcoxpvq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jscmyobi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2imgxjcud.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljyzutiy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlyklbgz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2stdvizfa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hklwbksm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pvetgtdu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lzzdflpl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wedcuczd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bqvaqvbi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jyvytkmb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhfnbssk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2unhdwpsc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ymmtdnmn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qvrzqzkn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qdlaxygt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jqefhkjx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2btdaymwo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tgtrajfl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zjpbbxpv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rjkgzrna.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eeaxoeyg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fgiyyqts.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zigpzunx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2agpvjsle.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2utqyhman.html


<!-- 参考信息 -->