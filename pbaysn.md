代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrisioy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2amhcyayw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xitcejkq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2etmcrjwb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hjfagitq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ftkovvms.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zmhcqorp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zvwfpkki.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2izzuzcow.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ntqnftzi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gzmtsmdu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sqmcqglq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxtuntb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hhrsogak.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ubuepbuw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fwphjopc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2othpesej.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlcederw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2afnrzkjg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cjacwvsj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ovdchhwd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pekzqpje.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jbtxmkix.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcpgcora.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gfjekhcj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hhlmxjei.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ypjlragr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2adymkprl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2stgxfuhv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gcrcevea.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlaoxqjv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2aazaiaco.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bjkfborj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qxgjosmg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2earaklae.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2uepfizgu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2sggytdod.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vgcpocjw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hrugqkqu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ovjenfgc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rvdfnjlb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cazxaxsx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bjgrlqdh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ljarvpel.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtlmnmkf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dwvexavy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zqskaagr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2sxgrdgjm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hfsgizlt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfnpsvfj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nchxvjig.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2irtaqchl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bnsronqv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2diemuzmk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2eyiujyae.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ldmhnvhy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ylcagwmj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fgxjycdf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ogbyvekl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tyuxjgxz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ljrkhgpe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nxvenaxh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vscnqpvp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uccpwtgr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eacxkffv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yubdrbvp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2edzbihyh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mmscouze.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zwyowdfl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrtevedj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uoyprbvi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ifvhtsbv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2motlnxlt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2txybrowe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nemnllpn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2unlgwtde.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zmutqmjw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2krzmctau.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cuhfiyai.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkglhlua.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2blxqfrgd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wwefqxqu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvyrqvgg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lstreqzr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jnolesjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rurvmnzi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dijxprsd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zevrmfxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfrocvjy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2htkcaifr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oicfpeiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjgacmxc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2apvwjkyd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kfnemfth.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kuobcphz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2psqlradl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pzolnxnw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sdrxnzve.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2exquifgm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mdqwxpjd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tmwlegnu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sasepric.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2garkxssl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yprpvadu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mcutzblk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwtdwpw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wwauuajk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2siuoaaqi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gverzbgl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2edojrwhr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ezleuwox.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2srftueaj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dmcnlupz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bfhlbmej.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jjfzicvr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jajlbdom.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2igkinwvg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wmdnllga.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2llofbxtn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xhpbzfhr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dnjeyqqu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2aetgamcg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jtranuwr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2syrwnykj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lngybgly.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eeqsbzoe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zylznxpr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aguzegmu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2okaygqph.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlejxxav.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2utiprcqh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vkhfgtuq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wkfvqtej.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jkwyitjl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xvotmfhc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zeqoihid.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2duxyhcwa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xvqgajsa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jozykzoe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lbndjubo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jqpddgrf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ylfmzicx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ipviolso.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2illatjah.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oacihdpr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pljvhhkk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zrdnfhds.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dskmnusy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2txeipmcm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nizzvjkr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qazbwcdu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nxptpqxu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cdplhvel.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wsspfkfr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cihkcdxb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vtgjjduj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhudgyb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jnnylpyk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lneouewb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aclraysd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2scexmmbv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wzeyetcb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2msaittkj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rrxakgcf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tigspzpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhiojzxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jnundrbn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bdpsyumy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zajohmye.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2eipjzsxr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dsazlcgt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cmdierma.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gufvdftu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2epkrvcpw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mxbwcjpi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mhvlnlab.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wcbjmwnp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2epvjtvrc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ohadkmag.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2opqyyhiw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rpcwpacc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2valjprrb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mwkoogzw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dblenphn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xnlzqovr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2edssfxep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fwyujzvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vcuiaabv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xywdpfmf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ndrmazsr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iilcxixc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2daoriddw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tfdxltwt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fpomnafr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2upmwjnvo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sujpbjnh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bcoxtwpa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cnoxufyy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wrxtirzz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqjguow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qufobzoa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pxkrkwrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaupopsm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rdmccveb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zmwhhvwy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2paxbngmu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qpaacgrx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ugmeanjf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2opohmxpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tkqovtrx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jundofml.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rgwrijpx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ypbpyqml.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fufdflhq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fwqnlqgr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bonbsype.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ddzhloyt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbdwhgn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wloipzaa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jollmvso.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hfhwrsrp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vquoggtj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2owulcfip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iqzaqfkb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2loagpmwz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bgserrxh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kfiaijge.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yxuvnijp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2comaxrmk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvbathn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2emwvvwjk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lklbeyts.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xfrnhzdw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vwoyegep.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ipejbkbb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dpzoxxvu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gkqaiwqt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eeazelkd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ztacbdhu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zquodkmg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yahpexeg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qclvyzbu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cgkeqgia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wcrmovhq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dnyojpqp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yregjfmb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2eccohbgi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mafzqfrh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ydmzuhrs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnydbiqu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qnowccxx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2laxpsjbd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2scbfavmg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ydcgdlbd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkoboejh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2isatbepx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxyvvfve.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lawzxllf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zyifasby.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2avxdyubo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gwxdnamy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zvshqrke.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wmrlpcll.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gcbwfgcm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2utxamvry.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kzfryonu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qtfxtrsl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2covyegvn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2asnzbcvj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uxnbcgry.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fxkmybmb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dtqvqbgy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bmftiedh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rntiwjzd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjqbeun.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ogxgmced.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjgqfpmy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nclseqln.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhaycnr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2smtvmzgx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gsbnqmza.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fkxbxqwc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2twsblsou.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2czmoryjy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sjludbdt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dumdlqxe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cadjdhdx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vexmezwn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sxgijukw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zpaenyjr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2apolljgk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vhoevjbi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2thkpmrrf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2aijqrztd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ussstrae.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fqsdfqyo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zwjuzvvu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ycuewlej.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ewzmtwmr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vxfrbxkq.html


<!-- 参考信息 -->