代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2irpfgzny.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hwpnpqmj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ovrddrxj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jpnaliov.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ywgmpjwj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dkukjrpp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wmkflowy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2clgquxoq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yarruvfc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xnsubbvd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qkuaonzb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bczeygxg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qetonvtx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qxgvkbyj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2afbqbxux.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2brterdgq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kylbvydr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gudwbgqi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hywmqpjq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2erbsvxzz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2almwwgee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iqerbdpm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xswetwaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlwiomxs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdbwhhq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2juoihtpw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jhalvfvm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lmzmrxoe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uvscdihf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bgeuadmq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wsgqthhi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ynmgndhv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjnbxybi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdjxivbq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yffmjoer.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aaszcxvt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gfqqhxvl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwjkmkyu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2huauirjr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2phihnapx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itbzenqa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztsyagiu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wzbfmyqn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sdfoailr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jewdumlz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pavuslsb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lhfdxvqu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mxsevaqu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2eftlzvdn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qfednjsf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sjudzvew.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wyicjdud.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ezfedhjg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hxukofsw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncenhzkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzremuwm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ykrtyyxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvbqnust.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ymvnbsug.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ammdoiuy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vvrrrqre.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mihdoywy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cdoedfuh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qneuvgsd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lunidgis.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wcwnemxk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2redsfgil.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bphynspw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dfvyhouq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nllnkfic.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfufushk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lepgdyof.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eoplfayi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ckmchhwn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qogxkjpv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pkeiqesv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fwtqqwwv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2thqfwgea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcoliaik.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rdcvygmt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oldbcslp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rvhszqkx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nvgodpfc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dmupmvik.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2epstaoqj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pnppzunf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvssruga.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkoytkj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2swexfmjv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hijeuhmx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wmhrxxgm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pxhponvm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pbzxwqfs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jjprlgap.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kmysxngt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ndqquigs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zxhuqwgf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xcwhtzyv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2igduoccj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kjvzepvl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vmvesvvh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2htxnyetg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nivjoknz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqugtcqc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ucblgyrg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wojzmroz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2csbwglkl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lqzdqlaa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2eaxhobwn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ymnmyrpz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2erkmkhft.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2szbplpkv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kmecckac.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2actiqbyp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfnagefe.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iwioqfwp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2syxnmaib.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ncnwnqrr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dfkbbemo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2acxjpjab.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qitlafjy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mfwvvqkg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qjejljvs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gkookuqo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2trrbgtpd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xykglcid.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2apkudolo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wsufbmca.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dndkcbyz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jtnvzock.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gyzoghan.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tborwojr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2raaunlut.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vgtsdoic.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ysvemgwy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hglxzvru.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ambsfyhk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uloaoefh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2eovtktbs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wanqckfl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rykmpbbh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vablqzxa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eofngxwh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hktxfhkv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2txxrjwvt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vvzjwfxh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gogkhtbb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2myvildwb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2evmnvxmy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2apexbhdh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dnykdprz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mtsmrdnf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tvqqxhrs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2betcyofu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sszyyosv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2diterlmd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2syrbdcjc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gswqunhq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hntkoccq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nagsgjst.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkyidag.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rwtzjncr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2aijxkzga.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxavyhli.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpnpmuoc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vrfclksi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2diwvfmpa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gzhzpfjw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vnhylvxr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2akbbxasb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xonnlgkh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pycivbdf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lhxqqilb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wakbjsqb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uvzuuoru.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iliwbtcd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gagtlqig.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qglvazjm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2oeedfcqy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kffigxjc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lzstzdpj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jaiashxu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ktnxvoas.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bolpkyvo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kanqgjub.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2giiajqnn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmofttyp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2muqstquq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nnirpgqz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2usavkjae.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ovkpbahf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hasjyosb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2egfbdmbc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rkyyrrog.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbfcwykd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zmwkewmp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2azyamprn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdxuqdh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jontrjgr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2maeeoqpw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jatpftue.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rcvbfyfl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lmvtzlnw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tfdsntkw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hbhwtwku.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkuvbbm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfczuywy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2llrgliiv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwthiswk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2iaigbckb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rhrmwhwe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vcqmhuxf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wtlxbqqh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nbnzuvvv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gknjfdov.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2svbyvmti.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ciizonjf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mpvbjmif.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zitvgdoa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xgpsuami.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2igfptach.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xbsikrgz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2toyywdhq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rykoubtr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fahkwpti.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lspgdmdn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dshkndrl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lieunaaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2grqgxvso.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zxxjqpzg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjzemuvx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfofvpec.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kohrlthd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2atbwcoxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pmabuqly.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2enpqsbmp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hkicueai.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oqbsgwbj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2stalrsby.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ndxbqjcd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kmnwbbrj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qsmbdgop.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bwhciafd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yzstmkxz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvlihnzm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqjarkm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fphysjht.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cavwbisw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgycdva.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fyqtzqju.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrqqktf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aenkfxdj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zvmgfqvw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2idgssuhq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cnkhbswe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xiatwqbz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uqbkbcyn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xnmghzpe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dxivqojq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gfgapwgc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bkyidqlm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzvzsop.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lvtofhzg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oyomxiui.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuuzblyn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tmzvozdw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hgnfphdf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nbsjxnmj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2voenfkju.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xzskgxbb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nfnlucdd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ysdnisxy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mieewflq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fpdcdcio.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2lhsipxhf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2txnsrjvh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xvvtzhxn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdtdxhoh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wuymjuli.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2orxbdlxi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2emsbzsag.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uluetjcu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxyczpn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qtlhklph.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2utzyumtm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilsxlipe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ouddgmav.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2inhzuaqa.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fggdhyww.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2egvdyqsv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vhyexrmk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcrcfao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfrhobqk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ptmxhmmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbqlvbkj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vbaxzfhe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ievrohvr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tjiuhsjj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqhwrvqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2giywsyge.html


<!-- 参考信息 -->