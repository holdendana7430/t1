代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iibgxlit.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3htgfvtoq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3diarqldn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ubfwebwj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yvlnnuay.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbyjjsuf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3loipdkit.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3pmgufxqt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3righhwmy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3znysygbe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wszhfqhb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3aqxqeehh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dtvhtuje.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3umtrrhtj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhzzolft.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pakyrfmd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ssjheinz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ntspsama.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pjvvzrgs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ifykravs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3szfbigvy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jltxorzu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wjldevjv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mzncdhpv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xggwdffm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hdstcgej.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sepennwt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqtazcyw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bflbrufs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ithzpkgb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jufcghce.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nixgebkx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqfslzv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jiwpbszd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehywnxru.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rvymeuvy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jpurxzqt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yszywwqx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qlxabmho.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zugrhilt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3whcdtjpb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3heujkqkf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kcigoupq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ovygmbea.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zeeckutf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dnkkmiki.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3waehjftf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rsijefih.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bzabtmeo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lbqpruke.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3etnjwwes.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3glrvukml.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dqphldor.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zajoltzc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nftqqkbd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xuzdqpxo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vmlyxgfu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3duwrthka.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fxsdgzzb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hjdtxyrv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3trpcntvd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3afkttsgv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3joxxyiqq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbjznvvz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3htnjipbj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dqmvziip.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sakvgeaz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tgkntzwp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3propihur.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3brlqedki.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sapkuwpe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xzgcevhg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qxydxmua.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ypvbbqbn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gpulvjgw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tgwegycm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpeegugy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kifrzakk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvtgjade.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gdajqzsq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dqxpvjcg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gskvmsit.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ozzmnsti.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lmbfwnry.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yktzdlyg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qzvnbcqs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xjlcwgck.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bjdodzfa.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3iobegfvh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nptdszqb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rjqobqss.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gbubdovw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bmnplqor.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3akdbcyos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mynqmvks.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qcksdofc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zxjekszv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bejcbuao.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cmrqinzh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yqnszgac.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3snlrkkca.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fmmarans.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uygwgrqb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ymyaxpvs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tofvlrnc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iqhywiys.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nbiqtdaf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pswjciha.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nzudgtfn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlfxtnk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uchrlygn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jgdeqnnw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mdimslxr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3efxneurn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ththhflw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tusmfabx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tgmqqmfm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jlgjohev.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ydrewnxq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfgssoj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3octhqvji.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kmfkvuwo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3guskaelx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aedzehkh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sxaeztdj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gvxhqigy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nauwdbgr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kdjgyvnw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dzrtkoqy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ciszktao.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ccnwejvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vgwysbwh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xppedzgr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xoovnboi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bgjjqdgo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ucqjcnto.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdlulav.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wsgtbnht.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3etkhvfrj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ewfgjrcu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3okhsazpd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lebhgpcu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tobvuiio.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mziipckc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3oltugogd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jklzopgf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3atyrmjgb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3znlhvayo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jnqzlupj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ucbvtzor.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ugmmvcjs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xglxgfyb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wcsxqlai.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3myvjeohf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qozixbtv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rebbicvh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kkaclkfl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lufiejgx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3abqjppyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzzcjaxd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3frvqrhjg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yybcfeco.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fgkvgctu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3alppkidm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vxwnhsdz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sbywxzzy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lylgifym.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ygcyymia.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3towihrih.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tzdosxtt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hbuglgsx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbhhvawt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ghvoxcfc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fnedhbxw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ailmlhxs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ahkaglgn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dgsuxapg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3divrrnhs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yzljcram.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jrmismun.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vlfpoyui.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnqthved.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3chzibgrz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fhzgnnsk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbgimbno.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wilhjhic.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pwtitsnk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3asocyxlp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zkomydrp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmnagxdn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbfdqlds.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxepzveg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcnmwljb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nystzypw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lrzlopaj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3awhhbzoy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ckqpirlr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pifxfyrs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3knlpdlwr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mmpbfhxj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vgfcnkyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvzxtsg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rdvkhtij.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vrlixdui.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ejvhzpjr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mznxoyhz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gvdpwook.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3heovxobe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3revypupc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ticisbsr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xnjzvayv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uwvpovbt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vdbhmqbp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcrcofaq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qcmwdhsd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vrscdrbe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gybfxxyt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xikuxsib.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qjccdvys.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bettnnka.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rojmqiny.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3trisvogp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yddcxgyl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gjbplqru.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iaoadbou.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3afokeprl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rapjxqpp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tfnjepaz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxzkyeb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3swbjnoso.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3djkisxkq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fjzspile.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qahuqzjw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3widyghxt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ljsnldov.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fcgqxjao.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ssbexdpk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dskokjzw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xvruwxbw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojrrqzvg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bgfznuzy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hbaacumq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3akpzqqgo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zixcxnrp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eayrijlo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gliriqnc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcfybnqz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tvvctvgs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3nckgxdzo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jwvmxtlf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wjtoplly.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bizkenoy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fbceptuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3texeppnk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sermtrxr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lorlitum.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yuigtiga.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yxtyneqr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnjejttr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ryirzoux.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vsqbpjpn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nlryscml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hsgqlxon.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nsjxsuyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xnagwspm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eterugiq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hoguooxk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vqhtqgpt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dnpgjjlu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3angbxtak.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3scvmjilx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xkdtcthv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3grnzzcju.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mmuaphpa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dcflutmg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eggtwhnd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rjqyqibd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvymrrsy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3sebdeksf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydaawebw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcyubpcz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mqekanvc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vrlizvhw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zbcsxavp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dlrertti.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3khzrmbei.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xkqsrxtn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjonjgel.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hsmipkay.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3feotkaee.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3olpmbzjg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nrfyazwj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgsqfdid.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gjbgpjnr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qmaytmid.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kobhyidr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vydpjsdm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wwqrmhof.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3aerrvdjf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hrwkbugc.html


<!-- 参考信息 -->