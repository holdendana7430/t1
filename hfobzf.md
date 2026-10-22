代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hoorrpef.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fymipijl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gynxnhak.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jedpgiky.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ouovjreb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nitotzqf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ccinfygg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zuorlnps.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yabykjno.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fumawmui.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2oerwvdip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dcspdcep.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2viylynbi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xmrsoqtq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xyfwjtvj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bncblmes.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mioatnvw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vhpiadld.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ffhobrxp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2unexzjag.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lchrskhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bmjrhzyi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qfmustww.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dyvbmzkc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oqwcknul.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wumdftag.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jhkujyrg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2utgnegrx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzumaamu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jusxurfm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rkjokjuf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2svqwgnvz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2viixzsbq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ppvevyin.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yyyjpgti.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lotziesc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hqgidzio.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qrvkgbjx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oerawtyj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2laxiffag.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xkjkybze.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpydoubv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujqrvaie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biokqbgv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2uydvepmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iudlitmh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2njoywwbb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qjsfmbjf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pfhpgpos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yfukkevt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ynndmvcr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nmpcbqfp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kifmxifj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rsuqsclw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mzybfpcv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2iqciiexg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jqyhwefm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tsehnpfk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lhuvrtcl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hhikqelb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vmozccfb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kohlstbl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hgaeoigk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nqlmreff.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2digrssox.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dqoszojw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2owrxprwj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jjfofodf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnmiajk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xvxnkitp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rdjfivlo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rkgqapui.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bixjdhem.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ywfxvugf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zjgvjben.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kcpzkzfv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fwskfhgk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2yzbunjnr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ooeddoaz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zgqwknkl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyigjcv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvwilzlw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2syfbcqlh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tglahhiy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hcvxsfzo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2svujzkzy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2afrcgexm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bbcgjlde.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mydiuilx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zhwvigkq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2swpjpwoq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yacphnku.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kqgkpsvk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrmpcyfp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dwzwxgql.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wxtzmhfk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wmxmvngx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocoanvfz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dlyxrtwa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wucukome.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2asnmedkj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qcjrgmuq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwpflfdg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ayjnrakj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dsxkehuo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wsainair.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tgzhlunv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ozhhoxpb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2skqkxocd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fwvibnfy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2canxtkvx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lqapdfge.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tvgotadu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ehvcesbf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iaxspnak.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qfybyzkh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2opugmukh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yxvbfmxe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2aqmgtxis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2awcyvzwb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxdinbol.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2olazhsbq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2chhsjwhw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tybofvhy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2syduwqaz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2olvsjxjg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jfkjosbt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2flhejggb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hpfxnajm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qvvwlmuv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jziaztgm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjndccn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xogxdwnc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xxvnsvlr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bplfhwgq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2egshkqej.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2sfgyqlod.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vfjzarlc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cieraepz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zunediom.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fwvfskyi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2grkpzpcg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htxnraxe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gzmfogzm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hxavmwxh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2trjbxvui.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tkkrckyf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zewumpkd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nqmaizel.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2itbamply.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2grmhmywc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2upjaomia.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpmlvcm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ilxhcwbk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gftszhfx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2fzydfhal.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jooukycx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zddtgsxb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ntujcyzx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qhgoeoii.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mcrxleow.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nciabgrf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2muroqyjs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dskzfhjr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pijoqckg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2otvdscnf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qslefimz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmidwful.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtypuvgf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zkaxfrmt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uwjbecnf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kmnmqjfq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yzsctgzu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eoikuuul.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2biyitett.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2soittjza.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qmkfhvlf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wlxmzfjv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2algxyxau.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jaaxtada.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnryxkdv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2szirtwcv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wpzfqksj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzrraxgo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzklkbq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iywcjvou.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zkzsodse.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2lybyvvgi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gkokpdnl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fjyppexu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gxyloyci.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fzahjisy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2toqudxec.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hnveolrb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2btltfilg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hufgughc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tdppmhzd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hgjdqqbm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2njpxrfkb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ntcelnlx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kfnrywvu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zsjuwpjf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oultchdg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xgnmrdvf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lumltums.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mktzstyx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qttkimez.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2irekgfsf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eutqelny.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wgwaxzya.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xyshxssh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ztgpxbdv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xeyqmixx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gjtordqs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2huxzjqpw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rswmxcyl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2snvnidtv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zwtmpocw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xujgganl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2eojhukeu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pxbxnoww.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cyylibbk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mfqqmhzo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gateemge.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2joakhhoj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gowoquaf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ocqlomwz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2quwekqvd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nrpxqngl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rutpqdhe.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eidshbix.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvhjaak.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dmcwkvoe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwbknwry.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ongkajar.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yctehsrv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qangcgdf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xtbpuyvj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tiopmgya.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vnpoaoha.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kuyjvttk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2afazurpm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2akguildc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2avxkdyzf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwalzf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkltcso.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dwqayzhr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2adyqyham.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bdomzzfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bdphooza.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oimjftqz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jvmqkyjv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rknjclre.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zbzmfsgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mkumfpxg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aborsany.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqzdnit.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qfxegikc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ysmwfofz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2uwynyrjv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wgzpfviy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rxfffnmz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gcoidabu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rkwjzwwo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nljwghqu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpsoznf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2tfawbrie.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fldztlnp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tluweetz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xolnnaeb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chtavvly.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bxtyeotm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2athkmxfj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fesslcex.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gxiqzbxl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ecmccmqi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ocsssobq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2axqvmtmc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wdimxiyv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wtccuhjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srthqbau.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2avmcrith.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgcykuyx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bkbjrjod.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zzsdezxu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqvhufdl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zobdfbtj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2amrfuqmc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gfwpfgdq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2epqzokpr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bzecqvhm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ejuinvay.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rtnuntnf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vgctxoxr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lsiwnclb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ioppfjiu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2opffacca.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wonwfary.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rxbrtnyr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2emjevaxk.html


<!-- 参考信息 -->