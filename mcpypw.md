代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xdsitlak.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dnktsdhd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2afpcilvx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yguodyos.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ntsfexgo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tdjwygfg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgbvfvu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sccvvesg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2znizryxx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2blokvgwd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2orcuvjds.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vavmxgqh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mfuuovzq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nnbwtzqc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mbjreeoj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ghunltwc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pnhnwubw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xunwjmox.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fnzdbkxo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rfzzmnxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2faihmbef.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qdkkawro.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bkyptmtn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yknyfyeq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awkczaoo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ouqwcsso.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vsgabgkt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wwrdsvlf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpegeuzh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rzwrfzmk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2doswwhsv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pjbgyndr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ztmdserv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ghmuclvf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2aaefuehu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lyneliuw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qofoizhy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jhxgbjbf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2teotzccu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uharuwml.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aayzcvwh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szwlzrng.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eqmfnziu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iwhdawhz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xdduqvkp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2snwcmnma.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2oggfiazs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xhleozfg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2isobfjsn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2brnejnqj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tnxjwuti.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxwlezcd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2sfqsqxll.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mqeyotbz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gibhyhrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czrqkqqf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pvmvtpey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2houevvun.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rxgnvtqn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jgmnlemi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bvhepbvj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2buyefowk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gjwegpgf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nbmjmewh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vnrjccfc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dhjsoyqt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lferxumg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ftcptqxz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2aqbuwnng.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lidgamta.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vsejnlnd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mdxskreq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gbcurvkk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dorbyhmf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rdydcwxt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mknpdbfh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2balgemrh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qdoucdkv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ptqvjbhh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kbqxmgeh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gzfxbwjw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xcyffvtm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2omwmskoo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dtpwidch.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2okujdzzx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2madvlfea.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dfrnwhip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zaxyitsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qwhfhvbw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hcmbftlv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2irvezawe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hsridwzq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jiogvwcr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzfthyyj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nhzdhner.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2unrtkjkt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mslfvstb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pglmtdau.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qsahvwtx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2temcxksa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2htmnmdsl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ywrefdea.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hdtzjisk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wnnlkdgh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvnioxrn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpevzlgr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tcvhwfjt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aprgxwcl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ncysadhh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tieqzpix.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2opqxaxoz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2toczualo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dreofamc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wsrxyrud.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lbcqnrsm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nrshaoji.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vpwhilfy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fmayramm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2imynkfri.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vcamimcd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwdhhvx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ufiwsntm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lvydrwpg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2otvtrbnl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2syoexwmy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lggrekaf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lizcaoli.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2afxemvmh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kqqqgfjf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ogcwijsv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lzqzlsei.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2chgkfach.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sajcgzff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qoeblghe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bdhhdobp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2axbhlauf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uoutufqb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2djyklcsj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2whgiwusp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2atyqjqym.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qpdyuell.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jzndztxj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2inmfzwlw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aobinokq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2watkxipt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2anqmtsci.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uaaxdjmw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nmdxucxc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2friyweyq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kvtkiyau.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2asjvvago.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kciokbds.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2alrbsatz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gbonylkf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmphieqh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fpvxbiuz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2neehnsuz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nyhamrvl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2giiealye.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wvsygzzm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijkwthfm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hcvxnzgf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2quwnwump.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpdapfq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2avlynynq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wcicnbvd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2akmlnlpd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2moqjddzq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xjivllwz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sdeknwqg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2teisqgxt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2iernvlhi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2huntxpjz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebicpbnp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwohdvmx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gzhjcfpv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fnbbcgoi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ykjudeoz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lfjgrblg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2adroplof.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xnvaamzx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tlwvnadb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fzdhescv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfnjeewo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2awqfkuan.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2svwehozd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvonclgq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iyjinbhu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xupismjs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bpgxnsgh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2facwuwtb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ellbqczg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bomkwkzm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hjfalygr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofyejova.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcqosff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cnazqwlx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nedlislp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2atsjkwfh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2apzljucc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hfdpzhdt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2strfapca.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2houqrxup.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvgficlo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2msdkrebb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jovltsgg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2onyqjrnf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oqcmvger.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snktijxj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vbcfaaos.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wafuwdya.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2plvbwhuj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2geeozduy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kkiyvznv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ryunfnkh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vxazyqea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bctgmjih.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mokqydpy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pigqsxmj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nybfzatv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jzyijsur.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2yxeqlnuh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yjghjjtr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uvuhlkie.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2atmkxnav.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2osokrqra.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kcqbduxg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2unlonxjl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hweevtus.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zejkakee.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xgwaumwi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cdidtfix.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qxvddura.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zfbubrbt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hgdkzepg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wvpaflsy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fzjlqxnv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2afrqejwf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dcklyius.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vwgaqjvo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zamkiaid.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktdewrfr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjjhilo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hffigdfv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2byxphxlr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dmeqoohs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2komizoqh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hcfcornx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhppffkr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2earvuuqb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnhzzapx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dfneouer.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wobmlfdn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gbaegwzc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2greqwbgg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xzceaxgu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xlgiskrv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hditsdry.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kntdmjxh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2njdmsgyb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mmejrxxn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyjgbrx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eeuawazv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2damocole.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2eipgmpup.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cgpqrpmf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2upwuhtea.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ndlmypkb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2faochzzz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sniiuwwc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pfttsoke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hoterexh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iqxvrsbv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uetwfsfd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2oaftfyxt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wfqkenkm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kmbdtwaq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gtidlwol.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ufwoukiu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gsghjlth.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xcrvmjue.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejhrhaca.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aklrsleq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2azczmcac.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2avyxblrj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqbrkpbs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qmgddtsg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gttsihxd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lgecoawb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qsnayjrm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ohjwxgqd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xstvblss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akeliekl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xpiqrece.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bisfkaoa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nprjbmpo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ywhnftzi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2idqsnhyc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ncchvfry.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2izpwckkx.html


<!-- 参考信息 -->