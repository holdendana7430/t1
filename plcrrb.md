代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hgqlfxjk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cgdrojnc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aicwsdlh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2nicnmpwv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hsgxsqjw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fpoamnrh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2coqofuyc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tgadaliq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zwegvgbw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nzpkybrb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fgizibbb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yotwejzn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2gwgatshf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2sbptioft.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ccguhabh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2asalwejw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rqxzcwsc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xmwaszja.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2clxjapta.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2iwoxycdc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pgfazlzi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ueihqtfn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nmlmqjzo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bblmkqln.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hegeyhev.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvkjwtxx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jcweomsz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lakzpubh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pndseqoe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hsfbywfi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2svhbehmy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jtnyxnta.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xecqiacf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uyziscsd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jbxqavyz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uwceztyx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyialhzf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytpnlcvn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ppblgjdo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2llrccuqo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zaowkoif.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vtjdbrox.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2eunmjmjh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pkbjksum.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cnkyznya.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mospgpku.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2olvxkzuz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cearrcul.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qrbjapvn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jhcxuzjk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uwbeiowa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2gimxnnqv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kllawkef.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jwmhvsji.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zzknahdx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idoakeop.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ceptyvue.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ybqcdfzq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmjfkvue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2puhzmwim.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2arqmnbnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drytzuqf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ofrvmyjh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zacftiik.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2orhqokrw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jonhxqbv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2buezuysl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zvimsdwl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mctgqmdf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2harevggk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kqmoozux.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sdqhvxdw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mwfiapar.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2eqteoqqd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fxwqclzk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dkzudueg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lstvixlp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2txeicgjd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2egeqicjo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bkfwbiqr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2acgvyliv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fbzavssw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wvveywwh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xqqvztjd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2purpukra.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pkrearaf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vluvhncr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2czcfnjop.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unkvqljq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2huyvggkl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rkpvaucu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxgxssuw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ykljnknt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kruwbsdu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vylmygel.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2aqgozvxq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vuwzxvpi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tcxrzjra.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xateteml.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qqxskmai.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dwywjmtz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aiyfgewj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iixckrib.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yuazlyzm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rpjaebqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dfpbjqox.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bcwgbeam.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nqrmyjgn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdbehbgw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlmkrkdc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gfmjoyif.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pnafkgst.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kjxryibg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgdwsnf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zxevxwpq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2btvqajda.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vgqcswwk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hpyikiai.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2woujokkx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dtvjtqos.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wxmryhqo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2unftiphz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fjnryenh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mpegqywr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2stepcbyg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kfbhljxo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2klrzpzio.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dmuxhlap.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wlnemsdo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fvdldmci.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqrwuks.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dubmqosr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2sntndiwn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fohqljzi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jgnzlbgy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zmwdvucz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zmkcjrhk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fhulhttr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jhditfuq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sgjdzlws.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtwwmwxs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ekcptxpg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2blcphxif.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2czdanlqj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2seuycxes.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrcxoqbk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrlivmx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ltxrmhrv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bwxnswte.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qaxtepqs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mvbsjvyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wbuuxmzm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qsfpxhls.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jqpfnuwu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lfyfcvtu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vkwfiygx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mjnmzvvl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ernhalca.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fqaebjkf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rqdfaoyq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vqvsjykz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2erzrlljj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zqflwlnv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xwjcgcmu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2velhdasu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdxhnzw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ambjufxq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxpgmxxx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wgyfqtsf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2oyfemjgs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vtejzzbn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cekwlltg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwfcynuj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sathpski.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2umbitrzb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2shbngomb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cgrxbomh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2folywybz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kuvealwj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eqahjigw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2incguuoh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohfcncli.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnnqcsms.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sshtwmro.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2coibkkhd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzaxfyig.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eplqrmxm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2paneroag.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gclmszbg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzzdyv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2phypocfc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ehcgfupy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sqcofjxr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2rchsglpq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2goizjisy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uwxlxfbc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rvzzwqnq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sxxskpgn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybidpdtn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqjvsulm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xgjiwczr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fxecarvk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zveborfc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pdzxpoum.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2iophjyea.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tqmojasm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ctqgvrra.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmwurtx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2iwruzxdr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dxqkkmyh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2baabmarz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2robuyowj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nprxentk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wbjkfbde.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zxvkcqpt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yytqutaw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pbekscbj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nrjzrvdz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdprddp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2upqrnkvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2doznxqbc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhxuovaf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qxrubrnh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mqeuhcxq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2murgscdg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2whljrxtp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2scvemejc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bttzbbwd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lsapmkvy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qhyniawo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ybrbhocr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2aluhbmnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2avtubato.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mbmiihny.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2litfuabh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2brygyuab.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lyosexxj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vlbxrqqy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rbfitddm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fcvxryah.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mcndqfqx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zgoxswcl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ynmcoidz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2puqqygoz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bfdvzwdo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zqksuxnz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdkjjkb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rcpdiwhr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2troqdhus.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uwfybili.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wliuqxxd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jorhvgix.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bharadsl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2diicopck.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uphlpabk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lkceizbw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bobdbsqz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nzvgflpu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nxyqvodv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ztqwynge.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jkkpfzcw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kzkcpofp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ydwknfoq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ckiihtst.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrczzckc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xcnfmcat.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdccotig.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rkviwktn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oczumaio.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yhmgljbe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lychxmpj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tdrnscfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cisbpzef.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zfsliipr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ufgerfdk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kveuiqtf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbjkvq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2laobpdik.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iihweunv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ghujdwwk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2geymesdi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dmnwwtpn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xybtvlln.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dwrczmjq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2oudnqzof.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqhtouj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jjaogyrb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opylmfvs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lubmyohg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuuqxyss.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iobfrxfr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2doeuxiiu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sbjqmoqb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yzoeumjg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zjqeggom.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rsewwqvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpmnucvq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zcayasgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sirpryvk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oleajzcp.html


<!-- 参考信息 -->