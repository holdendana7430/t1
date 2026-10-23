代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ykfdmjff.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nlxyvidb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3orcqenrc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mkfkwrbc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lisomeyu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3htprjjsc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ycssvvvm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xmgsmvoj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tayrtbdj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ihobfryw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rhqamlof.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vawevsjr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdodqvfy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kqxyfdws.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fbxmuldb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nykyuvcv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rvhxkuyx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbwvynuv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xhldlyxo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wlvttjwo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cwxyruws.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uzhngbhh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bpfdcoeh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wvhrpqik.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nsaflbft.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uchkegxr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nfuqfzha.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zlvqxays.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lkzfqpip.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ygexpqqv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqflabqy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jzjfaawm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fsbxhrzg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qrzrmpza.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aeoqjdxu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3njlxmrqt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyhmztx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tzdhquua.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eqhvojpj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lbvuhjzl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwsqwbmk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bzueyitp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hnyqnwqw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ubnpogcx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pgtavxui.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eykzbepd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3vujcllqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qqssgmnh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qoyjflce.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ipawnwal.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgtfivf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fbwvzakk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lqclwdhe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nuuoztcn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ummpjrsy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wqeokmuo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bzbjxnir.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3arvjfxhc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxxqhaeq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cvvgztxh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hgsgxcxi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rxcctkvd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvkzpbes.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ynctysgg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3usvyrfll.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3teoubzpn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xpkdymho.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iluundlw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlwciexl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ilixydgl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mkwithuf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzrskme.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dfdhyawl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3mpvnzlru.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wcexmhad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3oabriodv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dcqjecsw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3axfxghfw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3anusogfu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckvqgwmj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3idvtxtti.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pfjtyzke.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pugghcqn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qkuthzax.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3domriavh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lirbmvjc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ytputgdg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gobpfpcu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3azhiqwep.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gnnopssc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ryqpqvhe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fozhckah.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3naxrmydq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cvgpceqp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfguxnia.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hmzyuhqe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aditcgoi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qzoqpfso.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xewlrupe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rsjvyelc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jsalfgmf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tkwmieel.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbnzsmzw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kgpgjaea.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rgfbeeid.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjyqexh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xdqfzlhf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dpfvipfc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jqfaupad.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zslxmfbt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ykwndlcn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3woxacuwo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzdaiotd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3werwrjxn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3izpeifuv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ctpkjqnj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhepggtj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xepgeorj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mkdbhwbm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ynrbvvlu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yqgdwidr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3veoyvqtm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yhpzqeuj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hjpdamxk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xwnewsdb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ufobnrfz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vbifkhyh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xbcbitlm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mkdiiyyf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3psbicqls.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nhdsqhhv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sngtjcqq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xalqsrix.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yygltxml.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tlucvctk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3znwtejrs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3evczmqei.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xzzvyswo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwmrqysq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hqbersqu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zoimibjy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ihdxxmut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pvtjsqdn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3trrnseaq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gyygcckw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mokxxwbe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3utvicrsi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pkzkqhnt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3knpkpzib.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3btzaarbz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbwklqg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vihucpue.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tiuislza.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhnuola.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxojvwp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lfvgkvad.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xabgtedw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bmpsnsog.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbzfkwvi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3holjikkj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tfyxcpwx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yykdrwnw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3atbubntt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zdpvvmyv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lqtqhbwa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lnvsgzdv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sqoiarwo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvpkkaq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lremtuhb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3citktsst.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qngscuyq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vjktsqqc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ifsrdenx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wcxclnnu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nbvmszkv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdjkpzom.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwjfzn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dzfwsppi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rkmkqwbe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lwaucbut.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gbdvjbxc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kfrodnif.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qpmthkjk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ecfqfhvl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xlgybhiw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mintugbw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3autdepqp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxizql.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mavpxyyp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ltwyjdbm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekybycnn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gfdjodtr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gtwktrqc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tlxqkqce.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wnqbqlsg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rtcpbjtw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xrxuwpyu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opqrhpid.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yjjecdql.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsljtlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoyokpmu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gmdulkjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aclyrcmd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vikpnpaf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3drcnvnkl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bgzedaar.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vzozkigj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3utlzpnya.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3eckmaoxo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ficovzcm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gfhqdwnl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3awkfoaaq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpthdmwo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mcnhyady.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xusszrem.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zyyhyybi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xiqtoyiz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwishbf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bnxnbadb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pfrnnhep.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xqdihyfm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jyxxagzp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hjwfsalr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3muyvtqwh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3byvrdiiu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eywtkdyp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3efmmgxgy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wybzszrs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fuclipar.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnbxptj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jjeiwexf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3joihmpqy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dcndpvje.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wyvyzkyb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mfmwpscw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qiikyuoe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fpwkrpvq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ltamcksv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wdclhomc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kbingyyw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oaozvjjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ygejsvkr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gvgjwuvb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cxyscgkn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lbbgrtds.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mceovife.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ynorlgnj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hiywrqgh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uscioisx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvwcpfdd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmwszeho.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mgjkjdzl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rehnzsne.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eodmcinb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozklnzfm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pznchxyz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3loxiijpn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kzasrfsv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tqiuwcmb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrqdkrug.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qvuwcyqo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3blqqxwsv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3sbjzfgzi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3umraqxjk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3esmhcuhn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3epqtkpgn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ykwiwnqd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3axahejph.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mjpgwpid.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nkxjqscr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zhlqtbvi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rnjfzkvy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dklrghoc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3didcxgau.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvsogwo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3pcokbxkp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jcganivv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hljridvh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fsmzujhe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ryymdkzr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mnjlhkko.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjyuxfaa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yewtowvc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tkawtqbn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3auvbqbhp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rlthzbpo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mmudqchl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ubbppodb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xihqibtm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3petvhwgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zkykjpiq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3screnrex.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gtvljvdr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zlndesud.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aikrbikw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3piodxhxn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hvhzgkya.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3goorjerj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rzwuobgs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mtfjpgmf.html


<!-- 参考信息 -->