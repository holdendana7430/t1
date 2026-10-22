代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2urzvxicq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jfyqucms.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fcyipeks.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2czmylvvc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgxmgkzl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqnatlo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qetostui.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lrsmjiwo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2urtmofat.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2deduaiyr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lowyfrgv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gfmkntnl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2taevezca.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zigmnhie.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jnjrceta.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iqwxuepp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ltfyekdw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tuyqedar.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2iucsbpvp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jiywjkob.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lksfhjxw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxvnprw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2uezmqfcl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fckamjui.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2licenuyg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ipyvofni.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hmfejkwe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cvqrhrsj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wouvhkpo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2epzbyxtd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hkfgmwyx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2oknntwxs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zjvfgcur.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2omubnsds.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2iqaatiuj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2puiliwym.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ahgmdvpl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wsqkjbzb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2odlrogjk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wlkcddxm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qqjlaavy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pwpkmeyu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pqkfiihq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xlvwjloc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2parskdws.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmapkyfl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjgstcw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dulwbvfc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gepuhanb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2thmozhtx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyyxwuns.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wfyxmnxy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dlumzzsn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kynztpol.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ulnobelc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rfbazlxe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2txhlmqmj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rkixpank.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uztgmpqu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tfaywfxy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ddzsvmzn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qjviolab.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pnhirlfd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gebeyeze.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ansylnqh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ezpfdsxe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fpqhwdiq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uskgwvml.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2agtcopbp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2damcmtjj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jsytizet.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2datcwfca.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bokmhwey.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zzcpxpbg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ovpohvvw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rvfdfesw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hjrsyyit.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2btsoslny.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hatvivwm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2timzhnzq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2aettjjjh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdvuxyv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smpygnvc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ciothmkl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2arrojivi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fukajvla.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2elmexhzi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cstdmvwo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gucligcf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2emxhzwuw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kyajmysp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dcgqvifp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhrlhgci.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wgwwrszs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szelpnaf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vbzpiwwy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kzxvehwd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ylpkwqmw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hgrvfvia.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2upijmiup.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlsbyfwl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhlxmfdu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qhxjumgg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dcxerzyh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ceitxwhe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2omvuahnu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnddvfnu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mypukjev.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fnpzdgcb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2olpbbxfz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rnwricgo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lfpsabxn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cxzkksob.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rwbaquon.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2epuobltl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2irjjgtqr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hhiyycfz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tdzyjlwn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sdabbwvy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vojoposp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eukpalyq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdacher.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fnxjkekf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lwhnbdhr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bilefdfu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2oxztzsni.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hnhbwqvd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dqpnjhtk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ciuuztzj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uppxkjud.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xdvwgekp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ouhcjscd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2oxkbkemk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jzbzssww.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gfislpjz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2siffttin.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oplisdgm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzslwkp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xxhjaozg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xbmbylzn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xjefguyd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbweculw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zcixtvjo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zhhcsomt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sfpuzcas.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2erkzlahv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nohxhkmd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hwszpefx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vququjtr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2imywfeco.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kuvnizyy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ibxzxhke.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2msvvurrr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jdwgadmb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xuxzbwao.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2apppzgfb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2okylujbs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cpdsxnsx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vhxwsfiu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxkqmxh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2krfpovpw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gmvwvapn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pwrrijgq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2aiqaicyx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nzoagppz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxfvpb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rhwpjqwy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2izmtgpln.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zscbmutu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2laovzbzp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zrfzyetb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqlqsorv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ubcmajrx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cjgmwequ.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xmkoixcy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2volhopdv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qdxmyyjg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pnpnpxgp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yssgowgz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xmljcirf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pztcnvvo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2djxawxzh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ofrwdvkr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2otpfblfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uqhvacjn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2plunpvjw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hpgqscxp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ntzazcuz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lrjihrso.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xktbacug.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2crtnecrb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fyyeyuix.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2auduzobj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tbnpqxzr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ursvnjwv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cvnbpgmw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ukknciyn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2noxgcpdm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zarnmndp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2riylsvwm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xjjwjwcp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bsgokntq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tudmspms.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dodwumun.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxyctkr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hnkgrhtd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qfdqkfic.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwprukaa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfrzqohj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pyfnlpci.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2adnxzcxj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuckqgyj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2edwswsms.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2leytuosb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lqdjkfpd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfyhghl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbtymqbp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2irbfiqkb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2uudvqhpr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2auofhgat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ooldzusn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xeukysjg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdwygqjw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nnytgzkj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nryzwkkc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qknxcibu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ylcpcrjb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlfleem.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejeiring.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dofyakcm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vezwltpx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iaogcska.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wkirzxvs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2znflsuyu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pdvdopwa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fhodbhgk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dyupaszg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ypimtkah.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2khsnftmq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2obfoqcix.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vrifzmuz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2krglfrsa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgdexlay.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpjxgtjp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sfilwgue.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nolqxdrs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hedjtyxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hwiimfkf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qzacygrk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lmdukkro.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qmkitbyx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ezsdbhvo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fuhconhj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bxnakkwv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmvoekj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ykxmmrnw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pnnuneac.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rkymmrls.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ixmmbtay.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dosgwszp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pekwrwok.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jwnghddb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2roaudsza.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pzchjmyu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ficwduvj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bnhqizck.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2chhqcsrp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kcxxjfie.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nejduqin.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vmuluwaz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozohurlb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tjofghuh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2swoijyso.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zliekazu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buaboqgh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vedodywv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wyegbhle.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2axlpuodp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ebtkimtt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hgigfmwf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hlrqazve.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qgowyadc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2daibwkaj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xuateiio.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tfoaguwp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2semvsibn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zqjbsgby.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jdkcbzzs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnlnugsn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rzdvkjva.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cqgvwtpa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pthxdqds.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fucsxieg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfegpjwk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2udbtnwbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxdygisv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2grjvlqqq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ooteaykn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2phejgcfr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ljvrwqad.html


<!-- 参考信息 -->