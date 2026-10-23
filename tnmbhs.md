代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvomlsau.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qoswibnj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tvulrjyd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sanscprh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nptuzgku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xghzknkf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dnodmsbx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vfaesdje.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fimwqbce.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qdjecrwq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zwdnsjil.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uzyigjma.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ltiweblr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kbzdsevd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jpnebpbr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zogfxlem.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rhssrbzp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vsvjnxwn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iavxumvz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mizyxkim.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uadxuyrm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tetdpsyd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3swidtyjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3doudyvqi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kstnzkxh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdilrwf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3iboastaf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwhxybkj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eymrynma.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iwmyaycn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rmofoymz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3orzbhuyq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mzlcxkpk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfjdfzva.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aeankcbw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mutjyuqj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3pzhvluwc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pqcphtvl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwhfykkq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bxskiagl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ysnlsuqy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pnxkvaec.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmoafbk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wboghqqc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwcmpohh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zriglsex.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uprdxybn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpxhnned.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rhwdczgv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hksbcpgm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oteuzsdj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pjzrwqkw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ranwalmz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rxbyezyf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3daaatfoc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jqffobnt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjapahfs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tofyyhkq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zrrynewg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyvxxbwd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dqimqhwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrqvneq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jfnfwdcx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ilpxfwrm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lnedqecw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3bkpzreyy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wdyuuueh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bbveubti.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jidgluek.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fbuypyub.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wtkudyyy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bhyidgvn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3quafdiqc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3komhoowb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rnoophbh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xeippbpi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zbvxbqeg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tfjwqmam.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yhpamauy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vpsjlmcc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjnbbhfy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vmbwdeat.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kvzkfxlu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gthzmhyb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xqvwuwby.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gofydnqs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3shegzenq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bkzohadb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3riidwlpy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ppotcwyj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ovfoxasm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3covtuaxh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bdirjixy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bakbxpvo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gyzgtwsk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3corbkgxb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dhpxxydj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qoysccnb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tzmfpynq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ixgrffos.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qrxonjjs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jxpztdwt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nqucqmhj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3buelimfp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pshqjmdz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mokoifyk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qrqwztso.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwsvebik.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3njwopaew.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmaivmvv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vigsbauj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ruzumbbd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwebhbnl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qlclmfjr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3omffasjm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ohstdpdy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ahlrypsf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jhexpbhc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3oyyjrkou.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vksbfcel.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yfofsuqp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jqtcqhyc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ssgtveze.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkotgbix.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3icxradvi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gpojalrh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfwmlgyv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rlelehyi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3srillinz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lzzkxjvz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jiizhwsm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3boximosg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3htgllvxv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jtymjfev.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ufssxahe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3atjrjshx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dwhwdkvy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3apmkoiyw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nsccrevi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fxknqbjv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tolwghwv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlbpxhbj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ugislrbo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hpypddth.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dxbromxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xwmtitnp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fgmkmsix.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3llotadbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xwvzznvz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3btrwfkzq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hwybpggv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fsstmruy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uaqjrmno.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wnlpnigp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3whcdsttl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bhpbciih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zngyjonp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jxcpugxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smwdsmgv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jcmwhofc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3otgzrvvl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3asosheah.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ifwofman.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dhhdmusa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqlveopa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dtkclodh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3urkprhqy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvwsnkta.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yqbdbfki.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3acuebvtf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ndrvaebb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tuqinphy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ambqqtml.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjfdatx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ktiwvfat.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tbiwvypz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xlkqhslg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bvdlyytv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yifhztgj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kgdwghjx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3shmkbdhy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3suuudgdh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jfmxhbaa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3paixjplf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xaiffbbi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3viytagny.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mdnfdjtc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rawvcnum.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3edkudwid.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ssxdeqqu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3npqkwudg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tmgtmyxt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iwfoscvr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lklzsycp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3azwkbztd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3okxmdofs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lvjbjaln.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yxbmofjb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tkharsrb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3huycqltt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tedqzkpb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3adciyblw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pradnjdt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vidoqldk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3aeplwufv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vawvtisq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vpqfyhfa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lnorylii.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwfudztd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mvxakqiz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxjbqcu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hrhfavaa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zwnblvkk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nsfrlmmj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dbbtmoyc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uuqnyuff.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kltayguf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yukakfxz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tqcmupqb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xppaclge.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3embbmodu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pinsbqiv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ovrsdfsd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbvwaoo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mutkwcyz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3llvzpvqn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bhietwnh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtnkbew.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3uuptxzcd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yycxhpkp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ttdanxph.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cnohszqa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddvbpguv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3urobrdqu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3swyeumop.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ebutdgyq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wbujswrb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ftdzbcdh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3onfkgkxm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nywxcqld.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vodnovgz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zmdpwqdg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jotlmzwc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bpexlvvh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3haikamsr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jqiskcxr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pvmqfvvr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zqcianyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rdzxjrxx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hsxdnlwo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eegfzuzn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zkzhnsjz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxfcalwf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bloqvlak.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3oxvzvwic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3offsijjt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gfxoxmtf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sjktbkxy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rlwmiclz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3abrnfrzj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3suvrkbxx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3awmampri.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ffqtpjbf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3osjurpzz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wjfhkojq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kuhjkyzt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zusoyxrb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cgeuxkjq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3epzuimlm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlygyfue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekntfgqa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bekqbzkr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wptfzvji.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xuxtgarb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hpbrwerq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oswkqpnm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nvtyagdh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3syndbxus.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gikgjfgb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3smnvruoy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zvhwvnar.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mlavyfdo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3snibcpla.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3alrjlnrl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfbliix.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nvbbtblx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yehhzuia.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3avfmeqbe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tecylnov.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3arsoyqka.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3elimlcaj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tscsadvc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfiffjph.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rlekedoc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mbrlpuzp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vthdcazp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mscgdviq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zlkyqkyf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lqjizsgt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtmqbss.html


<!-- 参考信息 -->