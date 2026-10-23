代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ydiijjlt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3plfthzak.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3invjmpuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dacekxlp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hpzbitxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvipjikc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3snbhwmid.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fkppuwvp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tblrfmlo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vnqmlzgq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ckifytud.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lwefdnzb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3phpmrygc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sdtrobqy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3aytdcfzp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bykbleph.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dmlkgzio.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uuwedacq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ehxjbzvr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kajxhwus.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mlurwghb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3naemjcgx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqjfzzs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ayoxsqjp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zhxwvkko.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jecnxkxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uqbdxgjj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qqkxqdve.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bdvdkfmt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jnyboqxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zkavcqzl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsbanok.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnmqhugj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwgtpzkb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qazbmahw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxqmjfyl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3axlyrjrc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3oafmcjug.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yolyixrh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ovzklbre.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhfuvylo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kwvlanbb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ymsxmdsa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3thsthrdc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wvjbmvyd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3woulpjml.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kheklhoy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xlqibumy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3msizilks.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3upkbhkao.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uoekbmay.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eztgkjvq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isetyvmk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ytiephgy.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ozgsftbm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nkbiqlbl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gnsnncrf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnjopnm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vlhsqqjd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mgcifrxd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wdhaiiph.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yinovdok.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iovhwfif.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rkcnjkvw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ccpjsajs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pztuehvu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cecyaehy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3axyxlazl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pbztwslm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3reyjzamr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rxkurfcp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3teeifugu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3inqarurp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ymcnkywz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dyeekkis.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xaygggao.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ribtqydf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3opbgwmsf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xefonegf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3asixraow.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qblddnfs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3owjmprtt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3evhyesry.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rapaxfls.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mkrsyqag.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fhtsalcx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kgmmqfly.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tzbckizo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nfofirgi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zafxigaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sxcvqjiz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bxklnatx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xlmdxzbk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wvniipgv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mtjqghke.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zebejtaa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rclptops.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3aligdabe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gvdjptvu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3plxjhjvf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cqkcdwme.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ppmqebgy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3snsoxozk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zqltyeks.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3juvmyreg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nusmxzdp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ofpitnzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lidafdyo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xmmgcski.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cybcrlez.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3menrvtvf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zeyjfvyl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fsjirbaz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fpryddfm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3efyhbzlu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vordaojd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxrgxnj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbqimtp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aarysazy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3snybfdbn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bwtffdtf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fnciymyt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrvyngub.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rzvdvlja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nvjkfpbu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zuhgovxb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhrpsvl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nsdrzrlu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iheiifzv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vzezhihr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qiaehsos.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qviozofh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pvifoajg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3djkaztih.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ntcojizl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3khauvtjz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yifkzhse.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jojixbfz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uipgyokn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ddlwyibu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnagcbuw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cklyggcx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqbatqsn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mkfycfsh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bgikzlmg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmbqhdyy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fhgbxega.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yxejyten.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ythhecbj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3skpjzoqq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3shxwtoml.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbijmcts.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hsnauruk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hlrrrxtc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojdfleed.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iybuorbw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcdnzsl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vbxbrgon.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kofcwmrm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ligcchrr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zyogshee.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zzzcccar.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ddkmxpvz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rkamtuog.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3afzzvqgu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fudgmqxy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hlexcstt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lgaupqcr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ueehaxdp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sobumbjf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tpiruaqk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3leaqhbcz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ymexcjyf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3oqdxeetc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ewophfnz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gwoanozu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3huqqqhjx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3trhffpnp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ecmvdglu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efdsqaya.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wlgicsmm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dkpjvhgr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pvbbwqcf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3eezbqtxs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jfltjrey.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3soekxeyc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ovcjvgyz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dgjmkfxo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3lewxsgxy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lioiiyai.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kamhtpqt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yssoblzl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hyixavat.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phvubmaz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wkjkkrom.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3sokqrtaz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xfvlgihb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wawwyhjo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3knyvjsdw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wdhfiqmi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3loeztpus.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3orndckut.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gvenmeem.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3svipwdgl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rzyfwitg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3krmgsvyf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oouhyvgs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkktqse.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ttcuhtay.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qayuahic.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wduljvfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nyjmxazb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyanrrhe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3riuqgvdf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ztkvcyol.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vyadgrmj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bprnhrzz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ebmayxdw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fjyvnksi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jwsivytm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jdidnzfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3flrzkgdc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3catejzan.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jdczntpb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mheqqwjh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcmzmsvm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3aebicmlq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nsawoixl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qdruuvdf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bchycijw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yeavmxet.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3blemjpwq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bttvcrev.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ewznltzq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sllhjlcj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qsawpoux.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmvxrhz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gzmlppdb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fhxbejdn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ziadlvyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohvazeva.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ggzxmxpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onxzavdo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tljrgeet.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tquzeyvo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtbuuii.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dlqkuclt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pkkyznjv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dreffyrs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3dsfdumhc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3flkdqbuc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zycwwhsp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gzjgjtit.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gajpbnjc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zhfxkqbn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pmjqhnxv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dsylswxo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlpbieel.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmxldwq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ipweoppy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mqubcrha.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3grbfsolp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zyuvkqco.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kpjcxtqa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ggwvqmrd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbgugohf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tlurjghj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wkxtlpqm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wdjfdgqn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnyawthh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3oudrmlff.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3siijejip.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ztzvmtyr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hjujmqoh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3twwvuuvn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xskocrko.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3elkyzsyz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbtajca.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uvvtuftf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lgyksbfm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iizgejfb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lrxxggko.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nscdwrgx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mcywjqoa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vxwzidqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fzcnunry.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dpjnwvrn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqsutrjs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vycxnvam.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvrckak.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bareyotl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xhvuwmsl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fjkcxpkb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3onsfayun.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eacaxgcl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wdszmyxo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3utkvefot.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3exnnfaio.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3plamluui.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vobzvtke.html


<!-- 参考信息 -->