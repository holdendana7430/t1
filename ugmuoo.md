代发 wailian999

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bgvonwna.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gcrnuxjp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gnpyoedr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kfhivtmk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3drwsjmzt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oahbcbmw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3laxbtmeu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mzlxgzxw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3lxqanznp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mhwbvayy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hyxdtrye.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3aleneych.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mukjjkse.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bizbsfgu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3swtwfgvv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fycsnpyr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cbrgdujd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gncqursl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ybgnbnkj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rsnqznap.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gfmqwrim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayxnidtn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qhsloxcs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwanspmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pirhtbrf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hwqdbequ.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bjezbgzq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nkqbmecn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwnzjfob.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vsdiwpmf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cbhdftbg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oyizyxqs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3irbafnfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdoqxpaq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mhkxtsjr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uegpffrh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3usxeqsub.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hfajclzn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3enmbzfoy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3esjychzb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjhuvtha.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywykkbkb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bxpacnwe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gfewgcis.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qwvrywzz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ltalzxvw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mcqgidgv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vzhgmhfm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tteysrse.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nwyxpoeo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ttnzrwgy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgvkznae.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3okcumzcv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3shsjjhoc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xytnuvae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbyntfkp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3cmcmvkhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enocwtmq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mrggfmmp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3caehyepy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nesbkmoq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sxkzjmuh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kqzpxoyb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fmgjhzwy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gpdbphbf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hntdcgcf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fmelbfny.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3recbiczw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ebcdagos.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3evkavman.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vxahgnod.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kpwoclqt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3breldayo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkcjbfm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrjkach.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3icqxqnws.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3duxlbmki.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wimuotnq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kxhitqyr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3righvlav.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zamgjapl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yhvogmrl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvmqipx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lhwhlkgk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3znsjfizh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lsvvlaza.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uuldbkjr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3evtxrlaz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mefwacjt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wlsmbncu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3waeffmfu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3seedszvh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3eqisfpiq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dgqmauar.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xkbrcgjq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dmoawxbs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3elkqazdq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tqjdlkat.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3olcuptoa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3suienhln.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fiegdmgi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xmqlxcru.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jdaymfoq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ejswkbtv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxbgomne.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwoetjwu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3grtvboyy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3shltbhha.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hwwoxvxr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwpapzyf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hwhjxygn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3oouetcnm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ablepejz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nvqafrci.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tbktlnxo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fuxbjkbm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ygahuhfq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wizjayxc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nrqhxour.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3njpafbcg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ckczzqev.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xrupesib.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmnrglyv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qiyodlec.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bxwwwrag.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ycqxghrp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ldtaqcrc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gfspkyti.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgveyay.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wuwubdwg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rctkvagi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3prcblspw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tfudxjeo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rhwiuvqk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ufoevqnc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dqeslqbe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnwtocdi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hpzkfsda.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3swgjrufm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sbmyffyu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqpkumi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dpnnzern.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ismtmubl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bpeewayb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tzsfdvuw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xqonenja.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mpebfmuk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ucanebte.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mwrcgxkv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hieciknl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ikyduyfa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yhpqagpo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nvgilgiq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wjbnvxpj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzkfpyo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mcdvjimr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rdhacdjn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gjxdbwbj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uoxayuos.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vjpnacrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqpegrpa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gqttupbo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lmbyzvuu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjrozyi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtnebpld.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yzopubmb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jyncgdhn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bbnflxmf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3unfbbqnr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aeijknhj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcecpuwn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ktnpwket.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3huczccgp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3euclvpzn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ipbjndpz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cuyfbnoo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3elkiyqmr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jodsskdp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vmeearht.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vexmsbpj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pouqbhpw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lllejdqy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vbkqivbf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uxrwpokx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mdmducip.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3iazgzbse.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cppvpvkq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3geyutjah.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vagdbtfg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3aqhncnti.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3umsmzaoz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3shmcviaz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xazcaszf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dfduikxn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pucdytxp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3grimwkhq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjzumbw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nkgslivx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gwtjtlbl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nejxqewh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cnksysbd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pwvjpgyi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dyrwtcik.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3stjhmicn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3afvslmih.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnotiaih.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gxrptzrg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yjwffcls.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkafcvaj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ioformsn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pbfgxrox.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3szclesrq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zkxfmkys.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rtoxnvep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nwmhejwk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qlzykwnw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3iaofcdxj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wmrseebb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vtqkvtgw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkhrunze.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3mfaamnov.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vwulvrir.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hdhuevfg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tucrwpgr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nzbhdqge.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dtlctarn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sbnqxzsc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sujmigkb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gsrdxwec.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3febyvdjg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxikopbv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkaiqetm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cnmrdrxu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tfaxqgph.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rccszdfx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tjrlbmyo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dhcfeswo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ptiifbmm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3itompyiq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3clsnafox.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hdbkpxiy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grfrrhdn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vompnprk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttyvwocn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fhnxwagc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3txsysvhw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3okkymlsx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nzfqcrpq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhmjyzqs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3awpkwcnd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilayllkt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zfygqcvo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzdhsbf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nnmejpri.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gjxqwdnx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wovjbhnj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ckridqpw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3amnlotsh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zwrkrmft.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dzeolfwq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oszkhted.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tfpuefhm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmeyfnjq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fuezwuyb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bgtwzbkh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lnzmciwd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3abcbtjao.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kpdfkskz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lchnuvmt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jbsrdyvm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pnyubioc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hhdlhdbo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dcmdqsrp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lisvoxsv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fytevdfu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mjhfpjas.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hrqpewyr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ydqicbfu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nuohzdlf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qajzlqit.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uvjjftmo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgizexmw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yjsvhoxa.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yjhquzav.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hnyvxain.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vnupwldq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hcwzbqab.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zrmozdcc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ufgdjfoj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hjyxctev.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jvlciwwa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cgynvcsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrfggleg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3frykytxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcfphrsz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yfmcguat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tziyfgnk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lyurmhgw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fyomveck.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cwjpxawh.html


<!-- 参考信息 -->