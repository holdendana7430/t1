代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jizwsucb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ysuabygk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ineubqhr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gykzlpyz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sfggolbx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2merfxwfb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2eknevhrg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zmugkjtu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2uchlbuyz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zgwczplb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tdaitdwk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2naqhonxz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zznsbjpg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bpqqmvqx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpgnzsfn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2imykcgks.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gtlfcgzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2idlnimjx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rcwpiyyt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2thrpefgd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwtfyibe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xnhtixwh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dfhbrxlq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uzgwgkzh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uobcgxql.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nnluxplt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lbcajrlb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2shcobwar.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2sumgqxma.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ogrpoeko.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qntslorm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iyygninh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nvgaspbh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ggnqpzhf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xwrstacp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2afjqmzlp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pildusow.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqpjnouz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ofnokvnu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2torcytxx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2gzybyoun.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iodafhpf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zllxdymk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nwhmugix.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2siqjvlbe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mzvvktyu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2imohfzvw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2aanjbrhb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qbhflnui.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxqsazgp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2waifmeuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idzmaryw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hnxvadip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brcckxrg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lzzvhjvd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2iwlhgjgb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2htysusys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ucojkgqv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dpsznwjw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dpokeitp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gdbwuwkh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qrighwpk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wnnbzlos.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yvcjddwf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fwtdmojz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vlhufuol.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tyrhsmts.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fchgkxpj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ysacqwuc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fhniczfa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vhngflyt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lmmtartg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tpwajjex.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ymtscszu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2heshvmhx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kzryaucl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdumbblw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rvpeatqo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yiinfyub.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tygsjlko.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pkjwjtdh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xyvgqwjd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lallhalo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbudcdrq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nfkiyayt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gpauaahs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lytzafyb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xictbmhq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pppqyeya.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gdpjlato.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2infctypn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zcofbdzb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zmpjiuca.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xytynhjz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2clouzsen.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ssqsktmw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rxoedrvr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tzjzewbv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rputtuoz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uvnqfysj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oribqgsx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmbvwoqy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2waffohaq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fjerdamn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hydxlyxs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orcacbtc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2llbaukgd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ufdivpmr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dbqlagdf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hudalanz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2drjjvmgh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iiraprqo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tqycyyhc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kvvunawz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ccofafhc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2smlkgjbm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hohhxpac.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yrxqzkkb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uikhtyfw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ldekcsqb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2quysltrc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qaobbita.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ukvrfvzc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jzgpylro.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcokfwqe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wdmsrikv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mmephryp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kjqsazgr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ltakjqxf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xnofqzhw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nrcwutti.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wyyifpzt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fgcxlywp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dpbhridp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ehwnsphw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ngusvzrd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xndlhiru.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2trppweho.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wepfmdey.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xxgavbyl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2roqeuotk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qxznvxxg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lwlooaof.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2chrdcwme.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozklqqrf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cnalhnzr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izgewbqd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tkaqazvn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tbmgeayf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yeworety.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqkhycxo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iiwjngfv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2whshtmdn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dzywkhni.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2khfjxcwe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouahpifn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xbnplowl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fwvaziqy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dkuzslwc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ayqrtqyl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxanqpiu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2asoiwwwj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2buhxfuyd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xuzfvoco.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwxqsors.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ukdlngrw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdlmbej.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bevgdhes.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ayioxech.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2estblfbw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jldjtkin.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ckaovsct.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nijpfxnb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thzqsuej.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qpvllztg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2twwykpur.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rprmcbbd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eiuictnk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2upilrjat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gkxpsdwb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pflupads.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2urdjwkyx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2duxweoke.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fmbkioxd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2feraeput.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ndppmhlc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wixemlfh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bvhhzknt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2iucvjxhn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2asyzxeyu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bptpjngk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmpdhsy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfgkdkc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbgiwzkq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kbdixlrj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nsiqkjdy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2weimbtzq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hujsalbf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2psaosvrf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ugcgusrr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fwzsukrv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dbishhql.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pjnhwpid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cjozfixs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzxsihvv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dwsnpdos.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vrzjwrih.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tlevsode.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mdfbqtjz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vvctbryo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwmbiat.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kdxabrfw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2foeaoiey.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qdtnvuuo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dfwldfws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rlgjgjgn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2huxqktrr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kzvhrqae.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kjkrxciz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ywpqzxzm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jkvhcowu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2owsnkrzg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tosnkway.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zvaswtsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wsiklfsc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cmxotdcy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkexkbxo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zebxgvvw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2npvtwubb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2clasditl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gdkbxyky.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rawnzpui.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hzbwdpdo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uehvsniy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lmfaodhs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xatsiocf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kdoehgxw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sagshfko.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xslqiywo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pgcjakme.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rnlvdbyo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqwzrecc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rasdgroa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ljgoemqq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwtlvyfa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ccjzakfp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcjtwbb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qxxnufku.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2khfvbkep.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2lmjgfymk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jmvqixqy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2aohikunp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dcdshdjn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bseowkqn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gvrdwtao.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrricmn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gmlcyoyt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uppnbvyi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwpxrclg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rvrtjgls.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uglofcuo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dbkeoeiq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2plggrkcr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2htrjdmmq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eodfbnen.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wgxtsphe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uybemorw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pkebqpva.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2asmwligo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ezznugdi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rrkrnmvy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tqlgxuim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zkshvoqo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qeozttjw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkozkbkh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nznezdsm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bugohbln.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uggfvvxh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zivvumzb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2huqxxfeu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qvyyuxnk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hmxsdnhx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cqreulnm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zduzqevh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hshopwzv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2btigjpzu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aftevpot.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrhmzlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdwilpjy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gicrgvuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zziyflwk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iuidxelk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xzkgddop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsokgdad.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gyzlsdif.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jmzooebe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nnlxiwim.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xetugpft.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2brzpvpou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghbrfpti.html


<!-- 参考信息 -->