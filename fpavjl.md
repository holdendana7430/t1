代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kqbylcdj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xpqecwgo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mjfjdpxq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3uyswefzm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3msiebktw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ejmpzgen.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3idnbymtg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mdczuzhd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3diseokoy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvvsmsfo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cprvjcgc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rstqmziy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jdszwdem.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cwydwhkj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3reckqgmi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lhyeapxl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3impofioz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xakqdlnu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3viyustna.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3onsicrii.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fdosljtr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vfxykdkz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lyckutxw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ftpfyzkj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3guujgyvj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lrpjfrqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3nqybuqbx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3llapbtin.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3higuxlpx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlsudkto.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bgcjedeg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3csugpxim.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qejkqnnu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ctxkxieu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3eupjmilo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3igzprisz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3methjvnn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wgxbzzvp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rnhpswfd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nujbcrre.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jaihsyue.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkqakxkn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ldajgigy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyarbyqi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ujvcoeea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qypcokmz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ytyrhffz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yhjkthis.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pykfeoxj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nlvumlac.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ngdfkfuu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hezmmvbo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cxxezken.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wmkcesoq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pqsbtwbv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cmewmxnx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3iqnznzwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lztqdtir.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aegpboht.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3letoeenf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhydlsbk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zhckblgy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzscipz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vyucniss.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lfqiejvj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwceqojt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqmkqwps.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qtjdlqoo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ardqdpmr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nqlhotwo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rmtpcmgt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fverklgh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hdtukfza.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mwbujaay.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufluvncn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdxqnury.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yqbrmchy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kwdxzpzg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zkhzwisn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3uxrfgijj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uptllsxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vhapwhhg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3avyprvrv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ebicfozq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xictjpke.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zhkztooq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3enzkajxh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qwewcrdr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cfxqbibz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aiouahnk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dksjmybg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fplmwudv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkgopchr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pxjvrvjm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rwvuwkih.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pisgjcjj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3yyjkctnk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxtosei.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gmrbolvp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qofgqkxl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ufnvhudh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oxbwhevv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ymlxhvui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3elhcvfdd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zqmcoajv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sociymmg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hdbnilui.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3urmmoxdr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yftqdtjk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3omvxfgeo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwauicvz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mcovvwei.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fuvjgbkc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zhnnipbx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvfrhwsd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hbcswbxa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkeuyzbx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jigznedh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vrhrsekz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mfsfmfjl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbhejdly.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ckggezmk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tsvnnckd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3sdbajpcc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mshgiitu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zxmnrnhr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hlffauqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cxxkhegs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jyrwpcti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ztcqnora.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xnyhutgf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iycycgbb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wceaphov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nhhsvwtf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uoghgpxh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3reozeiyn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3agbmpodg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dusqlfau.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yadojsyh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qlijswfz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uwdsbadc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ggyewhyy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3znbkisqj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xewrygfb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3csabvlvz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hleebxyq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dnpshhmu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gicytmfp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3escwbcmz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3erhbcaol.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gvwndlcz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jvozvppc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3omfombnc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ljtaxizs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3roatjmbc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zhpsaals.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zxksbrgh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxubxjb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtlzrgr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxriumtj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hsleqqng.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3drsrcwks.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwmxwxcj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3otnszvpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3frtycjck.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ocqnsmqq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xregsopn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jnekpyey.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqehvunl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hvipkovl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqngdytp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oshkpgok.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eimzpftf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3enshoicy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhbqdhka.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ctvtfvof.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rxdboglm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dyqaolzd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rrhcwpug.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pabdyxsi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wajbbwyg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fsusmolw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3euzdrsiy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cmfutiub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3evaalzzj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pfysyhlj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gullqqsh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tbxycptu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bgfdiioy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sfzfjbkr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kqacwvfb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgucmxl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3olkulwwv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3okqljfbq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zauuouzv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zlzeulrr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zrpfoaoo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wsukczty.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3drujwrae.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nvgeluno.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rcifztcy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mjmaljzw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qrmvvqas.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yyvzjzmw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xcdwtoyg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sqhvetsv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ttlzlhss.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzltfssa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nqvbrxba.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uiixuawi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ncyqjqhg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qpucznpz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3slrjiixx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qmfchkgn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vmcjaual.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sadesnek.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3apunsfga.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pppvqhfb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxbshoil.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3owgiault.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rzdiwjqq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3udyyuovw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bikqcbbe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3byngocfn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fnmszcak.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fgdqoxvb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3velgilia.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wgftcvrn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xpbdrbur.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyzxjdm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zheyaaqd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ngsukqft.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tcyebpgh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vhfgvskg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhimtid.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3immpduew.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ntowgcaa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wvwdifpq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olafocqo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jyupnbki.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tbokbumy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yvrpzlsf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bqzitdmd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pmnvtclz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fgsiuqzz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jspspqta.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cedikvun.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3strdwlrq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dfewrnbv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pyesipjj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yzqlbkfa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sldavlvh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsowwbsp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rwvgxpgg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iygjynka.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yxaghejz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ocsvhuan.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ernvrwlf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3warjatft.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xeujpieo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jtdjiadl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3trrgovkf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bzrbecpe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mdduptbb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uvmznhpg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxhyjoj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wzllibhq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tcowsmcr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hmhbeqog.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxdsouje.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idvsawbj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fpirqeqh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3inzuntjl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmhyvqui.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wymzdiej.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nxudcgkt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jcwojszh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3myvwjmva.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ojedxluh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xgwcwabu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdkkbmjp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hvkwqyme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pimjgtwp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwemaeod.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xjhskkqt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3erznfhwm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zjdbtgco.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jxakyivq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3berfpewk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gabumttv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kigqfsut.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmmflzbv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3htdezeob.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qbufupfb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alghwfio.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvxjwjow.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dzaklaly.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iikkjhbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdftmmpb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3inojangy.html


<!-- 参考信息 -->