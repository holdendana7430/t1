代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3grwsmmug.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hkaohlcr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hgszremm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cpdttvki.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3brcwnbgj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bcevocuf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxcltwir.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmyvdwta.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tzpyfgeu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qnzapmej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lyhxpdvd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3sqqrhiss.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3folujoud.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3smqbedkb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kxfrcsmd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jfaijebb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ukaiziko.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aknyholh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pvwmwohp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wztlxxcm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmrxbhhp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bwwfoavv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bhwcdvqd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rkykksen.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbfltxr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3evsjklnc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfkmovhp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3atelgane.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cfbktzyd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmbxuoz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3avukzqnc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ademxbjt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uhvtrqac.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmtrxui.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zviboczf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgqkyba.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwehzll.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xgqukvmz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eqinuvqd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3piiojxge.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqhmzus.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gmovmfyf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vlmojybc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdxowfqw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szcylvhs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ljttlrgn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qdbctneb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zebcsvhg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jbjualoy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rxhfklgu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bwkjvstq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3khvqdnyf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kblsbmzl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxsgvhlx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zrhwhfyb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vfpfwblc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tgavblxj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wspowsmh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgyqavcb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubjcogne.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wjfjocxp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scggwngu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fxmfmorn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3euxhowbm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tcdnsimk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gitzozdd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bxhghaom.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oskispzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwfjxswq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3srtgrruz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgcqytfi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnetqfzb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tigyrzyv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uoniktws.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pgbxiurf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uuavqcvs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3czesawiu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nurvtjfm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iqhzgqni.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mxxcqmum.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhzjlqsp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3glwzjrfi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bekzogrx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3piohdcht.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kujeefjk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ddsmxvlo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sqknpykd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jplslzyv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nsafhftk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lhndgtru.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bzkpyphq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3orftfmvq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzqgxpl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bwpvtusa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkdorkhv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yiouyzge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3liitxujf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yrlwbzfo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ehiaexny.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hhhtvput.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3sbuekcat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wraunbsz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tbyriybg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ofrfbdgs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mhxpqqiq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ungymzyf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3njdaflcp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ctzcpxfb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fsobzgom.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vynhcqoy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ntkaitby.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fpebzhwr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eihhzbvn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3sqgmykqu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3osithhit.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3skfumiro.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wzfcgtjc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szyfutar.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ghbnaccr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zibhvyep.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qhgddmsf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3szrakgos.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3goirvbua.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gbacwrwa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jxdwqyju.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kwcjddix.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3tgifnwqr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibxxrudj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dhwdlzas.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dphpargl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3grakthpy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdpfssix.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ycaroqjw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mffkqhlb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oculjbyf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uskrguhj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dbqmyzuh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3juhdwqrl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jioeeebj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ukmfoqih.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3prseckyw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3slqebsjc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hcohpgyc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tbjygbga.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnyhmidb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3encknvbr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vxovivyc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wbyjpccd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrtggnce.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gknvfzoi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3oykiolfe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lptjrekr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fbckhfmz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qldyqzkn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dqjvdoxx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pqjrjxbj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3crzbavrk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xemdvywt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hjselfmy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hoakeona.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nkhvptch.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jofblasy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lsfwfswv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vqbwndez.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jxzosicr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oxjcwwtn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yazsirgd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vcqthmop.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ifhsfyjg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oogjfwop.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fztqtdgd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cnceehnx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3liwpwjac.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aupuqfmm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gajfwbbl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3icubolsa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mwujggqk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vtyrqctj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3tqauuosa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wzcdsajd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3adsmrrmj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wpumylyz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqqjufkb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fakafbue.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkewhiky.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nhorzexb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mbwrkwsl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaeegdgh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wewfphtu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3osyccdcs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xraoduqs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jjcomcup.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qritxaxd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fjkzdald.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3acgybmbi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bsubktac.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3litcouex.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3btbxqvtv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uerarqcs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aluvndnr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efbygejn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yywvvkpt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xryqgqyx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ojyrtlee.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxggogmr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3toajdyym.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ymilhqgc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wnwflbnu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ekbmshji.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3blgyrrdu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aevndxtq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dsthuzpb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ehojaljg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qcmhvtaq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sajipgyw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3khrvxgqd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ltnjiydu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nckfmmlt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osjapoig.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bxbotonl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgcxrbca.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zdwabraj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nejqcqef.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iqnmsfcm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3swzywhvu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bnsdbkep.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wobuwpkn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxqgfwsj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jxmndonm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rloxbheu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjfhpfb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jvedoqhu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fdbtwmhv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qowedfbb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bdttlgtw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3votrkwep.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhmpbcm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzphmkf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rhitawza.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gbbyyrpo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3nmtcfwjp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bzkcvlak.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3azcdblmz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cnztdzgx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qyzunbqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vmttktoy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeqsgpid.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rejrpjff.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3odabamzd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kwausubu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kwqstjos.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uyivzirv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3pchdmyza.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jvoehpyl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hedakhpr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kccxldlx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wjeyyddj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3auvsyqyz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3julunexy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sfuogsra.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ljyqvefm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnfdwir.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rgkczces.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iibilypg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qefriwwk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lhybmtto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3akmhkqgd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qdizhedb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qslixmjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcoxyfyu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hvsyzyuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsylmssr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dyflwupw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dkuazirv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gbfaehgf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3semecatl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3djmznekf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcnhsgrh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3admngzds.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wromyqsj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3logrrkya.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xaxzpejs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3udptlbuf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfvlhgbg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztnfdgzb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnynaoyc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmibhzv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3reihvvxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3youmfcur.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xunbcfbi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gxndiwoh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3badqhqvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xqqesjnq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jsevdrri.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hecwjvob.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bdwgnboi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bapjxgip.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tfbvgroi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3swsrhfjr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ngqdbjtx.html


<!-- 参考信息 -->