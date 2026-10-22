代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ibomqgdq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ytarvyww.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2esvlhwte.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fzaevwnq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ibgsdmfb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jtgrmdrt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lnpqdauc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2urafwora.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yawhoogv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2eqwhfvow.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2sgablyuu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vvsyzcow.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aqhokorl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bttnxmab.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2sqotmput.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2llgatpdp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2gnrjikff.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kypyojzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2grwvszxn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qhdrcrdi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nprqpfmk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wxdwzfbo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgxptbpv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tkcyjnnf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zougcmac.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhdrcndd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dpmmaapq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrozfwvl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eegptsef.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iyyjhmet.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wtjneyla.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uqtwdvxt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2eagigjbl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qqmgdqew.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ckcokiyh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yhyachay.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkyxdnkb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rohngxkj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gxztrzrx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wnzsrjsa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lbhyoetn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rfwuxvcg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vabgdqtp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2plujwhmn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixfzllgc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2markkbbr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dmvkgsbq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2klknjbfs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jelsavxf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2palivdye.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qnwkyvjo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vvhkcfeo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2voarawvr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2crwcpudp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2inejwzjq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gntezdml.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jwiqlitv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mjzqkyqg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uktdixfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcctcfei.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sqbhfjgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwhrubjh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sgumvcqm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zivyvzqx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kdttvvob.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ydqvbdlm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ylemrjvb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xguqtkfo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ccqqckpe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2egzejsvm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rzaaeppn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qivjdqxm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wkilinni.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2brphzvbo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cadzyrvv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rmssesrf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2llsxmbfq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zizwmnba.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tziggzph.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pliczbmd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wsgzukry.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wactawnk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2auifnfih.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2clfkphlg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2raiagela.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2itleazlh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gbolvutp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxkutro.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nbibemjx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2aygmjesq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcsupjsf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzbumcyg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rlwvktxw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rkyjokue.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wxotdoxg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkdwjyv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmvkzfb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ylpedfup.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rbwhgazr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qaznnzwl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lyiodeur.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xnjfujrv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ksjrbnnb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2pkhbdzgr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ctwqadug.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2asytsrez.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cmfrekyq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2axeslknu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cprchxhy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zcchgcdv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2piiopmyw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ctxyvxez.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2akygfhbv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxzcchv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rnknfrco.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2eujrkldd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2usmcywjy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2viuqakuy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ndqjevdz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gsgzlrpn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pgogqyig.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hzaxuuqz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2klaaffkk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kzrnwwdw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vcizamuh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vovrenjs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggewlmsq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ckvivtse.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iupyerpb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jqhihyyh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2spjzllro.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lxvwlnkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zvnlanmb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2smrhzpze.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2sriybjub.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2byjhmccv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rghhaxux.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jupmialy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cbbvzkcu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2olcfrmtr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vggkxodm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eglltyzi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ekkwxyvb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mkhwmaij.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2odfvnyni.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bciaohfa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vqltwfzo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xvtssmrw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tjzwjley.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cjimoylr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2owceeokx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sjtshtqh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cgsrmlpj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wgommmuj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xyregaap.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2srwqhybi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2exsfpocj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vxaeldwy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dslhyios.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hvuhmotd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sopycbvu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ybknarxs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vbruabuw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gcjcodqc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvoelyi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2othjdrfl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gyvkgpvg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2havmfmwr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzwpulp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2riexqhsc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2eyieehpo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2aguqgcgx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pnoegrdd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bbqixhpi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukcrkgew.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ydnwqmrq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hyoukorh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xexkrlnn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tivdebco.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vmxctiaq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfwglptn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xfotgicy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fwiwlwvk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2stnlhrxk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2alzjxkvp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vavisowv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pmhnoiwb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yaszfspx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vjkpuhde.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dreylyss.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwmhdqjb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ywnwtcbb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2smxgqyri.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fmujgayp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qmlacmkb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pxvtuiux.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2osgaoffm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2catbfidh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vojheyuf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ntquhfht.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sjcmesja.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2edrmwpij.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vkejadam.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nxwyzipk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xticsdfs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xsbfnkpc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xokvziez.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkjkztvj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkpzrsn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivycfqzq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2apoqwyxl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pklinmvd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tqewdmur.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xmpzpioe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sufmpfuq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vwfrglha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sbvntysy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2meetxxmy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nnupgrzl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lzzujtmm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oewigplh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mmgervfa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vcwvsxml.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ozslqmrf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xkkmrneu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjxzhex.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2iyitxdyi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yvywcjqu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ipbnmrwx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2njeigjew.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dtwzbzhn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bggjvuvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uubqxugv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bchjlkkx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bcayfgjf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xunorxod.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gzhizblf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qazgwrwy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2eexlrhof.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2blpxjued.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2flzysjbt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bgcyqkfs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2amhrtrpr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2iabvorcb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2szxdydro.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2opfqwlje.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jdjcghwc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2flbkzcnh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtnfhpf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nrvxrybm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfloftw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mzdenodv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbnrvwnp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2sknuhoyt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jyvbfrwj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yispiksn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zreyrbkk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yslejgsk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mpkxxgpb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fzpubdpz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nfrqqpaq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qepedali.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ppvznust.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uqrdwrwk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rdoyvnwu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sgnqhaze.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yoyxviyt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qoqvalfk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpnwmtmu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pjyeamcr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbwxuji.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2utmdctes.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ladyjbou.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2syemxhhs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dvowwaxb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zsvpkxbv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbmjgs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jbizaxqf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2knqfjsil.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sdmjnilq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yqsfetcc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgcihcg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymhfknkw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2asjtgpuw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ngxiltmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jspmlfrf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wsiinxlx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dvynpusy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ndcxtrxr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufpmzxxs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ypgqkspt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qtshgang.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2orgoroll.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rjnevvmi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yafsgkqc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dmfpkoxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fejtlnos.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ywifmnep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltjhpcux.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gxbsdgby.html


<!-- 参考信息 -->