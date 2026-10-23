代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unjohqur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3krzovwoo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yjpnhsid.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rpmiahkp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3svawgetq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rjhjcnse.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pbmksjql.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekqfxwfx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhexttja.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnrdthw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yuudjlpl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cuzufevt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukhwvmhc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ydjrbgex.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3paekrcma.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3arzkmzit.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sbmcfyxt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3puogtkmw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kgqsdpuf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dtdlfdqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rgydbcmd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3atrqksue.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3esdlaebl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mlsyjjnb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3avxlxedc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ludjnktb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ejrqudje.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qgxsmojc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lllzndtq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qsjrakxz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mjybylwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sduelgim.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kcrirjsj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ejstkbcx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znhtrqfx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3arrjhkoy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3twhsbunb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wfkmahya.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jkzskrml.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3awannqux.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gleokduu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ubqkoziu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ctjjtflj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lirylcmz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ogwnttgq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdljiml.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qgwazenb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wwdbtgbi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhknmzny.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpbadgf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fjpkksze.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dlkngehn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3trojiywf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tafwwqom.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obvzxqar.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jrjkkgty.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3imqmyvci.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ejsorlmq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hzafzivu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rvaywotr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ymipgpzj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3muvaykip.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3asbpntqs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dicnwucp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gkeqrwse.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tnbtfcue.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jyeqqroy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pdgbtbrg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3oqefgopl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dumisxar.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qhudxttg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cbbmngmv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3upevctxp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aepdohbo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kcjptevq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kseyjexu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ydtupfqg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rxxigomg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cewaaqqh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3inskwcjo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cquhhpgp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hedxwjzk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zyccajiv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3puabgual.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zopsuaqf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwddzxbb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ueowfryp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wojnycwz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wgkghgod.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qncnisxv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3foegutzb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3neadqaxj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yxmcwypc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qmertphi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tjqxqjwa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ybjjorwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djzpfqoz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wskekhbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efsghbfh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ofkekogs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3geskmmwe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tyshdahe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tvsxzjst.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wtarnaie.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvpptemw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3miyormlp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gdtcyldu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3njzpwavy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqfqylwm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bdazhhta.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qahfnzhr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fhrrikjr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3agqtnbve.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3igwglyaf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xybulabi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mxeiutdp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yfxslnsf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zkgyivum.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hwokgkdg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ezigcuzp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3knjpwncd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3owwernca.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrmbusm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sltmjbei.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ykolqfls.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yhuocpqt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dvejflgx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vxhvkjto.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qaxuwkes.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3trsuwocw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhfxuoc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wvnawdxx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zmlurhku.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mrvelrki.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lxvqwjts.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ghkurqkc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dokjdwmp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ldxqvzpv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sjpmoixi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nqchwjlu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cfjassbh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fnjdwpsw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jdhirhok.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nialsnmz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3coskkjko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3plsgetqj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3etuaeqwp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pnlxptmc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bnaavaqe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kihhskcz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3djgybtxm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ociunhkt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rxnunhbf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3juhfsgtf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xgtvkexc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pesisuvj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3khzfizxj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cgjwcxug.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xrorgrxy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gxrwfuoo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3oyudkhjg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xvcrugil.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ewhhbosg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xbhzftqz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pjqigcuq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fsfljcgn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3prklurep.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hidkfbym.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3posognda.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xpfmytjs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pvokjhir.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zgsudsqx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlpvcxu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3pzlmfuhi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3leytytor.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ewoeafhj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yodidsvl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xljtfuhn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bgnezfsk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zcyotfsx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gxmllpzo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmtmfrfa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uswpvokb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jlxawmwz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3grsmvtiy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tabzpdgl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hsbwluxt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cjroygox.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nfotrxsi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jkbrrkya.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zwxwjowb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dheqbkgz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dafdvwov.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vnclveeo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xjothtgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oxpdtdqm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3smppugxj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qjalheid.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sazaqmmb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvksbntc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vwwmlxdb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kihngyph.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifqdcqqc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mtnuisvv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hrewnatt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sfmhucxu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3alvhreby.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nbkotvln.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3shmjbjzi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mlwnjbdb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rxllmhgg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwigxzha.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vshlseyd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3infhinex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bapuktyd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrpwcsex.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3apuosnpx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hteqbwid.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bdntuucq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdisogw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfgcxjc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xltzzupn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3eosicvix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mplsykdy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3citnnpng.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ojjfjkfo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwonroch.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddscoyeo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxgpukji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qrbvakbm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ybxaepbe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shhmfzoy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3icytsuwp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3radtcslq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qfeccmjx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rwkbvsob.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vxcwtngr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3emftrbgo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xtjmdhng.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ideeravv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tqbleivm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kolaahcp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3sjhxqkla.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3yyywbufo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ttdbufem.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvaifvbz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvprxcxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gfjbbysv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vntdchqh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3njewewnw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dgpsvvkj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3btafxfvy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lvcxgcme.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lshfcmpp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3yvtizyrs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qmttbbdd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vfuioxvl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3apipdyrx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ctuaojcn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3voogyorl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzqxonho.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mecqwwnr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vyanjwmw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qgdmtpns.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zkmongny.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3llniptny.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqrgcvfn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3avqguqee.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3byenrhqh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bguhbzuj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3abbccxhf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gwyyzyka.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ylpkvadk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mrrtcmxx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pvtpuaho.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3slixzbis.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hcoyelxl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iffuqauj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acdhssbn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nrqjzsfu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jnpntolo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mrplykpl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pnztblvv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qgiqnexo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fogoctfb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uqabjokf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kpyxzlvo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3puodvvnr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qsktbbfl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ijqiniuh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oieuoogs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mlmwvkmt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ejavjdyl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mtampuqu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3sodpmutu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ziwnggkl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ogzusljs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbxowfjo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gysyhxvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3togaubee.html


<!-- 参考信息 -->