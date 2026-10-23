代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xacysond.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gnrojrod.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ltdjnuym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tyitetdi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtavndnh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjwsvvy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ipkayarz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xedtrmtd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpybtzka.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pfczvxpe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xmxtdfec.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yomwexev.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xnzhqasa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3koornqnd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfjqkap.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gqhexeop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ocfkepkn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvpkaqzd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ngezoafj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bzhxkkdm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3aclwpxbh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zscgufxy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aanqfxtd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pgeyohrq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jiomyooq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hlaysofs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tyfjcgue.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bgwxdvnb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3aivzoyxw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gwghswaf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsrwogru.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3npmmnkap.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hagesjlp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lwdhhxwh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ryxqokqu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vgziznxk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3quaehcdg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vvsbzymv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqaccvx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jefidwqv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtzidkgr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yavyltxz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fakktxja.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3sbzdfkwr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ofwqdocm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lnrbynwe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3izsghjyc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yzwsicus.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hughdcxi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbuwnel.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kahrlfcm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qdhmxmbo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wicjdtwq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3eaexgnje.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ptddpxvr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bttcxvjr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3eawvvjgk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3igdferja.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3iiqkpscw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ivqmzfjd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxcuqylh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gflxwgap.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3juunqoia.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3msmevsns.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dealllfi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwihfuyn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xycovpjd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3erjkijyf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zghdjgvi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rwcywwjv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wxrkexpp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jiimelwr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pookbxtb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jqeollei.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3apxzvrec.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibktvtmt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ykzazbbr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yhsbsssh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ozaeklkk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3chehfezu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rxcrfaxy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ymfdxjdi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vlirvqvv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aqyxnyql.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ykexgspj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkppbsex.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpsxjmv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yxsarema.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfactnxw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqcpysu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yeykgrdb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gysaobao.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bninrxsf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dkmlznwd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdzlwdu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ovjdoyhg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pxyajtmv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fzeotoac.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3njvanulr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pwjtxkxf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fgrlzvqz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cpbqdoob.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kotdsxkp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbimliaz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nsmhsukq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3brxmsgjv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzxpgjsc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3eqenxsbt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nyhpvcjk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hhxuzvfq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gwqmecma.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3iexpuljn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwtnsehn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vcsfwgzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nrznohcq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpiozwn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qruuesmo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gojxrrps.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xqricegn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vnxbbjsm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ogqlacki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ywklyyfc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jhhfxpyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwuibkj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tizalsac.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wxfglghc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrawlux.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lqkhmkgp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cnnansdc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qcfpatwo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yeudnjeq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ldzlomrg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3udybcyww.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mgsqwyaf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tifrngmg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3spnkhikd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acpkgfsz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfoevhja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovclnbje.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpitae.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nzqqimbn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cmezxgcj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xcttxpch.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rabocqjm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cphohofe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lmnflrkw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tytewjjs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3moviqhts.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3avxjlkmw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ffkkjlsr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzhogpcc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rcnwpjjd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mivqaqhp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yipvyvke.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3dfbrogoy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lbyeiygq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qjgohptk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bsdwmgdi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zzhbidec.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bmzaoyxm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkztpamx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3adejtvly.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dllkzbgh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kujtxazr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wefbtsvp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxsireyy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3duatxasv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wugcolfr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ojvfcgib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3yppauzqr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wbarkjgu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3czfihwsm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gmfkucww.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xqpripyd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3apqdwowu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zuplfjvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fwbzbebk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ufmmpiku.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ynawtmpn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lcxdztzs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gwwjxsod.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cmrsqqrg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ewqmrdyw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cieokrap.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ynksdgxl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvfagchc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fpkhkzjb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3typtwefo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ufxladsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yvsjbrsg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3edjqxxbv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tkkcxuex.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kcdnbbdl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qmejtegk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wtjommcz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdljdxka.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggeknjhr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hsqiauyf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ajoighhi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3togecwzb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3iuejgwqq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3udnaixwn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kafuoivn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvjefzw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vdgqknuw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jvthrltj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lgefihmc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yktdvrur.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iefhlcuv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3glvnluqz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ysobyvku.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ulezfndc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3sjitkmzv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fdazdtwn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fkzloosn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uxdgjjlv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vlnahjei.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jtpulcbs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iekoayjh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3khdtioob.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vhulkzdz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ajbotcbv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ppjadxsn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cnoghsba.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oucgxqbl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fdtfqqib.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mbelpjge.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xdbstxxb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pbyafdcm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gmuclbhm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ijxpvobw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zyvwjdiz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3layfkldf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ofyigslw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zjopvoap.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3daaqznjt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3stporagg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vzmkgmgh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bagpgyod.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pfablzuk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ufmlkmnf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vletvrcn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3smjecpsu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wxgfauju.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qsxjasxt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dsgmfqsj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uislmzvh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zrfdnclr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fruniuxe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjvdrgfn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qgatkkos.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hemfkbsb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gewhnoob.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vtaufjib.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fcsqsqya.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nulnbnst.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wrpzqtyj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nzlfifyw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tkvutfdh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oaamtqtc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvnjwck.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mcesuwaw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3trdlcuse.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3odkygpjp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dqjiwbdd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wfvauwjk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thtqnhso.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jjnbqsgn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pnjxpubs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xwarauhf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kwcunqvl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pjxdumsn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jpstslop.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vyqvhmob.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qotnxjsz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tatjuuvp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gprrjyyt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bugspmim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oankcree.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vtfwaneb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vibqyczz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rfqkmpep.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3chvtvsvr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3reeyerpx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3eauvooaf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhftkoez.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fesdqbsl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xtcduixx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xqxwoivy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ffeejaip.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tovppawx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3btoatums.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mytpoyyb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gnteqpzu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kkoqumqu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cveecqcw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ykukcwzn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fpvsdoxk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtixhms.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvuzrbic.html


<!-- 参考信息 -->