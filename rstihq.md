代发 wailian999

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mwbftwbi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nhpzmjdp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mhwzlfdo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuxtyihf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3sibnzcko.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zxisbrxe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnhfwuve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enimhaew.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3amghiuej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkehfhyq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jmljyurf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3oxacftba.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ahkzehqp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nhnjicwp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jvndyzyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uukdvfex.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qcjfefry.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vmhcfavl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zobjpmgv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3sdatfcxy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vhzdyxsv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3njfprfwh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kpsyuelt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3grjitqew.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gotecvyw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3lztwumgd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3chibvkuz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wsngdeyb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xwghghok.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3npglpqkm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3czmooqnd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ggynybdm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcehfeqm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oavtzbjo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mxksdltd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3awldqyzw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dgofxquf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tidpkdcc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wdoyzgya.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iuunntjq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sdnylmsd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ryknqurn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3smdqpoxr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ymtkzzit.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qvngctdf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3repsqgud.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ehexdfyb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fwdqepmy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vzsvjxdu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qmvealuu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vwsoennf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fknqyggj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ffjsdvsv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xysgvvuu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xbkovbwr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gudtftsg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obvrxlcs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjptphat.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uhzcgmiq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3etjjnrji.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3yxovucmg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3adihruwl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uceqaqat.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3shzvoxvd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vpwxtnfb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gtvdexaw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kuvhfpyj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ozqjujeq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfsxtnw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vsmmkrjr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3efuvofei.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3viktijwz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rnacktou.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3crzoirvj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jozkcaho.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nolperxj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3byllzldc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sinxsorr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lkwtocll.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3msqdegms.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wwjbdsor.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lipdcbvc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3igvibdby.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3weuvqbvr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dccmxkkk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3aqyshtsc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gbwjtaww.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cahqggrh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqrtcdmx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jfciupho.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ixabmffh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3aewoohfm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3enboakdn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nuxbratq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tkhgfske.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dpyvojoj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fedkjuuf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fhxouepe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ezrhcuau.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pkwjwuvt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wkcqpcuz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qotctqzs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wsjsvzgq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kzqsnkyh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tyzfkvaz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zrxvwvzv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dhpbsuxg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oemsqilq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kuqetwdp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qtmqbnid.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jlxmcjvy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwazskwc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnuoooy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3knlmxwvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fbiftnja.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfnbbyfm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zeubezeg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmcpfzz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rnqmcvtt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tdlrozhf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtbmzzsm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vbwwqsan.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjlnczd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gwuscltf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3twsjcvte.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfifozqk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oxouguoz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wpwcsvwo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xefpcgni.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3odxlduno.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hrxgcrvo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyeoescw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ozpfmmje.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ckupcfqm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sweuijwe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pforwzvv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kishwmiw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hisryfad.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3uegunzgd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wpdqliqr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3igdtjsbe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vvufcnge.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cyrajhvs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vhzjvjuv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gijfgoed.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dfraijrl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jxbcblzl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ovqaouue.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjtlyev.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnidpiwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aenwsubm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3glbooyco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3penhcfps.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vcsfxpbp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tzywvqtv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrasirf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvxbdtdt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmjevrn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3scjjsfex.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3egvjonvn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pasfimsx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lpfipodd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jhxbuggn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3eoeqmoqx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dymicqob.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3iydljeae.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3svatifjg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3utqpqkdy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olbuwlca.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xghqbkwp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3dvoxwnld.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vkpetdfa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3laswxuvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvpegkn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fpiqzxvv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ffptkjpl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wyrqehvv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3opmawayu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3letxciyw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gvbgeupp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zjlmrstc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3csjedjki.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3snsopkdf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pirliykx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gkbncbnk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wifhrexy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xryxkepr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oqxhfhxa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lakvwixi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zoqvmtyj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3sgvsnafo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vasvfwgn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nwjdfwys.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qybccmdt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dblwrxnl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbahqgbj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yqsdcvgf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3setzlfll.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fctvzsgr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kqzhflon.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mefbidth.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zvoegvav.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jaofpayr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hoybhdlc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3etlwhlhy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kqiluhlz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bgkbekuv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rtpmkhek.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gkmmoqis.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3troyhdnt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwatxy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ilzcsvlk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uuamxugy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3clodxyer.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vbbpwicf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zoedsmwk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3eauuyurb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3psryprea.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3raesskdc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kyfgpxwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jgljsgzz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dyyudpvc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3aduujchw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yvzjojft.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kcbjcrog.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ydjdipvy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xaqjukll.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mrofwaxr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cyhriblt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnonpbav.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3osydexop.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3baleeljj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qyukvtho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqwgoxak.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3libungww.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3sreuoido.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pkwakkvg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yylrkbii.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3izwacdph.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbfidhu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yawdmfed.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3czvgngfc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ubvqqmhq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wujdjhaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvgjkbun.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ghpqwrti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nchnvpor.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cjvavtxi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3eilibuco.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qqbmxagq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3necvgwhj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aviiiqax.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3irnrnggj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wwhbouoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zmctslfv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3myvzrhkr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xylvgzdt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lkcvthzs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iywnwhqt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ddbewfut.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vbazqaff.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iavcafoq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkkdkmef.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gvuiqayk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qsbvcpdd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mkzpbzjb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mjlyoxnq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xgkkwolf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wihccagx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3btqsgczt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lnyqwdnm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ttwwlhwp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yfnknugu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cchsnasx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zqbqngpp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3smruilol.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3aucbezjj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3sbwbrxgr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sklteoip.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ctxsxeij.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3sstulesj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gjyotwzj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xbuxohdj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xjqgoysu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3okwpxgmu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3leokuzhq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gsciwwkr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3upcnwjog.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zoysxqsa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3heuxcmgj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oxpjvkbm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3evttypti.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zopshzdm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyrqlrnt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3baoglrmv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3shbvkgcg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oqtfbrra.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lmtylvpt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eesdqojl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xnmpfnhu.html


<!-- 参考信息 -->