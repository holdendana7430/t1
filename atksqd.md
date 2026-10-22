代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2voazwagj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sxxobxfd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pyarhszs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xsjodqnq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wzylamwd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2sxdmpvax.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ywtiajqo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nbmuuquh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2thqtvryb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2auhjxrcg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dtjxegqx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2opvnmiyk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tnsxsuiq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fetylkky.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uroffxes.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ykapspnq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ccpxposz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvbawnla.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tkyffrxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wrfdqyvf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ehannvat.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gtebszuk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zlacppwe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qtubnfhx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2btvjkxba.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2grggfvcy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rypseryx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jgjwzvli.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpfatffn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2llkkzjwx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xlpdvxel.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rhfnxjia.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kwtihrqo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mzyamstf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jlvspgmm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jvldodrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boqttope.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkhfccdx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lglwlatp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nebumfrv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2psrapvxf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kbailkmh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qrvzhdcr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xlfknguu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uvrltcna.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dlnzeyyf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dbawdeej.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yasoxjkr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2quikwkmk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2icuvpfqj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqccoibx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwofccvo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rlwobrfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fucpduwl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wirduxjn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sercxqez.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mhfxcvfx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2laqcidlv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tomtvhhx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ynnddruv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2imupjxln.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kuxijnry.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xmphliwq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yljbdyqu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2whswqpru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2oirqadjg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pqajiuqe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dgbjtztp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2citailfp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uxuhhavk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sivteubg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qhutfxud.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gvqbrams.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjutcn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lozfdidg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xjuicqvb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dwjwiave.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkaspznh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uuonaspa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2aebpuvak.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jbbhgotn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ptgbzbae.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fniamfmg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2aovtaejo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gsboalhq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tkqugirx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qmeoxqav.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vvdvfnzi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zrfettpf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ahcizixr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fevjbdqg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iezvlczz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rlmfszjz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gzdgqbkw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzrgmlyd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tadmetwn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yiopozyv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kzsdfqww.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ssehnkgj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2krvlyrdj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2onlqumka.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2efnvpjxg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2debnvssh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wnronpjb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bdliqoae.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffevisnk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2idyklahr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lmwidsud.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2voqkhyaf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tzrdsdnz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lqfuhwyj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iftnvkky.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjrppybo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xjbodaxa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mlencqhc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hyrmfpuu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxfpzbsk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2bfgwpqwv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ocusavjc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xxsqmavk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2agbgnrfu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kmytyehw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kujegszz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qycizkhe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2trmshdaa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2atbncxmr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jpdpxurz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2purhlaho.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmhjfnso.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2loxvcmxh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dlcqhsnf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qhpiwkdv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgygduv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mzyhxhad.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wkdfbmye.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qspjqrdl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzqsoll.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gnescigj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zclvmgxd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2grztnlhn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rslxhwlh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tvkaxgyc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fbrdeagw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gokrlprk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jrrwnlxi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yvqjpegz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqfarkwu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uczwdblv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mtzuhjfw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tgxcddhk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2lbcvizzo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2feschlbl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pqfaglpe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yndgupsx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2stymqsvo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lhfmylai.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrmwior.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ovojgcot.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2faazzuho.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgmxgzl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wkvrwitn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ccgnrmtt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2seogttjy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hwzcqrex.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2arujopwv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eejangel.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cinahiez.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdesqxhk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zhfngoab.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fblvvcje.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ovvkordc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mipayyzo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mtsbekdq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gwzspyxf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2psrkfhre.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qelysuzi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvtuatio.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqwfndoa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aaegszmx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hwulyamg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fiixdqjt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kgdmpsmx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhiszcsg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2natwhwgl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yxahtwtn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2luipktnp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uhmxmhfq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zokfrkcv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cafqmlsf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tqqbitvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evvvabdd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cjpuosfi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2smnynudo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkuozip.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tnpksewu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zaqqzowi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dugpemve.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nsgpdkhx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cspdxjsf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znlacsek.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sklklnxe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wpcobnfj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hsqrqfqd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qwqvcceg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfyisim.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mtlpwtnq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vltozivl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2smqdoxvf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cxobbmox.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zshgvlup.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2didlsrrl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qxstcssd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ryscialt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wypfehzd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pfdtfvcw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kroulneh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2usejqpkr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvgswwq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qodsbvlh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ulrvhomd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hfcdmqfj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vqyqucky.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ykqvzimr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2okldxfdn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ppmiujff.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zlvgdhpk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyatcqn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2osnwowxw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jmrjwbnf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rutksogs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cfmbvxqv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kvwttnig.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wapbmhqg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jvugoved.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zcrzkrzi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jxgcyzut.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xcisvooi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iingxnte.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jbsrocqc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfcxdsgx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jrxovdde.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tyhjxmmu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ksllgddn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zxvvidjk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfyeefid.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wiqgfxhz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aumtyqrk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pcvzoxtg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wulbaaat.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qegimltn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lupailzy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2acjtlngf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2llpibyry.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xqknbgqs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2runxndzb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzgghiwf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zisihckl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rzhcwaqi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pzspndpe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hrxektyy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdditbmn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2agjuiscs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2kbvrrsyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmodsbh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2abyspwlr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wvoeeqih.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bdlvcekt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kqqtnbwp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2otfgxwfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xhqjdaua.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2grjzrgkf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rkdfuapj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2etjgzhwj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmgxvfk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rilsoqvf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2byadldbp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ifjagdhp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zagkxfdb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2npyquhca.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjwatrcj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ruseupxc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mbnrrtrk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oycafqpa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ymoyphcy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2myhykjfz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qdexrmzb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bfakcobn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vszwvgil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyqvjghn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cvqxckvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxzrueaq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usbgysrb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tgsjexuj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hidmyfqg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kkkkqxdc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2djzizvxp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zscjnyfb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nwuwwkzv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wklrmkhq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nxxbjqyk.html


<!-- 参考信息 -->