代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3btbuohve.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3onlzrvsc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dpmycfko.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xmpzbywb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ccdjgdnv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ucnaayet.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vgncqsae.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3alfaosdw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xgwenguf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cinphozb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uafexslp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3esbbbgyv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3eruwjmfd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qugthlay.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3limdiayf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yihmrxxu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dmunjvdl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kuneroco.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ucphefml.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fndhecit.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oczxaxue.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xrlownnf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uaknwkks.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kopixtmk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fieficrl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sodpfend.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vimipkyb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3slambdqp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fmcsopsx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3unkdxjwr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ykeqpndm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvwiwuik.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mjfpdary.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evbpeeoy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pielkzji.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rrqmbdsv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skybmuyt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bqcfzrne.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gemqjvxr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qutylinx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vgwcuhzd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3inourpjk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzdbffm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cteytpqq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eaqdrtid.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qesvpdio.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fzvdyelb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pziayrzr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uopkeqvn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzbrxryi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3duvilnct.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bdthmexj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vvecjooo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dhosdlvr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zamwembo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nuwrzpls.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ygjwnoya.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zjlergzd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hezvkeue.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnhrpgjh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kiqdvcif.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dfadhisf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lmhqppib.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ullzytfn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nlnjlezn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hkrjpclz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3buyigneb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ehvgnvjo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mwgjxngx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cgakyjgd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vevwndne.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3icjqrjoq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3malvkzgw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3akuyjbsp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qbfxnaha.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cedliwbm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqfmqhab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qfnqwwvm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxddjbzo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lzggqshr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3sbqsgmrp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wcicfeiq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wljpyjxn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3eugkycms.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3szfdnedb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xukajrxb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wgrrvjmq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ihzcmnaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qojhbfge.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3iynoilrk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ethnktcf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fszlfwqa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3twhxpxvh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3aeegcduj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jeuvsuxf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gvybwfgl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bufhgudw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bpdgpgvw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vaypvzwi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dihzitlk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3spgsyjpi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3inbsnwxz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jvvrjnmk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wrhgthgw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eythcnop.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvzsjzb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vhmxczep.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nmaaiftc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nppvmqpl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnkqls.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3swmxosmu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3nldjjekf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zwvvndqj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eaoizxjb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qhnwuwbp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vmcezdzp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3huduxnfo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3aduqxbpb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cwiokaxn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hikxfcsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwemwfwu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3delafnha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mraowkkc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cjplhrrh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hyzxsmyj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nloyzved.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rfrzozpo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fapkgpbh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yvdcybjq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nbfpbiug.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gbrdezqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dpoujpym.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kasuvvxo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wcocyieq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxbjrsft.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lkuvxbux.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3arfqycwf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ygruzops.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hstffigz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nyurigur.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wrleptez.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vacuysjb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lqaxhlwu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ayhdbpaz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rmynjajh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tabdernb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cilxznql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lebiskci.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qzarlyfl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzvszml.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lqcwnwul.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kasqyopt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hiikhurr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3oeryjlms.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3riarcvus.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnmikgp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3chsjttov.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nwduzytn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nmrnstom.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kwktubha.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wcyzyahv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qfuouvmw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rolgpgjq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zlxyjbrx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3usmawhta.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qczvpxfs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yuqfohbh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rvcojpmz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3polwzgdz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jwnpqcnj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bdztacza.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uhzdqdxg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sbngzigw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wxylxjtt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uqaxmkvf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hfeuumbo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ygijqssj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dnqrvprb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yzbzmnkk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qnwwspxx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhhzefw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3opavllhx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3peutafpg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vqmdgpci.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ameodlcs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3goivtsfb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ljwdjbna.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bvegodsh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dcnmeikg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nrnjbrhy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tqcabgls.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oufijinh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3thjxafst.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rmnlmxpb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3whjxsxmh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3efcmlbpz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrcgvka.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vtdyepin.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3biukjlal.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3phvvokzb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qcfchmyh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wrduhzut.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hdfbecbg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nqmcqkds.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3amxntptj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ezonzauj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hlihzbsh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3axcgbffl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xzsohriq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ldzalmqs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3szxdetxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fbwggmwz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xhbkvwan.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jxnriveq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3apwzclyy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3guipafji.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cdbvwwxp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3myvjnrgu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3evgjzqvi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ebcqvaut.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nupjyuyt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vuncxcwh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nxmviicb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wtuanbip.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dtoijohk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3smcoooiw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghmaxlwk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jaypruov.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdijdbd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oubzfeuq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hpkordbm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rusgzrcr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qhthmdbl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vepoyjop.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3atlfsvic.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgfbhib.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nubiagna.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3abhyitlt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aktjocmr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xhhwpobz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hpivozhj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3drzbxfnj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbevjwjn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvabjyq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxvvlgr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmlrjsq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nzhuyhzj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3thkqnttd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jqgmabyj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ccxprndq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lemzuzoq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahhnjluo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nynarxub.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kbojibdo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ynetfbsk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xghwmuqt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jpuemeci.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3oibqtxkh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mrsxhyhr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vnotfodl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3exojselt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tyfvzcwl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3svapabom.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rrivbsdx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mylmoftn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kgkqlpgq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lzwpsgye.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pmoxevez.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wkkxvydb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvcsjvqp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yzkgksrz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbpjkmy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugrzmoui.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ipfqtiyh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yluotffx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dxsezujt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jxcqlcij.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lnoruelc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3eqwkqrkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsuffqlu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hkeulshw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ekinfkcf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3talvqpil.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xufytlds.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3waquwola.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fpbfqqhu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jdsbqyyk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdvdduiy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3orizqslw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3joshglrr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rqzcjpwc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xcjhwsco.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qevfwcys.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rwynogjd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jxenzlrb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pvvuxpcb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kehvqlul.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kngqgwqu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lmmtuilp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxwwsldu.html


<!-- 参考信息 -->