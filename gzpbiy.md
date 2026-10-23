代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zayptjmc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pabuizwv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3aziuvsds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yljpeqew.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nmxdfcyl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3usrxwabx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zktzslnp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cibeyoen.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xximpomy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3biptezqf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vjntadvy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kevsfnjl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dlcqfdxd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ndukxjul.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wgxlcjat.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vjqxnvul.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cyjmhvpp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfuvvfvf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zvwyqhad.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hjlpxbph.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zezzccch.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sulfgcxz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vqnarkwt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hfhtarde.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3glfyjyaf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3emxqvtqi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vgqqyfkd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qvyvayfr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3meimqzve.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jzszlvob.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kctlmjcj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3addhwbrq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pecncyxh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dddvcomz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nybxpdjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujqdupsu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dfwixogk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqrpiseq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hosmettc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zkfbzcti.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lfqsglmp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xdintrzf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3awkwjjbu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3oblkmpwe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3mbqjijoh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uktwtteo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pjxurequ.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pszhyssa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ffbajbmg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3grqfytgl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ldnpuvre.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3loednuqa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukcgaszp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3elzngdph.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qdryipxz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zafupdyy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wywtdupz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jibifagd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqrknaq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zaoppijn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ccppmdne.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bxrxilac.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wfjfyach.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubzibttb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bcdjarof.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qmparlei.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3sreemxpn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdajczp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jdbgppmi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wcwalbac.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3knfmjzrp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tcfpvvxg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvjxwpok.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bierlufj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jbgxaffk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kfqdqwzu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iycvkoow.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wkepekky.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kenneqyq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3peuicyyu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ubjdgxdu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rxecsysg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dtpxicet.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lzghkckx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbypczrb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3znmynkvq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3enorpkcg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ffhxpjdh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wsfmbshn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dbqrqpnv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lmxpevik.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wlxqnvha.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wlybwtae.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3quzixhhj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nzmddnbr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwfgcesd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gsoacnjh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvuldsfi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qeojwvkg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eutxbrvc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wvgkfmdf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3giipvkbh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uftneueo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3twkpzjpk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3einnbizh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3yktajuec.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3epzdydzf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jxhfzcsf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ujliuhei.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qxdnnwhe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qhtfmypf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3huownhqj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pexzkmna.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3avmdcaiz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ihiuonnl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pgmuvawx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhqfduhd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3njwzeysx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3belaseyw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bjvwdons.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwhqnmh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nxeileer.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdifqkh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iioxtgqn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cixexsie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ahbeszdg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3winujojd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3szvhdpfc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3uhallbht.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vjhcmmlo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3opvcdaaq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xbtoeaej.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pplwwpdz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tlhkkgel.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyanxnsp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uxajumkj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eyropjpy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3huyjqyjy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ohsklosv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vqdnxkwy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mvulzsjz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3knifxibz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ocrrbswf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eunxgrdq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tamrshsl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fbbrvuxu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dlrboenx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zyhwzych.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojccomhv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xyojpbyr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iajcfxoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nbxphqfq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fslipkwu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lyxzhpjd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3efhvewbv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tbvykgbv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fuqsxwyi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkexxvgi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ajmjeulk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrkhbjj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvskiydr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uewppudf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjwpcqwn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hrprijrl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3akdsazje.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3althcvds.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rfvyxdkw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nihunhmd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fpeiksew.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mpppcmwb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ykzrtkob.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iljoynud.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tudcrhuy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jrwzatys.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxetqcsw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hznsegan.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amozvjtg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ihuipbxz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gyyxbezd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3urnuabat.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3koqbfzjc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xvvfqhok.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qjlvrkxi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtdsrciu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xjahvskm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oepgkhuu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3recrdmty.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vonlwxwi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sspsrulz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yiuhuqop.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3uwpqcwao.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cdibqpst.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kvvlwydz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3srwbdcaf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pxdhbuyf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dbywavww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrqoibnd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xozspxrq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ldnydqho.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ktkmseid.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vxwofhvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ajzrwttv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rxgxefwd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3esnnvqsr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3palglbvx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ptujqugz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ygcfttne.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3cmbniqkp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lwpyacij.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zskszylh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ppqvmtae.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3skicyucx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vsppabqt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yemcezrp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3napwawwj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tkhgpflp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3skhdxhhd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ajgzitcz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3agfvrbed.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jbbmoghy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ekwjsefu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bklqhlfe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxvyklt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vyafdrwl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzfpldck.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ugufjzcy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kgaoaouv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jqawrnoh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqpjvdlv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qsapzfuc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3osrweozt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jzaksgtw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3diccijbd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ayvynhfp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ffanglcd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jsfjiouc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hldoorpy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zlorplpw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3slonltgw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xuhhjoft.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ismfuznu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sqihghfn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rzveirxn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kdqtmxht.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bnhapvuc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3icseujtx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vodjxwsp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kfmiqtez.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bgixznzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fztwtyit.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dxhhmtam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tctdqykh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yekxussd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lxdmltll.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yogdczxf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3udhjjhyg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bjnyoauu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zzurqdwj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tdufndin.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kxnulrzf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gjyoeiqe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pznyzpjp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3etzvswys.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zciljwwq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gstdwpyn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wxwcahwl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3awpwhial.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zvwisacs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wtcfrtcd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tyehvzmn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lsrveodi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yueatxwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnogbzgo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jahozozc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmogbdee.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ujhfxxga.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3eoaufaiv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3imnzhcuq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bugdwqsu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zjxxxxuj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dfqkraoi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yicqckxm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yowbusyp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lvhojiqt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nayyhwnq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qbomebiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ijrlszti.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vgwmvycw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnqyubh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fkotwbdd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cvkoevhb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vxjagdbr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xioplibm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sidgyqko.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zuzyvjtv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mphlbqca.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jqtqspgk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nadzxtxe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dgcbaymh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jonixtrt.html


<!-- 参考信息 -->