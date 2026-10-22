代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sbuvvfff.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2goblrksi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2glcgamgm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oukmkttp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2keuclxlr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nvjxmice.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xkbewlcd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nrebgdrb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mwncfuas.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qkwfcigt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwmlouye.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nbjonuqb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uxhdrcvb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2llmdfknj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xbilfchp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iiytpuxg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zxwnsaqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aetkfyzs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mnbussjt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdewhbm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sjlprtpw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vhhvimnq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sbxqwdkr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rcdntule.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2weikdzjc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqsybuz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2epkbvczh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zgkupjbv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kyvherag.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2oulksvjr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ynqfrsdp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jnosulnb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2htrsdonz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ejykuxxr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wojbbgoa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jsjpcspa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wsenyids.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ukzsngea.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbslfydw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kifhtmnl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2awxnzjov.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mdjymfry.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kedczhbe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2orbkbbdg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2asqrodme.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dyslqino.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ackffywf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bdcvoquv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fixkffjq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xkwehdeh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hupflhyy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ektgrbvl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2znuivqrz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2toibraku.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hvhffgfg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gekypjbk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jhterzdf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uuazoetl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2htuwsepf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxkxerr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrtphjlj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2goxfjjgw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyukhdfr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ysksogst.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnvdaqnd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkhpmx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fmdnrwkb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qwshkage.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yjpbzbvy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hmgnycgq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2eqsvssgh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wypaunib.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mormesve.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2glakltlh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yruzoarz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aunoimtp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lncfipww.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gifbluhp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzohut.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kwnnktkk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fcpmpqww.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2chywojbr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bvfdyijh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2feydzywl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ysrpgtbe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sneeletr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2krtijilt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zatwraqn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wcsdwfbw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cnrcmwon.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ayavbbzz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xahbbgce.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hfwkmldj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2roflfcak.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zrgevkbx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iaixjdsy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wntiowlc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2asvukdot.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2meuzubfc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wjjopnof.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kiolebup.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzzdkxvh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qejyykbd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2heekqeic.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wyttxtkg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kkipixeq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvyppwt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2twltscai.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fhjvimpu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gnnbpgkb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hjfhutuf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dkafyjgh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qoklihar.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrzwbib.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptdxqdhc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2maghhtyu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wqbrmpvg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2egkrujjy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2avbthxsz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xjfanpss.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybtzxaqs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2akruabyi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yqhepmes.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kirhthdx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2toehhkbh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uodfmstj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qyzgdkhh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fuzvxqzo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wbuzasgl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rfkiaubr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ozplffuo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ztadtulp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cweggmys.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wsxhgbxj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2htgedqjj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nayhfsyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vevuzvfa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsxuikxl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xfcxvvqc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sfnfbrod.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2srtpaofn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mogulvcy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nojshzlr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eylayxoi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lobdmxfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cyrgmtpq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcoopii.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2spbjxdch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udcnyqiq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xifpvihn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvlvpheo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sehccnxu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bgokoele.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ubjdezxy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ipjhqlxa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kjmcbprv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2eoyxujke.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kbyetxhe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mvfhxteq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sooligev.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zpujmsoh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vpkyebsf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eqgequul.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lilgnvqb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jeaqwrgs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbymqbc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fptzvhvp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hwdruzfd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xtgfhlmn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yjgqxyjw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ahjtqkxd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nbpfuetd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2liqdvsiq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hmqqhdux.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdvbarl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pfxcskzy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xsfezdfp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tofjiglb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2voweqbug.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xbcbjxji.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zmerfzqp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cbibbcdk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sfimzsaa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jsaphyug.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ctsocudz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zvhpeztt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qncwqbgp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pwgyguyx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vvwvanjx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fvqsuwwm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2chyyaixv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cdqlztdn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2trcirbkt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2laelgorx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zjnufnve.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mgydorcc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kcjwkegx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qyaptxty.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jaxslglq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zddzwrer.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kclgftei.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mmawzcdo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxfdkkk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dyowbyxx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pjvzdiqe.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cohmkzxk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2keoybsos.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pajrommk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2krxfbdbj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bsetrdeq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jfgazvsz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hjcekxdx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dhdwbvny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhpbclp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tidrqdnq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2usllbang.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dxdqlyir.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jnfofmae.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2veujvnjd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gqxwyhbb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2syvgvwys.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rfrxmevc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mtqfaddo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vgmgmozc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kzpezfnk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uxwnafhd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2esdpkpmz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aapoaiwk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2herydlbf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dtwsmdoo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uhaxljzx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yfkicydg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pxcsztng.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jmwcuypl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2flvretqz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ywdcbbzf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2phxsewuh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ieqgbwzh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2emxsddpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2crhotuaz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mhbzzfhx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bcqdilsr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vvpaswht.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2locbwthy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dqsunthm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tsplffii.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jbterjuy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bnddlptd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qktcehjf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cigczhwd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jeszluvs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hakhnnhb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fsxalhzy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymjovsyn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gfbpheof.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2olusqirc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2srkpefip.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rhaiamqj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tsmkwoxp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nngoabpm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fepugbsl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ifvvcbad.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2avlrdghb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqxxpor.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2larqhjcx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hrvumett.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2miqkrxrt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfpomkse.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2sngifmny.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2esbverka.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oscfxamu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nnbqxjhm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ntxvolql.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2inpmotqs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kmsqgdpg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2pqvvkifo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xdtfxqef.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2idpnuctf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjooopge.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wgqfaimz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hnapdsmx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nxbfdxgv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nngbnnxp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqqzjesr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fdlzntis.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kkfhocnr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wbvwkimn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwnadkmn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xllcuzbk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zuupvftd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2elfxbocu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kedrqbml.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wxxndcpy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xfatlxwq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mquyjumg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ggdnozqi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qxvxiqvv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nrtgpava.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgekftbc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qvwdxezx.html


<!-- 参考信息 -->