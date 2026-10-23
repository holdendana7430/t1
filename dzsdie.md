代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cefblzrv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3efqrlexj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3znerostj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wozrxjhw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3plbeurvg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3btnniddz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cowwtdco.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jxbxjaex.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ymrdcsjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3swsnqlua.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nuywqdbo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3svuluqai.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lirimjez.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lzwnggmo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvdjmjwv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3smhlyocr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ypfcucsg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3thpctiiw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kkgcmdic.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qyuwjjex.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ggadftlb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pgaaesdx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wqrltxoq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhebxhoi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbaclqjz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rqmofhun.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lvptszza.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jofuoedf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lqioesjy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sciypyyt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zeybujdf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dxfwzusb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqosyrzn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3psoxvmxv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fytxalbz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3swghneyh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3sgqbqfbj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zrbehsid.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ensmtxgh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gkeudzuk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lxwneugy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ufwbhqtq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfzpahl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3axowglwp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dimmvqjj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oujjgwhp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3andvrylb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lvgkeccx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ozcmduzz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3akkydojr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eytlcqyz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qcvqcvck.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vitixsay.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vaxayeml.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3eojcfwxd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3calkgoux.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbfxfdrn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xlbkzyco.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3moupfqjw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvaozvrd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ecyhkkim.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvoxkdf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aknvoipn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bljkenwt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xklxdsht.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cmqvirnl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3srsqhaxr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3izrzkmgd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3syitvuqw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3txcspbfx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fhrakhyv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3eydtelko.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmmddjz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3esfujkfk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bsmwztzn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ubhcgexc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fgkcmfqr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nsnqfkoh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ddvzfdue.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bcgzykkh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zhnnatal.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lyogzjum.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3eceuogqq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fuwbwatk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ntebkwga.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irvjrsuk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3znrwlchd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lfdxcfya.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jyahzfzp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3nabxgsfs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ldduceos.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3neekummk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3irrylelr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aratmluw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmizpylx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3esrtyisl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yjbrfjak.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ndrcjupn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xjykrxop.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3emgahlnf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cmqcovlh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ayfisaxo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xitaznkp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lrakodgg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qvflysrt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfltcumg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvsbwdcr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fnqqebbd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjlxrwz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mbgwwypc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eocqmyxj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3wqsczffq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmqebzo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yaggktmp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vlhsogwk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3odjevkcy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qzofouwl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3oydgfnhq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3orqfyaaa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fnmrnkpe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pkjdfsmq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjqzgkc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtrqvkw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iiglsife.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xkjqrhim.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hoecleet.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mdyovjvn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ssggioko.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3sanczyhv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mwamslfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ceijcsna.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kfdrwpfr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qjnugquh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxyqbgsm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lzeltalb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zajwsveu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3noyazsdw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kpmyszxv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qeehwcfk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pilfsixh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sebrxcqr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3naclsswk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kxwcurwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mpuncfpo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wrfclzsd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fdzcyupo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ciogdpmp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zdhwtizr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xwipshcf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyeakzyh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jnbqixgf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zwasjiox.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xrvdfaac.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yxbvtcbs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oeevkmed.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fkwqayqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nppzzyvt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3twiunncx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxffxdvo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dyeptodr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ovcmxtpu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eurmiymd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vyfscfha.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wvxqsvrd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhlcoaop.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eokftpdn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dmggdgdj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zirruahv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dwbjccrf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vdbzxlcc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3velpkslj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnatjhl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ooolmmkh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jmzkbene.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gkbaqsxq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qnyepemk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xjvbnqnk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hpbkstta.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jkkapfmm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wfyvvgjk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vjzyzkfj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ypmjsebq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgdbgbh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3picqmjtt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3acfulkje.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wiowqtea.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ntxefajq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ernrgqwy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3adifmnga.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3imqhaxmy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dqjryuwc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kycyadaa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hgdkabex.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zxpsdixx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ieahwjos.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nybpqced.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vzxrzdjw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3adyquemp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fmopbzxc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3khwplinc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vdmakukh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zmswxiew.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3oiyguwdq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xrcrxhcp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bbltzwae.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3anbomomf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3efyrwmui.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjeoyaul.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xfdmokkx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qnlqbusj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwyseljd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bjouqfyu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yvmgsxbc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3allwcjrm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lveeivik.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3biosdyjf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbirnqhh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kreztnjn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hkakjvnk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqrflqzh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ddwbjeef.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbwltvg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dvhgstoy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uanosukb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ndyefxca.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rjucenvt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ebtnjkcy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wesayslb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wobdeboh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3thdnbfyn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fnqpvgfz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kffxxiaf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mtsmlfiq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxshxqqz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yipsubfm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qgrxdruc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3monhqiwp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3urxvbvja.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3upioqsyy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dmjcoidf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3toopdrfu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dsujzxuc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3arvaqsjr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3viopwxgw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qyoqdvlv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wblxtgck.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3flcpshps.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbipftz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3stbsgamq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3toddbchx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gqdxwfst.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sgiuhdsm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igittunw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rvnmnbwk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zxvfgnhd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3brtedeco.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sydgywrp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oscthaup.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gpsntuyw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrqgoxb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xcfkhltk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ulbwntep.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3htipvekt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tolnsuyj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3keutxknv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wovghsxv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pqqqqler.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3avyfwcqs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3eayznmqv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3abprzuro.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3keugghpr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3txcowxbl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3loqvkcbg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3simultxw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wuoxvzla.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ditipbnn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mxqbkurm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dovyfiar.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yuepvjig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3sxkzqmiu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kecsssfo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3totwioyo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ofknygro.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3thueqnug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kxfludzg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lptkapju.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qqbpzwkm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwnxdxkm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpkfjqps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wyazkrqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ioioxthx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3immdrttw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfiqdqha.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xxvmdeht.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rjecbvpj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mpiakopk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3sgehlpsu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3flpgabgv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kxhszokb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iaglihaq.html


<!-- 参考信息 -->