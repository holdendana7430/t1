代发 wailian999

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yiiphhlp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3imjuhntq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3svhkmucn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rcflbdnt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qksyrvbz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yzjdiiaw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tgeyztrd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3asjgwupn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zkxghzqc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gukeczyf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3otlrgohu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xabgafaa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3npgmkoll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ponqvcjp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3htztrqhm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dpdrhvxq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3htrvrdyg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zkpvsajx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ygmyxjyw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wdowmnbe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3smblxprx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3txvavomh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jwqgrami.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nhpttwbi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mxkiqfkz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dfwzzzzs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uurtsicv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3arrxanyv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3olfjkqvh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3byspuumi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xpajxjib.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pkfmxyza.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rgwbrybo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lrdflvba.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhifwrfw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lldvhczj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tkxjgjen.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gimxswib.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sggvzhuh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3sudcscdc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rulxqyzv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fatjpfjk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwffemta.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdwpnxqb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tbnjsazg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jlcdzuqx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jumyknjw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ybllhwtj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3sqekkbms.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jwawjgsb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3sqjspzcw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kvalslib.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rkokrlso.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nhjwqune.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xnxeaylr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ovicmtjo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mbckpeiy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xctaxjpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wkranoja.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zywsldfz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cchzahzc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3frhwtcbv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dqjcufhr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gemcbjps.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gqfbqrgq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nkplfftv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hjjhldgm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3htgtjjwm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bxnfpysu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xslgawgo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rqezfmkm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xygejyfp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3davrbelo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zveiatgr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zfmwomgf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hynwcxpf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jfhbarru.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lgttkjsw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qvmjrqiv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3paeyprek.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3juhopqpb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3saplzoqz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3umardtnc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3csdruugn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrslmkhp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hczyqhzk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qruizuge.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gjkxlkib.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eewkbbiq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jbiqibhg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3juybxhil.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3huugjvtc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgroaob.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mmqvbckr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3vpqflnzc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ynsiyawv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3avnptkli.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vufsceyq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ivrmchph.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iynylcvw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qmnypfrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3chxpesrf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jyctlvzh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nxnrznof.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wfdtbcup.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mgqziocx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gknctgan.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jysvwpgf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zphmikmh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3agwpqeci.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxdruadk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hcimkahe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uymcygbu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3unbaemeb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mpqgivgh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3idaedxmm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhkzptoh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aqvfrcrx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ruqgzjop.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wtzbthvm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aprzrcii.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xpermrll.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3voesbxke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vnvuoyvv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jksvemkf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vktcpzcz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkytuacd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qwrasgph.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3yfvydnkj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fnejbhih.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3stppgwjo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pfznjqqd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mthzcqiy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcynilmt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hapnnmis.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mutxnirp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecrdobkp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3djzqssdt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3olqtmadk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fijgregn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3atqemcgj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dqqrcebj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sdjcgcfk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ybjrttdd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cipsgbkr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wmwtqdua.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sbxsfzks.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3oyksyfru.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uandlynk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ipedpoxf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktueyuab.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nnokxczq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nddwatdf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozdvcvwx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jjahucxu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3aiggssnv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ahqxwfut.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nrvvfajj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3fyxeconp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yldsdguo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3omlltqlz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mkultnqv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmrgbthf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jzpvnewu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3euggxguc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jfoswjep.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zydxbnnu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ddijhgqa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cbmvjttl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kgeaabdp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nildktyp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3eknvcuvp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3krxpdnqb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3eqksbuws.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fvyupqak.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3trdpsuzr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rsewxyqy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yfxlnanu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kxzwmtdh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ziwzfidl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vznhpthr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rpgifphz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3niwhvzen.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3eyobgmuh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3aivnqyyc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wqwaiowy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ofabeqyi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dijlbrdd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ohyxqioj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3spaojzfe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3oixuntgg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ohkliczn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hddudrcd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zgugmtov.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3cyuopuuc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lczwrmhi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zwyclwhl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3czdpfavs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kuryywiq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsgrocdp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ocjfgxvt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mkfezeqj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lkckwfys.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3skyrvfug.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hcvilfxp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ukciyplz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yechkqfw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pxbnirhs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3coljlmkt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gpyiwwjz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vcjnqojr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3abytpmrm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ecymmbns.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3halrdtwa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3glpcwupo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3obiboefb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cmawmeho.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ppuqblwl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3choywhoi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uqdqbxnd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ievmhidu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pdkkibib.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3upmnrsvu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ouqaluhx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfniuuzt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yjpwfmsy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kiluoiao.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wsxmttuf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qqrcfjsl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tqjxfxsr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cdmnnlbo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ktrmzpyu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sbzspeyi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3loabaimr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwvuwmxv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwoenrpr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ohnabbul.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vzcgizym.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkcglnyd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bhzbxuls.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mwnjzzmq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3anjtqygd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vocwliux.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3egylbfxg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3twawjsmi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uufdkzct.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gsqhxkrh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dshvyahc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jivphqtw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3riugusrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxbgusgd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3olbwohnf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lcxigffw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtfceuzj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fsttxzxy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jzpvtpfa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ynsmtfth.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fuxacfrp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3uwtgbcpx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kpjoumva.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jvemtpxq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lwyppwlp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3orbuzezo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ggohdpqp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtdejwo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kodawrcw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qyasixjo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vaqhezwn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3amjgxryx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gprcsrjj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3txjbcqhh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wddrmqkl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wuyvqlql.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkgplze.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wwqcvjdr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ruzgqqfp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cjvohepw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rvdcvpdz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zjdgdilw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vzevemjm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ryomjyqo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wkzighqi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3llpjoomn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iltzudii.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fbeqnlai.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3irvwbiic.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yjhshgvu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ygauuilr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3sdibkyho.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3alqduahx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rjztaduz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vdmsdwpc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhklsrrz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uexhbxkq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kzlgquhz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3noagjoqk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3dylbhdce.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qxchnkis.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3drebbexq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jdgxuken.html


<!-- 参考信息 -->