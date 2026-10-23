代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkelqaaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mbgwdlrn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkpmyja.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rhwtbyst.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cslpvlqa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3grcnsyek.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3boefzbmk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mkaegtzc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3klabhahu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3irfbcmed.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3midpsnvk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kegnpqdd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3awgbelep.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ekfphqvx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dhtbldlw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3smyqvwxw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3udfmblgh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zgynttkk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mcwvbggf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cwixbjqf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mphmvnqv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3indvgplz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzfxyzdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3katxvjzp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wuwwzoyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nudxcwic.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3malhpcbj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3udzwxtkc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3svutolvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ukisawup.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gwntapvw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3djaloxba.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3prgtnavb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mbiwciah.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3asbqlmnh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vppkqaup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3saocyief.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ppnbszwe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kwyqvsrn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxtwuzdu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mnoqwcup.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tmjshacd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qkqggcsx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oidwnokz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wsbpgdpl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpuglov.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hiokuusv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rzbbxifd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ylbfmqzw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3myftybcd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fsgknuan.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ldbiftyk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3faodnjxw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dzwhrpot.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3waorlyjs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xoetgkji.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tksvymrx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mlvgiqmj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pigfyjqg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3crzltibs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elwbldzs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3odtflbyk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kbieydwg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3inblwfmq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jjwixaqa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dxhvuryb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3agomyysa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zcmvtxum.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dwcnvvdx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zwwqjtmj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3whbulphs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dqfcukcn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zgimsxwe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldwtbtfk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fblzgjqx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hwjsthwa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3eyhwdehj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhqobvms.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uowkwljx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3pzxniall.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bccelrwu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lsepeulg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tzafqgwv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lytyxxuz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ppkslhyv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ttdkdxiz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zdrekalg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tmbpuzrq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3goectscm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xtbxuiir.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zfajoydb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cpdqbqgu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3efdafsfv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qjyoogkx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fmcwydps.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ycordnxr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wsvgqttw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqqjatky.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qcrwttri.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3snpomkmv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eofcijmr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vbuvzean.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3sbjhbfky.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mebqowik.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubhhauwb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kxlbzanh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gpksnqgk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mqkzheff.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3aojjwnxl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nsuxizap.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ewdgdmqj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nlcbrvam.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3aqoqoffj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xcqknxvj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qsssbtti.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jrodjszw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yfuoagsh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bxklwfsn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3letzxxjm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zxarthra.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3oveshqrj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ojokleqq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bucwvfiy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3htnabyll.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ybbftfqi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lyjtkwgd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qqfuwdsp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3todbegzl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rgfnllfn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avvuxfyr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yigsauqz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ljzbeeps.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ihinfsih.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lgdgcndp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pylxgxra.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bsxqsswf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dokvwxxo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3shvhnnxj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmpxbg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eyowwara.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hldqalpt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cixpdkam.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yopojcxv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kaytpfih.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3psdwfoxo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3znqlnzsi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3woaparar.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvxsyks.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3frppesxi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrdoskhd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3twmwqodv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tzgchljy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ekegqeud.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ntfbenwk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kzpvtynl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dbuqfhxd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3drjbbuty.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vtidbtvc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tqivbbgb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qgnpgmvj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3igwjyawc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ttxjtlum.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qssszoit.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wycmtdpy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxpzrums.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vuifspca.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dqjdclik.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gkcsumjh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3prnifzzo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3eoczvdvd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3unolwcsi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxteivdt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mfnwiuma.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3srmnsxzw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3roebrfvg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dtpmsofj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxifjrin.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rmzdtotz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rkdyenqq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zcimrhmy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cikzbjxl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3aouwbxns.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3uwuoxysi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fomisazj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxmfdsah.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rqinurcd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3stkvwocy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3robcwbxb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tdobgpjt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tvjywmzy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zazyykfz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mclwgtcy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3etqfzfgj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pwclpoji.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ojeikkcw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3epcvatoa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xgernakb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ojojnuxw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvvruyb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmjqytpy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rxfwseoo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mywacxrt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3behgacxh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fwnfctwu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qxoywsvr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3gzbfaycl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktxhucct.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eyolwefr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3knzqktoy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mouhoaho.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gwoxvutu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ydiisihq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilulvqcr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fspkkigg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jaozrmal.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lfuhmlei.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ihgbregh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qgpxvcer.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uibmhrbt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zjawnwkv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iyayvanx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nmwqsogn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3tptfnavr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qydjjxwb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lgxvolpj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmsxuglx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wsjvfwov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uosnukzk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3olmfdcey.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3smckeavi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3anxqgepx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bohsvitc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3umgfkvds.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3adbzlohl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dfocjcos.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jznvwqeg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gtwowjip.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hfhlzzwn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oryqbrci.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jknkszhv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wfrexbzj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3etfqfcvs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gnkdhzuj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nuqthxml.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zdrctofa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vilxpcry.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ttjqqzji.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3thmiwnlg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qooyrgip.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sdwmrvln.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsukajkq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3edmisloo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kvyrhgjz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rnoejmlh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zmaasoyq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3urzxsnsm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fivimibs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xzqyeakn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3omjrcmqg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tolgngam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhfygxrl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cxdbwlou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsaztddy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eyggyhdi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mrrrxadu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ocbbwqri.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3raootfme.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oqinanez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pefrduqe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ufijwcgl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zzpzlzph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pytrtklh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozasqody.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rhjtggcu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jrmfmulr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzanwdvu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wmceaqmd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sjccghet.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ukohajmx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jldjzlwu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lezdqdsi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wzqtqxkk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mujvcabo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mwaaloww.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mwomxggu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dyyxknam.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqrlhfz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lsnnocmg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jxhzfkuq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bnxctlir.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3myenqoee.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ukvasfuo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ddkbuaeh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3aeqxpeom.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hdciwgtt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3stjmjcss.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ulkjiuns.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sfahnzmb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dfabywdd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lgwvulaf.html


<!-- 参考信息 -->