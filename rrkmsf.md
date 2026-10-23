代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pvbqsdbe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3enignadm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3eiwloxbw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fzzkgptf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3snwtwhde.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qfygzmie.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zvyfsqcj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jcdaoifw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3euicjwji.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nzzijfod.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3atfmymjo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ysqrjqib.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ipwvmoiv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggnbyyty.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rardovbi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xtlzmlvt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crdxamfx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdhhico.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3axvuqhin.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vxrffsjs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3odnirpte.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fwkvdtar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmjsdnsy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jzrqopxe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hgkmehvk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pkbdztus.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bgctnvto.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lqldhrip.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fnqscbiv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ijmiqwgo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3amwhnnjf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vwzasbtm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfawgqyb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hsahmggv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrktjgph.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pnivgoql.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hgbrtczr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gfoyeiyn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zlnaejap.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lptjelhm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrszywu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3laadvgoi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xptedcfz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yvxerztp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qkdfgggx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ybpgtqib.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dybsktxg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sgkbmogj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gchxnxru.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zdwqkisr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrftrakn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dlwmacjw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3brrjupfv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anknodnv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhvckhvg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gftouqbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wfqnxizb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tnnatuti.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ilgoylsz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3utsnzwcm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lzoabgwr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zfwoudqo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqwtufi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qmdezfoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grhliytt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3esddkiqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebtfixyi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3piukwsok.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3eksdmkna.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3aovumqsr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wccbwbhj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3diolfwmu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kokgvlfj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hpbhpybe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nzvxospm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qommgjnv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3araharzd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zkoizihx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pigedqif.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nndllqpe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wazigexb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lyhozyja.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3btzodijb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xrlldfdl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lcjpcjee.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dknybuxp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ihrvgpcu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cretlxuz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3meqyqwsr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yxfozlpe.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ykfmirlj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xpjormhw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lmnwqcgo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gubxizkn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vzpkxhon.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tlgeulpd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3owcrgsdt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fovdbvqs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uqupnpgi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gmznfjwv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ziobzgwm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wqzycrpo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jyljvrlc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vssbkurk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qrpmhcpt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bhwlkytv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sswntwdu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xuybxwdj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yagasyhh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kxgkkpxj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tizjjgmr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kbpqmwuw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ifockjwe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgfvhpxw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmrvbnzh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ajrbcwai.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pmgglsxy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mvfkueuc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vlurytwz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hzhveoxs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kmqntayj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kdlfvfgx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qnzvgznt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yvzshmjx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3alkevesy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dinauaqc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fbccysmi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjnuqpn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yldxquyr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3edwtdpxn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uheubflq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xhjbtauc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wwsxciur.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3csllrejz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3atwtqvhw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wyoarmcx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jizyvvzk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3agshudbh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qlablofk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ughlagzt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhyuome.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bgimidjd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vforldmc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iqnowtca.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wkcniktk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3atlbjuih.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mcfrooup.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjmxteza.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3akkhrdiz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ucglrqov.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3isbdgumo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ngcqsqpu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lkinnetj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rjunpzwg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jgzkqmhw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mlnxwetj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rehxfqnu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxqmvzpc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pbtrxnlh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xgrgyxfl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3psmyjbpc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3egjmcufw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3exglvdmb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nelknxqg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3afuvlcoj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nkxgudcw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cfubbztz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pzdobykf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cwoubtqb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ocktkivi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3khrabzlc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3epjflcbk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rrluzvic.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3synpzwft.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rtjeisas.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wlqpiber.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xjbdxfla.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zydydwma.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mynvnruj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iqlovuwe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yomclugq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wfdsoioz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tquophft.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xerfryci.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ukcgxjro.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cldjjzok.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uqznzcfb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3egfvubiw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvcginp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ddccbapy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qzxblkob.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gepcokpd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vlijohdp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3facgffgu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wuoieaac.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3yxbfvdmr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqycchbn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cipibhrq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cssbdbly.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcrnusk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sihfthkk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eaagksef.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hkzseyul.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkswmmra.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rrtnarze.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pmakaunu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hatqehzd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdrjdki.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3epmpkzsc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pqxsvnbu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jonkagsb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jmbxugpe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wsjmwcni.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iszudoes.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtvfyeer.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sacnhtpy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gzybdxvm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hayslxkh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kmumsjvv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3luqqevwd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zywgbxtj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qerriuyf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkuuvwc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tupsbazs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3drxsvimt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vakxxfox.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3utysnxkr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhucbyrh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cwqcghsx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fpnganss.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3beircgbr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bdkjmnno.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bulogciw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zsmzjwrs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pekvrtfg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xererrpo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hmbcuzls.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kdjhktlz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mrwawmwc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wkcnatpr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rhcgqyro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bvobnhxu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3eixrwgae.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3catormri.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3scjxxxnv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3scysvhdl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fpxauvhh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lheruhax.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zonvyfyi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mliqnybb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uadglwsv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wpzagkoh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mssxkyds.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jaioeera.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gsrogudo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nthxjhua.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vqjqdjlc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbpschxa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bvyeumuv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xaxohraj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ajkxmvmk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qpinpcrk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vfxnqwkv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vnpgbtno.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jyfyessy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbibzlpu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vjsnfhvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vniofsie.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqtyqnrt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qezhsjls.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqxvarel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3idaihsqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iopesrzt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxldee.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xklfyvqy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuhhznym.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmyufxvb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zallxkmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bkgkvztu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ikjswxyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khhscicw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nntkznep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dqlzmdkp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hfbwzshg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3oapedyzi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zsgeglwc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qmvlvyxo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3slqokidi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3giomxqli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yidrilxx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vwcglihf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3brkbpbdw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3alyowssx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3urnedgui.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jzduazsg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sszsfedc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3koswseyl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cdulqczr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eawskxok.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jjrlpphn.html


<!-- 参考信息 -->