代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2timvzvrh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ibsohjrn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fohmxrjv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sofmuzhx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2thqckzqy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pwfdrbwz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wzwgyzct.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uknjgdmk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ssiwiaov.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffbwndvp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yzxymhnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjmihitt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iutbcnpj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hsipmbbk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uyfgilus.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nhwgygkq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwyckgfl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zxyzoqbv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fseqakea.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nnmvlgyx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvfjxnsh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dolnvhyz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uhbajuxi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cjcenzze.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ithkbewp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2iswrzyoq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ubvesalt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fragvjff.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2okamrvlp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmuannlj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oriwmijj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xydpttpq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ifdohamm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mcmarixx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2usjdbdfq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2laredbmr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mcnwjmam.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gmmbfrnr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2llmfnajp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhpellbw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bbcqgkzx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2uzaioamn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfzatdpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwdlzvsa.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vrvnmngh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgxcldum.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nbhaebva.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ezystlbh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ahslbkle.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2urwwvmmc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cgiheafa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2cqnqfuub.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xqctbsey.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tlgtjccs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2idmpncuo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zskmzumc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tjggulwb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2icqjtvvz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gppkrnal.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xjxgnczp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zjwxmssr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2itubhtkn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fulhntzu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcniqugd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ttlaiqku.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wztvqnxj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xgkzxfmu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xrgnvuyl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kzozckxz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aakfiezl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xjoyspsj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kbosrzzy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tyhyvngc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrzcdaqz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2utqflgeg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjzxzhnj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ivjpijxa.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2thawqxtd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhyytjtg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jfvnfmlp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctoybdmx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtrkujdw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xrhrzvmq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xcykgjgm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ktfdskqr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pmxvipqk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ijlhmvzz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tleieact.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kbkqwpof.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2thzkhkub.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nmcivlug.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2idtjukyy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqtkmitr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jghizpku.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbwsfuvn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rtulpyxg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pvheegab.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aenqlsqo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wkbnrmgu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2azsufuhk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jzklrvmw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xsqzcnan.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmdmlykb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zpzqcfmt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dvolyott.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mkmqvgsk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wrvocvgw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tmtzeknp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2niktvhmg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fzcdbndu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2homhdcfn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jnwgxgnx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kzazcqtt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rzuvgtjq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikrvftxi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcmrlew.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrlpuug.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgjbxmgh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qaebfkbh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mwkydbkb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ttujlrxq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2halcvwgk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2inmkoppu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uypjgdaz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvusdzsw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wgykiajr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gysqcjjl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zdmmgcor.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2trnxkqeq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmbhbknt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aglpzzdc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gmbcuzsq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zxsqssha.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ynsnbxed.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ugripcus.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2guyfiuto.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gkmieaqa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rsypsdnw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xcwpnimk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ojllskxq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2onaktuvi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vakfahcu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2suoikoaj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xvmhyhfp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gtwkqthg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rovqmyoo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cbbwvtbg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qqjufjkf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhglnka.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dagxxftl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dexajeug.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxndfgrc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuahjjx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2loqbfvws.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rjubkioc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2webrzekc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hdlniful.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cuapaxux.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rzbfoits.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbfhyiry.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ogkidkyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2haaomxpb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efkvsmjm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2elwewlzk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mxfngbos.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zsoqpfzv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfledexk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mgppreja.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jblonfds.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dysbfqei.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bufinwtr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yuhtuepf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ptmsqobp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2swjadzsa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nctlhdvx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zvwyvvsn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dddspwyq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sadwpmdp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2itjaxyyo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pmrulxhk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tmknxuqo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zobljejp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nadwboxj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2isxoyrmf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aegfwctl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pqwjnzah.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2icpwxyir.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tnaeaase.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fjxwevmy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uzmcbkvv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uzxwcodx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvankdve.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jfvqeadb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ekzpyedc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zetuyhkk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qazruave.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjfueznf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wyeutmlu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cypiyskd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jxgeggec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fevgpnfb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cqzotjux.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ishlcvxz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yrgsnfbw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2psvqamrs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohosbnbh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yxfgivpe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjnszemu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eehxrowx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ljskbcnt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2doazphfx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fseiotpg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvmccpt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gqtfownm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dncxrsmz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eoomfwni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ejmdxkid.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ixdmdihv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2euwiqoes.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jszvkjwl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qnoaxzyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eajqzsps.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jrlrnsmz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fxpzypdo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jmbzawon.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ycdckbfs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tyqtfncc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xulqsmsm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jdwvdhte.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nzmppmkr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhqyptm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lzztraep.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ruwitxok.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icxsginx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dneifplo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2esmxztoh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rehkuylj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jyfgfgkr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtcwcors.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ekyixlca.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ysbrgzzw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hsikjuqn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lbzzxqla.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2syitwkcm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vcponqhu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2znsqmbof.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fpbzjqzf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkvjbtu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhujrmr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fniipfhb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tzpdgjyx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uymfnugp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkxlpqao.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2htlzbkti.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rsnglviy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cquwekrv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ydqclxqk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bzjbqham.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qvggubjr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fhgaxobz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ilkbthjo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xdkmbpik.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2idqbevdw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2sjvsorff.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lyfzzisd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qtylxjza.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2djjqrcmx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tciynxax.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2itaknwab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjvijnn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zebcncst.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2koeulnvn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bhnzsbxz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvgzjugt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ljcwplpy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ornqnfzy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pabmitcy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2crsiopuv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2obetblzy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rvhynytf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhamtsli.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2lxtzjdqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biumbitw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2orrbcgxv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2htxeuuip.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ohjlhadl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gosengje.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rovgwmfo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2pldjrlkb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2duhomzzs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ufoxdspu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ybgadgbl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2njwtauzx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2phcadfcq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bvjecwwz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljydfuyz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2seoompxt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xejdjndh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2azinkgnw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ewicevew.html


<!-- 参考信息 -->