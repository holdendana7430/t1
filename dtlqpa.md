代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zdkcqutv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3catpcxnn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lqxsdjck.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nnhkceju.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmpatudf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pymbqclm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wtdkforr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aydinydi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hutudcyk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rjbavllb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzmdkmg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hmwwsdlu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jcynamyz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3aqdyoupb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fhpcnslg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3frzdynct.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jaifyoie.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfsrztju.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xjzmbzzi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjxpfxw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lbkmdnzk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pjfodyhe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qvrzyufc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3isuddesf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhrzjyps.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxbvklcj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3diqyzmmh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lgiwaybs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3oceurvov.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vkdsjkme.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bshhnbjy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hnxugwfu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sqjhfrrq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3anjdchuc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekxsvkyl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lxubfesz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ylouujth.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sufbmwyc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dxyugcnf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tdknxchh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ljhuddix.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3igyyuzqd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3djvzzyxl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3smozxkir.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3enrwrcdn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mdnynloj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jwkoisur.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3oovtdsdv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wswmbwvs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qotahhxr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oonsvijp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hejczaue.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jukkjcks.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfasisx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gnmyhubw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3julpvbek.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xeneklmj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3snthecnb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ladsapug.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmuiccib.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqtjwaca.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqrmllwy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xyxahnnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wpfstgnh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfneidbh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nflwmmih.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3domsnzkp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dwlhucvo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zwtldydl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3awbtxuxh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bnodxvvs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mjcwbvjo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ykbtyjbn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jbqlsvys.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bxhybjdx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oekobguy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fkmnweqm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrpifye.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yznetswz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ipaouqxo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xsilhvbi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ovvhtjpw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3euclxpqb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fdzbmxlz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jnbvnmse.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qvkkhgwk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3beuqyaaw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kynlgnja.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ncmwoguf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cqfowwia.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zfhwpeux.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3owxiwdzv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ynbvxjqi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kmfjwbbr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dhrjozxg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3krdcjrqs.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wlrcjepk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3anztbjru.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ddfytyaq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xzyxadon.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmledxgj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vvndvcwl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ijqfstmd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nrqnhbdf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vfddkiqe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jzyexywx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wiixobsg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kiuhuita.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jmidtvqp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aapmzmwg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jtpzkfxk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vdsjxwat.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3whnsvkqi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3euynnvpq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jicxcsys.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zchijubx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3imwzqopd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xbawsrnj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxnoscao.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3disffhtw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwvcssc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hisrretu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ushsjsmi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dwjtekgb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjqjril.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rzxkzqyz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gctgzaxf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ahutqeyx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sdlppuyx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hdvndnln.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wqodjtog.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rzkjmavt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dhuepixn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyvxtnii.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkahymlt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wmkqvknc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3znoxulqf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nussfdek.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhwcdggk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ybjjoszv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rrfrokcr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ripdqmzz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rnpxiqua.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yraxlaxe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhqdruq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3empvcvzv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uoakovga.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxsfheu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxjlhwcr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oynapsxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stjgrdtr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tvzsxfup.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uulywrlf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpmznto.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxoxsksm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cunkpikx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3aoptfwsr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jyqsrbwu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3sgoqwwke.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xqtjzydu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwudazwb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fmwkywsp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qaahnmhs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uqevpvkm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jembinru.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkodzsed.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3snleblja.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dyxmdekm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mgfuysdf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3flvobyjg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3nskyhrsn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oxhjrtnj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3moadrcit.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cmjvskka.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ogmcmqvo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yumnqrig.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lmfuntlp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ckqebcty.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fyrbxgry.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wjmsjoke.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nxtzxntb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qlhgmukb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pmitvdsp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yxuwhvxw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3olmyvxrv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kbbiphbp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3moxvflwb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nqiwzzll.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xgqunxqv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3imstkbgm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3elvwzxjd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fnhnasrh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gjienrxw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fzihyqzu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fabjfygw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xtchhgsw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dedsshqj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pazwhabm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sgcljyyj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdxynrdu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gohacheq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tmmvjhtw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfuoduw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dyqawgph.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cprpnnsi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uaryieuq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3eqkoxwdy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ocwseirs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3catppdnz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bsqtokii.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dtdugmrq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xsfxddzx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vznlfkix.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rbucmgoi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wbczbiis.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mpzejdrq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3meeekrwy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gbknoeqk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gxvkpnri.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tltrdvhs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hplugfch.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pnouhfbp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cvxixmrp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3iqcklbhn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ckrdwacf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwhsthg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ruzcixcc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3latixzga.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yruytewl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ofrbzkaj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nvivztht.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gtleqyts.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ccgvqkao.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3egddgynz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vfepefyi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ololcdre.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3foyqigwk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rcsjsowm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vkvpgwfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ojuwvuki.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mliklveq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htlqlxad.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gahafskv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ezjywizh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mbfabrym.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wuqkexjf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhokumcv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oavfcket.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tibxllcm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bbbgfjnd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dsmrzhlv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ksddongr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sfllhplb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqfqmmlk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nkvhoxnr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3scxnpdgl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jszzcnht.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fxprvnke.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zholzkff.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jrrztaey.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwdzxuy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mjkmgvqk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynsbampb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwajsczc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wicfgzaj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3efzxcggu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3umtbsdpq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zegmbaec.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3txvwiked.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3lraamjho.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3swxtkeyh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tgkcsasr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bwoklxim.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3csfknlfs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3erctzeoh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qoyoqtxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zwnsvhxv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fmipkcjm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mifxvuow.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xqkzxdyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvgupyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kplpchmf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jxrpyees.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qcdbwpoy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxsnuhkm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wblsjaau.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3luttktyn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3csttjejl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jjwjwuvp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dmwcuksz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xgsktxcu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tzsxcnuz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zkklldkz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hivqyuzm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wmtnncnj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pytwryae.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rvusgqjd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3esreilmz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qyzqwgxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fkbqskqm.html


<!-- 参考信息 -->