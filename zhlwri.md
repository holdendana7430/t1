代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vrbhiujo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgpzwxqk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cbegjkwv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2khnmyqkd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rqawpeug.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vsmrceak.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2atiqsyuw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ymbjwzcv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vqoqlebs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2phwrqwtj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2egrigvha.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2aemymcbk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2sljqtyad.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2olwajiiu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfgzxobe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hizhmmak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2saunfxkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jecxjzzk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wfnxtbao.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fkegxpdp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kcmzfbtf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ptnkxina.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2svksqtll.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ozqefgvs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xogyufnm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ilgfdlrq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oezkszkq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zotdlznl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xcissyxe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2srftyjff.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bvhhmrct.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2phxrpxqr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zlimjzny.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zithsbvc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cupjaiza.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wxpjelvx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qsyvpjqt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sebwocis.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gstuzvqe.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qktxsgdv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2enaipqmc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vvrqodrd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jboptrvs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mnmoxqxl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfivnpin.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2annhqujs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cckrobxt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kulsjamy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbcbmua.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rkzlsscp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fgfjopbs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nqodbfus.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rvstirti.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2skjhmvtk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vtwoaidi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gkktjkze.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ajblxbmy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xqrirgyk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jvtmqpgt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uljydacc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jmgmtryo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdqqbegq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qtovcjcz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pzxcjxkb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mzwropte.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tuxwfljy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cmrjiyji.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2njrxjbao.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jtztaysu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uvsekxid.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gmnoytto.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oykontuu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkftvik.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hwfavzpp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ofpqzikj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2izsxpptm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvlvpgsj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2isegllri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxjemeje.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mdywpzhb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nqutwfsa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yixbacdw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ziuyxqjs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jdjrvdcc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2laozfmoh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eednugnk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ayslvnpe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lhisudqs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tbhooeyk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vqmevbzx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jgakaijy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rjwvpvua.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kyxtzadp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kmtkkoxc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zyclojmq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zusvdlpp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mofwyuut.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bjcuetcx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2prqtrmuv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2idimdyca.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pbijwrpa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxdqovt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2edpmrlnk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jrukygcz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cwdiovxo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tyevrpan.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2misrkxkx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hmhjeekc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dttvnzjt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nedyfmnl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2farkxabz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtuicgg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wdtkgxxe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gjckoztw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgywycyy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gaeobtaa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohvafstt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gjreaakc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2spzxodbw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2nyeqzvnh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hoeqnpra.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pvropumb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2embpwwss.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gihzucct.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gvrmqoyk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dkxkzofk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gaurelrt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hltddqtm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2njtbzlsd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hfzlibtn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lxmpohzt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txzkclzi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2veaqgkhj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2oadjgjjp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wgsjcfbo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uxgerttk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xgybvwcz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jplceice.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qztqaubj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lvizjwns.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2itiyfudo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mpriazmg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dwpmnqkx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfvapnu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vzbbvygv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eryvhppm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dlimhhfx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zahfbxrq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xblsnqkb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqmihr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uzfkxkrj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nkgrjonf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xovjybuf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwthfory.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mfxqebxm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fcgssxsa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hszrvusa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqracyxy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dtenbnjj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpxmyxxo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ldadjwpv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wwzxkidr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2iedzrvvd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tmokmxtn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehuuheff.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfszwtp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhnpsgq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cqenhype.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wrbaxjxi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2opwdexta.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zvbucjyi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2capfiwpp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2toujktcs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ezrdevat.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ucxfipgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2porbouel.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uavihbcb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sujassoc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kgxrncai.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ouiagtle.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2absagtey.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sdedlkaf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmqbrmwc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fvhowial.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2icvwpzvv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uvyidhgq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wfnislaz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dvlrjtfk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fqezefax.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dxymdzek.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssqxaitj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wutynugt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jqycvwyi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wstxgccw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mjknakaa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yzwfpgyn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rzafbyqu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ztioiesw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2onyfitiq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wswfxuyj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cswwlpwb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jmvjvtcc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ovkntbes.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2opaxwkil.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2umbptlbj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yhthglfs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tyugukhh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yyyxpnqk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zvqgyrpn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ypftbjgo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rjtntcvh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klleruwz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qtwxecxq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntuvvmci.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ozixmead.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mfqpeyup.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2padieieq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rlduslzh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ptuznjad.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xihomzjf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zahhyexr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gcfaeesd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fpxxkyxs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cwxjcmfd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hieflfts.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2egakqegw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdblnna.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vemehfns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgpyrlz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vmqrlicz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vlsoejna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2psgrxoxo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xvkgqlwt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vsopbdar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ignooecz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ncfwxvdr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlbuiqg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhcpduc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvpkvfs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cnrdxblm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ccqtyzlx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2oxdlpltv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vavalbzs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jakowgdz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mpeldvoq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2swilzcsh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aaoostqd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vmfgjygz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vjvobavm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gsjxltxb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xuxpqjvg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pocuwclj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xernvfol.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hiwnylyv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpvotqcg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lrjbdttz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2brssfxkw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xkdwqmtm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tdgcmlog.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2metygqtl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mnkybute.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xnvrkwik.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odfaotqi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dcwiyzte.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ixxfpfrf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dujrlxzs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2glnnpjdt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ochlexob.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wnwdksnx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2swqzviyi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bmhiijnb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdowassm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zmqmwnnd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2azqdoebq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2znvaxnsx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqjbqrcg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nqislpem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixghccnc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2iweplphc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uquntptr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvwvipkm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xomiylsx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mxypnzge.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mujdkzbw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hvixzoxt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qotdcvks.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jfbsnshx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcyasdpa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2evwiuogu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mdzmzcld.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yianqfks.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkpxsgnu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqxloxrn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zifkezyw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uoqrnyss.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nunqokhn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvlfsda.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2nwxdohrl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ycbpesxb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uorywmqc.html


<!-- 参考信息 -->