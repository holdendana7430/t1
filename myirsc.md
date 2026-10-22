代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sunuinbi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vhryfhtz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rikkwsem.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tewyxjeq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uctmtvjx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qzlyhnhc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nrmaedze.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldtxauej.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ufilqlxn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ifguuyaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zwurhqwz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kjjjmddr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzzyfkgq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ukgtkzmx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dugvurdr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wvfnpyia.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxahnywp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iavfsgen.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zotbgsdo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ytgdqfhw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lpeekwai.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xtoofkgx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cxmghhvi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mpvjxaxf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iumjqqdr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ienfxaeq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uvfvijif.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ydhjybxr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qzvoxmft.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rhhkghza.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ngmxjpkh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lhwgmfdp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2huoreqlb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kapdnwdj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cajtorad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xazauyjm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zvjkhsws.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2aktshpgq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fkrmehue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2peawchak.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2haqcfubi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yolqkzxm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2djsbtbxg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2fvcxkywc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ravnwfsw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ienllyxs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2matooxji.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ammxpyyp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2diyyqegv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vllergxg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hjmxcqnb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2swwnsehe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ykkneykm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2iowdmnvv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2azydzfao.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iqataqyx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2enmjbzur.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2apgogxab.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sfuomrvj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iyyigvpr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dydsmggo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwuebag.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mhqsuilg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2syqwofld.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gztrlast.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2djecjqyi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kiojldsc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2flfarmyj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mwjxrqvz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qnwxuhlb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oqshdxda.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ieypcxup.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hcywaspb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lzntfgmk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2eljjrpuw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbmlixh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nncxfizq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2suwcampj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qqqtrtdt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2anomzfjg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pmcorssr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kriwiuye.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2acqkospz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2iveofzny.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vozocpex.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gizzhrcg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hseamyex.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yvtgzrqa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iggwgehs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xufgzlge.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kdydfezb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gnnghhxv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ajbodruu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nztgdobt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2alzmsgvs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2akarzrll.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uulvpkzr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zuiqstrj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qakcqixz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fnsgyzjk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oryfzwiq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yyfwswyn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2amvicina.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2usnkbann.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rozruzdx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vtvbzzxz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2muhvjsjw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hnjqzogv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2soqvjrfp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mlxqxlgy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tektpyoi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nvuqjnis.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2joojgjkx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnrgwuco.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pykugwgk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hxrmltrk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pffdjbdw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xttjdzgq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qzhctllv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2udoxjvdp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jvqejlrw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gcbqloli.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2iapmztxd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mhwcsbnd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ovtvbgjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kipbckfv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2imypajus.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pywfmipv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jjbzgxpr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2itqenbks.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zcgmxchf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2curehcja.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pxjhgarm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2acsflqjn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qedrxiim.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fgdkzsfz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2itngaigl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hoewtfor.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwzjloh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aoyrjstv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eisdoewl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oayyjznp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jiqaclcn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qqppgnuh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2knorgpug.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tvwdxruj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kujburhc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwbildxy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmitbgsn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2abqxejoa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bzhxogak.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uxdcjpxw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjjsoqmh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkldvtz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vovbbxiv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2csqlreru.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cquhfoxw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vsugddca.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zggnmcsu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xtymcdxd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xsgmjgvu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yaghqker.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekiudowk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcozfcwb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2olvtlspl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkerkrzb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xadjhxjb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zgvbyoqd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wlwoembh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ogwwinoq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghrsouvw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2edqxwkbi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fkohorsa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fmcgomeg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rayawlkv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lhfscbtd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ekviaoqf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2juxtfwuf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ghaasrus.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yafypaeh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2skwdjuse.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2amcknkne.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vxaqsesa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jdfbmdmx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rwbxhicw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hjvuyuck.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hcbxgshy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvwrwtyx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zlsmwvte.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgxnciv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2apopmoau.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wezifcxt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlylynzb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2skosoaxc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2venyrkog.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ghtrhnmi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qqihsojz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vbzbbixe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gimuqrxm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2joliwrax.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2geasfcmq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ceftsdjt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ghaacuoh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkpnwoec.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wuchkjqa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vfmxkhwy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cvnekete.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pevdcapb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ymtwakva.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2efyseksy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zczfqhjz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hjvkthik.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2oshluunx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pxdvqcnw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eldlgriz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtibbqpt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hudpvucq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rbadwcvb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hffrmszb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ohzhklus.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ubcjssoj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ahxufbpc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bbteahvk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lbxxcgnu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dmuygeef.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwxhuqu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yaxhpbep.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdeponus.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yubtebfs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tinllmyo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2svmgmszw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2metinzgr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdwknlo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xrosloij.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgtgaklk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qirfixax.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2najwutws.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ibhgydvc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xzulkhlo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qmvyhvrt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ycptkqyw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qeeflunw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wfhifbdp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mpjiywwo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nldpjbvr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2avhuuonr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tdmhnlcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yxatcpzc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2brgwtyim.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2sxdccjjv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mswlcuxu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mhzwudsr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ashonexw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hmqedjca.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ccadkrqm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2powhyqvr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ttyvqkkl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wwpotvli.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2whacwqdq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mssashwa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2svxdwocj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wmkuygdu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jsprrsff.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nytvuxbi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xipfxuxd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvluumbp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kmvwfkoz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vnjwijcb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bymqjbqu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nksecqlw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aftxzfxp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2njvnvftl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ucackhww.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qeinuneo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tpqupqwy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wchinlxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rueadrug.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2krefeltb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msxdrcmp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iyminobs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yoskmeib.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mptfaiji.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmkvprbt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ogghcvul.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bckoyopb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ewonxigo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rxzzvoio.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mrazdalp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pwykobky.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zxklmyiz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fxneqotl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ajexvrea.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mbrdyltr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivisjiaw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmkfvur.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oarkmrla.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2akhvtmfp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zlnaxkwn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ozhhthfn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2urrxfdrf.html


<!-- 参考信息 -->