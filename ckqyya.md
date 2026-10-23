代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3unvqknst.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jzdhynlk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aerqmsbn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jvogtwhk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyhhnpqm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmkpxogo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yeqlguua.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vuezcbri.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3pszqsxpp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtsgpywd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gzosfgxg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fqdsrxix.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zprzzbsv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3onaenloa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rkkizzcf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ioajjdan.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xxhlvgee.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3biguytik.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kcujkhtw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cnbtspnd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hfiroqfe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3izusnecc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3awcgcxpj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ryavtomy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ambmymrb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wyytneva.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dzljycbl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yejskmfa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3facpkgim.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qwwnpnae.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3edcshcrj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cwstoujr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djfrzxcl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3sjifrotm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qclnjksq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3swfmwsoo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3njfvdapm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fdblqexc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kviaukgb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jlnwzfen.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vcnfxkwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wbbwhuhd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ktfafiyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iighucww.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bawtwsmn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rqyoeryf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mdzenepq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3chohsvkz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bifdyytk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yhopshat.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3blxhujuw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3awkouabm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3awnhpota.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3radwaztt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nsyysdzr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ohvcjmsa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lzpfvhbe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fkcemkhn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3chthzndh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hlzhlapf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3srpqgabu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnahytya.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kgcyjbgw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqqalbbw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfoqlesp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kyunkoui.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vcpiygbp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cxpcloic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gckzcwkw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jllyebdm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxtujsyn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rgqnodfv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yxmqqwmi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hnuunnwl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlchnujv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cuvosjag.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tyvqhruv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3luisklxh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3odygkuko.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yupbzwiz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcwwbayz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vzcgjnhb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wynfujmt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wljtzmxt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zcujibgy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mmoovuzt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlmukmxs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jbojrvkt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ottdefgk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ebkrhqzh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yaticast.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3elzvbbgc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jmpcypao.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3olpeuuis.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myfgouuh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hevgehbb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3orgznvrh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwfpacs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3sedpdcyw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vatoghqm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vlrnxeww.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fuhmysdi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zcetfbdw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhblebei.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfrgqen.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkrcvgd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sndyvirr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nztwqlwr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbszpchx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3izwkxool.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ihpajxnm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pfrffmaq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wtunnptu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jvkydabv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ntbatmrm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jecqfjum.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqwitmze.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwpybten.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hfwyawkp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtiobxsr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ycqpovkz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbcwviw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tbgudgpi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tymloiiz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3goaadbgb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3llkbpsro.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jhcflweu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fhrmvkwg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3akskycul.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wastspom.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3euvxhfff.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3niyodmac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3upsmwyht.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ifkkbrvi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cetmptmk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rmzutwxl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yvshxtxe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hgwtkedp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dibuihso.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cxgjtloq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pgkrcjrp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qimpntep.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdripqbu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnzburs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjztayfo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lddbsptm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jvovinyk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hdflrzlz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilecyqei.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3aqfrgrza.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vurnewue.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zayxuyvc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rvzljhtq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wuqptomo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zknurqzu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lyeckkfn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qeijyinq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bdfnfvsl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cksaxphw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djvtolhz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dgfqknff.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bpceargz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nvydvhjw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ejvyphdq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdsdasd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmbfgy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gjjhgwkx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vhxkkvob.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzceqmrz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nsrstuip.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mqjfkrep.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rabwrmii.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jyiubarv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ajvxnmgc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fyxkwkpb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3madbbrpw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3arryowyu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zlrfezov.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sznkrbdi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eogrvjyf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ovuzikbr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tealjfnt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jsitjwzh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zcdfcjpv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oswuhtty.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cdlawnho.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lizqyowr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3owyfrwzc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bwoaayym.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dmzubama.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3acjdvgiq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uxmlizps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzgoropg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qiltbatg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqswkdad.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3unebeewm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hlnychyj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tvpmryal.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vosgfmpe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hsslrckr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3devbwmsj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yghdrwoy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ccykfloo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ocgqberq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jyxqtxgc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3spfpkhpv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3klyonwfg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3masopclr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bpvwyixf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsaoixy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qxictvpe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ievmccfm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kzmlknpb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3muprhgio.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pxdjpbrq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qpngmvuu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkzirur.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cdabuzsj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oearldru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kzpmtatn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wssfqdlv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbhdxnn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fwrapcfs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3psrozlio.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oagxfxlx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ketztnln.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jodslvst.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aqxxencg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3idbcwvvo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hwfnsvrr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wyjivkpd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3uvtkymgi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pbgzqdyi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lgmoigem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oikmbtlz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ydapvydh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ugcuhkgk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3iqjbvctl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fmwbaika.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gwemehyo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fiezbzgr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gblaipbh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lviabaje.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dtjiuaao.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fymbudto.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3plpmpopn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3slaxersi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mwolrymp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hhqhwtzm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cldkxdrd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zwrrlddb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3idwjyceh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfowxdw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cbqalxwj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fvanicua.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhpjknpr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lqgucyfa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sauxgrhh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jpqjtrxs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qrguczxi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jhvhwaia.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xszsdduj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bkkiqfsa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3blmgevtb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ayyyqcqb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pghcnwdn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkwjbmj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ersadlcn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3oiqqrlhi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lgqcimwn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpncmqp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bczpwzdo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3heyadjzm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3eybhednm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jmkfbpul.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jqxgwsoe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hniztmok.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bomtpgxm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hqfjqdkk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wrdzqwdo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pqmalyye.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3poquikpu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3atbfiouv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rrqienak.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tziqpkbk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jpkbkeyw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bjyuxbxy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kxakmezn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tulveoxy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tdobstlp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yynsscej.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bgewwqoc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vpletvyg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mtxvlulo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ujntmqra.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kpjpigqc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xbqrcxnd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3unfcjpdo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3buwezvxv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wqmphjjp.html


<!-- 参考信息 -->