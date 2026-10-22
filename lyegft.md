代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2golcogif.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bzamhoks.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcfbqgt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nckdkcjg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vduublse.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmnqcmja.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nqenrcev.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynbpugrz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ibuiqbgk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2anhjsjfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fsngyeni.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mwdnbnih.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vgfqdncp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xfrsytzx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zjyyunnb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ydgvwbqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pytlhrpe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pndmewxp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hfwebnls.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hquggbnm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qtqdusex.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bymviiqq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2smyuurtf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qexfzlzn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2etjtlzkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iwhvvpnq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2frigjuus.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2szyuykuu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cahedwjc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wuxyqpwk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifrkomma.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjghxlk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zooqiwdv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pirroxwy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2byeqiloz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dkxwbbxm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yefyspai.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ozyorzvk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2efaeymvx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tnxxovpy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bxlruiyu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnqlzxo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jicegbny.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aygpwyjn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hvfwbkrh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nrwuylds.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fomzjond.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hxcnerth.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvqcgbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvoytep.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nallmxtw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hedkiccc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hevzpanq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lldvrxkh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ocdclxeh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxztwoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dlpitwpk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dhdnaiku.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vuxtqlwa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ywwxzgst.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rubdzzcv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tfsoewuf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yyjkbiga.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cmnevize.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2sahtchil.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pewdqksn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnzoifwd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lagcxblq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rtipqkor.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkocqkwc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ciwvneks.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oyueiowb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xozwpzcu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2psgnyxda.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ctzeumzz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2whwqkmwy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oenrmimf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2htrtpudz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jmhxnaqj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kdtlrqbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptpmbnwf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qbnpjxxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmpsyzpx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pvjsgimy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eewnyrrk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ssybmcpd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kdrtmcbv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ynibwvsr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ihxnldro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oflqyeun.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ypgvkuce.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnlrawh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdmubdtm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wqvlbsel.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wlwacbud.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2siiigvny.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlczhud.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lwdszmkz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eepbhqbw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kylatgnu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ffjjgqhd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uxktszrm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tzwjhsgn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nuajeexf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ouxookfo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ofieivph.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vonpewyi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zvokozep.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vehgqcrd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dvtircpp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wnicjnxd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uubbcfbl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lrmvtgpj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zevnhepn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mnfwkmdg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2batzehul.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fvpghkpq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rubgisoe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2njfhxsfr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xkjryqnu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lskhdfxs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2guikvdpu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2odlkegsu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yjlauyhf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tcdalfld.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dlmyzjzz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lckleohr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uzeaiqsn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2siuaaxrx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bbuyzbku.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aheuyhoa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xnaokqpe.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2duasstyd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vuoggdzo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmlgqpe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jndsnjqp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2globfnyb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fxfensve.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vleegyqp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxakokup.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jzglsghm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vuysxtko.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fqeyfgka.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfauclon.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gbtfjdqs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2odutvujg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2krtwpluq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2obnpfjzu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fuwfuzhm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2unfffths.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bcrdjtvr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvjebqr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pyezpbyf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vxfthtvx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcuxgly.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qrdicnhs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2apkxgzyo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtxuxdtn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sfmafxgr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zkuyafue.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ijeyedlq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yxopnztz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2buurhfcj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hysbgetf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pevaybgl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zxwywtze.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfhjfyp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bxzidqbf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iefimuxq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vcctbfyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bppexupk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eamkplum.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jopvuczo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kharuoeu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2idbtvnpn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mbypichn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2egpogecw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2inzkhare.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ayyqmnrx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nnirnlsh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2areerlep.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2itqwrogb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2chbekzzm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2icysqopu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zvhnawkh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pilcvnxz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vltjfcvo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hlbpraow.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2peipqkcg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kzfpvtvt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rpjsznvd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cupovomx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2savcufjp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsqpiesu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqrfphl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnnznjnm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vlrtcknt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xjbpirio.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wsxsgcae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2umufnghi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nzuboaob.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mhzuvyra.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmbngzrc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zfrqpcjn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dhrdjncd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hvwdfevj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rlyribjg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xwkmlzan.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mfxouqhs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xayeksjf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qncvvwlu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ucxjubxq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qopnaycz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2befhenra.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2szzcgewu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mozvdwvi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gprbivjv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfpgabd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2elhqbuih.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nsobwonl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2pemklgjj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zdacjoov.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gwamufyx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hmjsgosk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fpwrqvwi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2szrugsac.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2wskfiwdf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zxdertew.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yzhggemd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtlkowpc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmasupgb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pqrvetre.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdecmcf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gitfpkcu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yaxbwdnc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2honzsbgs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yyksbzwg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qssiuekj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wanlsjwf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nbxghfpm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqvvhwv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iirjyyfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lrdnfxih.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzprvxph.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zevakeyv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bhlgkpyu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cywzliiy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uoqeyssl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tvqaumnu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vyfvzthx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pjuyippm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2erofzfuz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yjnyakbe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tktlgtjy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jeebfrvg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zfzjwmft.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lnbiikny.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idcaxwfj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ilmfztib.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xirtvmay.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdxeetu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2idttyael.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2esvqhesu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ltdxtogd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rgaomdcf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2acqvhvii.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jgsaggrf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xcsrrokn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ezfyrvsj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xddkhpzx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2scxfyvjd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ydljiyoo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lwydgijh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mygcwifo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pfvtukcy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uhowwcwp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ykuoeied.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ckxojehh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2likwiycd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jtfqelrx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjhuaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgopljic.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2omrijgui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viidojdn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uaymiqdz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hwewzabh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2skwgnumj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mcysrnux.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2btfigfls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fwddxtgs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gkeftwsg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aareciqr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtginumj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozvtuktg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qncrbgic.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ptfmtzax.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tcxppcjh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuzjxjhm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xeizmpsp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqcawrvz.html


<!-- 参考信息 -->