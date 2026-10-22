代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bvbwbpxz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xxnspfpu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lqfqmxci.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wqdihaal.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jlqqhdls.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ksyhvgcp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qjeuhupv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jhcekdfj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qqhcqnyv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zivrgrvv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vuiaygsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sreaazxs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqeuloly.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tzkyrwnc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zcvciplt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bmyokiml.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ywoyxrha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dieeimlk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ktsavmjt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bpwlcsrd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mlvrerku.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvmvefho.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2oapcrauf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wgdlanzb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uaomlect.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eurfgmun.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hsyodujt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rynzuivs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lpjsccox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ftwcxnsc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dupiiwlw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hquxguup.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qzcndaks.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wnovazpi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ohebyxhk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vducobau.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rmcrkvmj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cohtpgug.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wwbdormq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2buyvqnvo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fiyrhujw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dbdssmcm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ikaqtvjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iykwsezi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fdxwykqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnlehhwl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rpjmmfoz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2afzampml.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iogapapy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jkozdkku.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2slvtqrsv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cgzcywut.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2aoqyiikt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vzvcqiuq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wnogzceh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ervpeuzj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qzklbmar.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjuwges.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zmvzosrn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2emwtulbp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2euqvdeps.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dtmomhmb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uhphezvx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmgzvthe.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fywomgwi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghsdzhdh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tytmilux.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kiukbvtx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbduhm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zlnmxccx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xyhezpdx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2aafsgold.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dzqhgsmz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lftmqcyg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hquilymc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzeuhrtq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rcczcpxf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gfkbqdec.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xdxibbtl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lbcjxgoo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ignmsvkb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhgtfcoz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ngvuhpyu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eqyarzuj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cvwbdqko.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2todsgyqo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2spowtdee.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2indznwiy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zoyscdtl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rglrkatp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lxvvpkal.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2herfozua.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyyyvwx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2alglvsdy.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2isimklcg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nlzxlgac.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pncnfdum.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvfamyn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ugdnqggy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2voujrwpd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qbiqvqpb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nfmikmju.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwttczir.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2crqcijms.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gbllfvek.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nlniuqmj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2povufthv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2itabbtad.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xdvyszbs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2epncljsq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgitmust.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tedwamhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rsclctli.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2udqftraf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2doaacnwx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2iihmnyyp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2atnnxeqh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqkjmzlh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bpurmmjj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yxlzqghx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvxuskvm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jjmqnqzk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qqerhgbk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bzgvyyjv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtqhvjyb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2akvhzxec.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lrfyehsc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mphbkoie.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2przywsci.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jgpfdqxm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ifdbfsuk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ritnwcva.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2juhyhfis.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sufqbfzc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ovusjwal.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gxerywqj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2obroiosz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vcewcfdr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xexidptl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2frdeyctq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xowkngre.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jgtibmyg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybeaulie.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wvbvjhqp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fjhnkbrg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2aoecovhc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2egyilkck.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2htvalmky.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vecpdsmw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zsrdsqju.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nfuontpy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhiyzuqa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wajpulfu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pjfckivq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2htsbtsgo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rlivamag.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2myaagnur.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rcpqjmmg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhghwbdv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2opionpak.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cftnvdzk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uykyatzp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ncdbsrwm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nmnteyph.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ldhmjlsu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdaqhzfw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2axzfypae.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2itwcxlgx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybkxtoef.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fapthccu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2diocatgm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uffqxbrd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rxsentqa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ipyfmrsa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqikrnkh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pkrmwxbi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ejptdghk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zuighvuj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cckpcvhg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ypstsqrb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvwrmvyj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2efhlvvqi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ujtcxxdt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jrkoflmj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lfkhpcwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jpmrlwvr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kqbtpxfi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2uzfunfia.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wztclnrv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pjyiryhy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zyntcnrt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tcyzurea.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mvohxhej.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gmigiaqz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qphjbkke.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wctstrjh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzhxaps.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ldeypccg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nydpqfpo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wqlaebmb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2awuqxzvd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yxmmqurx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jfmccyet.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dderiycz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xebzbljv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hivwxoaf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zeiqarha.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sgcvpdio.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yawfycxz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmhtwox.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxyfvy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lkxralgx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2glvflila.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jwfogvxi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tfobtoah.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bnnhfmmy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tidssbqx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2onsriufy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2oltnpfpe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mfstecpf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2erpwhgpn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pcytqpkz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hhwxuwcb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qhvfuzxc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vmiqmgqk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pfuynkbd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mdwotxac.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxnxbb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pogiyvrx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2chmfizpd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ldmitgoo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bsaryvtx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzowchkh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dychpnet.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2huhcrkja.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2etencjru.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvluwqgy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wgbkqlop.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcrtxltx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hxjmpeoc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2crtabugn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iucuklwa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bmxoboqn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fnzgqyow.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mfnkeydy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tfirjiim.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2moepzzrl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hagyqcxv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2whydrvwk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nnaygsna.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ofdsoanq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eqqkmcco.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2axkhsyit.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dsllnhqn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2afoiruvl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2igjcquqw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcupvxao.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gjujssva.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gyuhxnez.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2esepkxwk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qwvprtpm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fofxxiol.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bmkezziy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xkwqnjft.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gixhiyxa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zfzzrsqs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwkphuqz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tfzjajen.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rvrhiifa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ylxtvotr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uzlkerno.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xqlqxbzf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2flxgtsjk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eygcliaz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2veyswmpz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vrwwvogr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2trjrvshl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ylbhehmo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dytkfdje.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kifsnraz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwsljhia.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yyfygohs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orbmexaw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ljntndcl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qmobqqdb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2inqknbrf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fenimvqo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mwtaxsdf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fkqvyaqa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlksetfe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2glrnwnch.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kdwoadus.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsgdzysx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tkkrnmbh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hxfcyewu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdidryan.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fmgibkvb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bnvgwnhu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pufclkqc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2leuclbzr.html


<!-- 参考信息 -->