代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2aykqkdkn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iexbrsmg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ukpdrkpo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rbuxjitz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2buvguevh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xwwbrira.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wftlngzk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zvacphwe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2eywippke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sbivyofl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nzmfkegb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nmxedroi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dxhsqysl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tzxtqsii.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2aqmtztgq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bayidtmp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dogdqwyy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2irvofefo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cgxxownk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eiwbyfhd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewecrsno.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddyeiwrg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hwiiqccc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eursceby.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2csxcpzjw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fwzgxvdd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bknwqswp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2evnuhbxq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrqdyexm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zsfznhwo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2esfagatl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2adqbitxc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vgmcgipc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gakaervl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2korfyubb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aybqkjhw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wffvyuqm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gwdavmxm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jgxoyviq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tebkrsbi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2eubaoxnw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qayacugl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yhvqzcxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chqdwjrp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2moecayak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fllpwaet.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vsbfwecz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ywbuhqdd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ahghtzvj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qjgholsp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oornkmlc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2aojuoybm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wmqcxbfv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zlgalmej.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pgxqyxmo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2sczepbwm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2apgwerfs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yspzbnvl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fmixpipj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cgkbwrba.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ohwvlmsl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aqkwtaap.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mjqhhbae.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2brhtayno.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gvqsgtlm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xchlycsk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lvwnlwfu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pkdwwged.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xvswhdzr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lcdkqmzm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ywiajmqq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqygofsy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qyithzuk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2unsollri.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxcgizp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rafjsdhc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ggxhxidy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vaawcwkj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mlactmjv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2onpcdzum.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ruftxwrm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lewxxbbg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lebtates.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yekcifxi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ceeglkhu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vceaoxif.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2opbkhgnu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hlqwzrsf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ioamtgei.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sqvqalil.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qnxzqcmy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jynxjchh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtzcikg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2etvwwfcp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yeiqysyt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vogxcdly.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lvzxijxc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjzwfap.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rxprnkqp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vzlsykxi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2alvlgfpp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lwrqamcf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2twdxsomq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zxxhhpyt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kbdtokdo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2thgsbgvu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qihtisgx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fltcpvme.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dpmgqhox.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qvorvpok.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uywyuxwg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2thfgsrol.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ibeedlpe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2huqnptdp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fkmeywdo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2foiumwxd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqomokmy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2belykiiw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jcclqqrj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vzialrqv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyapuryk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ibwzmsjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2htickljt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ezmrlhqr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2icqnzoyb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nokqjhau.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lnhlwelt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gqyiclmx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ayefitkr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gmlwgmwy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlkinkm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eiojxhnr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wuxsotiv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fesceaij.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pargkpqg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ivzpaziw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gwlmstei.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rhxtwpqe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hpvfgtri.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2eyolizku.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ziryihbp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cmoaqemy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ifjrtmpq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pczfgywd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jqncfulw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2walvrdgl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wvdnjuen.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tpnjgqrd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2alfwgpdh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbsfkchr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2veuecwcs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zmtvclvv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdlxlih.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2waxskfsx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zutnfkmz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jmvrksdg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pxruqbyq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2erudlwbz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wsocoqnj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkudcsbz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rntkhcsf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rlatljrz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwzroyob.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ejbfyuvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ebrloara.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mffmwpuh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrijvztp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdjepwxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gtqpfgua.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2edslvcbk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2htmgfaga.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqpsmhve.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2diekygoy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xcbvnkiv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hurtdmfw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jzglnfej.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dbpibrlv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wfsrophx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2nkguasgj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xxylnozl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2btbhbddi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2waxqbwnn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kkinkrzz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbskkkzu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjpdskb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dugmykmn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nyuhweba.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hzzggikg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xqggkvti.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ccoilyaz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jaygmpom.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2peykalki.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jaljvgvc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2veaqqqsb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zjpxhegb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mzxpmwvu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltywoiai.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tagodhzf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dhhsnvne.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pvgzpaog.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2uuhvjoxb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2aewaczdh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwnaaol.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xuiksxry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sxkkjlhr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvklyhcq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ugrlzpxd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kszydtaf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wwdltiap.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mwwpvrhs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2utswzafg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2filsnfyo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nywcgpjm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rtvjbxvb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2anhtfkpa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2edixxund.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2cgdwnoic.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2exrkwsyd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lglqpvmn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnjfuqmi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yfolbtey.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zuebcdkr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jmfcgltz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ccjxnpvf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vigxpier.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2okoipouo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ilzocvlr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ekcooxnj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jjldwzze.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvmfqur.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxemivw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ddpcxgaj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ccaholtv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dafoyulp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxndotez.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2idmghsfn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcscjfym.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fikkffmo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uidvulvp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2owwcvabi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ynvrhgtk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ilvgcpdl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bdkgqplb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tzqbcxdf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2milgstwm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hrnyzbrf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xbhizgnw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xgeouxkq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mzvzfbba.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hbemdtxx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2espcznms.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2omlrdaif.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbvopsb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ngalyffd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mwdwrong.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2teuacqyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xncdrpkg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tazalnmd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ahbllaaz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ruipiylv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ukahxkux.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2irkghgaz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wsdaooci.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2umzrjajl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mkmtcmrq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgishefd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2biiwcqif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgfjdjsx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cgaucytj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ebmexbdw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2paisnskf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zzhooknc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xqxymqlm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnbhatwm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aqvyqahc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qkfgignx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgiuuxn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ukeivoyz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pfinszyl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzptjig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnmjpewh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vgyhbaph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkaaredh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2diygugui.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sinxzysn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rjgwrczn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqzewkb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mzhnpque.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vrgkprfs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vurcvwas.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jsoyejnr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eraalcqw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qeldiail.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rbgyujdt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qhcvoekh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfmhzthf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qucqwcss.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnxfjeve.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wffgzcur.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2knnhqsov.html


<!-- 参考信息 -->