代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2acovfofw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2eorayqxy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fyexryys.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jzwyxlvh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ycbqynfn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jstqfdhg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wuypkbva.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uephnmbp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fjwtjckx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xldnbrcu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysujauvb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2oyqoeqwx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qsrsxltn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ykghrast.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2loqvaqig.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2unhjwyam.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2unrtmhot.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2etgqlufm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2shhgeehe.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cpjidrbw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bibksldw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2utlvlfua.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqdwkwv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jiihbbbo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fxbnsuxc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xhovlrny.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bbrexphl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2njtepyis.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkzshlc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ikdkokbr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bocyatee.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pncpkeoe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pylhcvuf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2endotolj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mcuvrcdo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xojvslqc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xjmnogtb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mfvhtdyo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pvcahnqs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2smbqboss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mpvzmzxa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2koptntqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2savtiyqn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vumvtbmr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uhwsozqw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arniurfi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nultrjaa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wntgzqcv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwgjuq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zczjxtcj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wsaonztj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2flikdbdd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rvsvrfzo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2navfrbob.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2svvyuhdd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xvrslrjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nprkhyvh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ukukycbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kctyzzcu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dwojupaz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gnsxjblu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pfhzdacy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdxnjffs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zpqetnmx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lvrrqcof.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwspzmuy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uqyfspys.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2reyseefw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ddyhhtcc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aefkifyn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zeqzfiof.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vukrueid.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tksenqog.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kqbcaqst.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vyfkpdcd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2avitlgav.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gvtciyqr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rygtntrj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lihyxkgt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ottpcupr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dmuyfhwa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zxrdhgwh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbyghv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dhbutoyg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kyaaizrc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgxwkqu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jgadlwlz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwzgpfq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qcedeqje.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hprumocm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2reqjvwkq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nyrkwykg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yxpeexwo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2crwtxlib.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jfxhwzas.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2epxqyjix.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2emlfmlyt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yapirtmu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nwcucgnq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2onglrcjl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cllirvsw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pdgsodai.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2krehjapc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ekkzsysx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2trpwarxc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbccytc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2pkpsghuw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qooekvdv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xeaojjrc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ehjhmbzf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqqhaibv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2elymbbtn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2omebrooj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eltftgkg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yommmlib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmmokkfv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhuybtn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2safreucp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uhxitzvp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqxolthi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2aotruzfh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fxobdnxt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2smahygls.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2acglggfu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2phttzrhq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mbxtnxon.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mmkeypnz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qsxaknrs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ctaieanr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oadgitkf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2juwwkchm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nhajotja.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tzyzhnxt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2spxbxxwz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ycveebrw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yrvjakjk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bavbivrk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gsmbuzut.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhodfv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xjlokrqd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zykgspma.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2okwzawsq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fgbopsxw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zyezyuhj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zabdqcno.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xltxrgfm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iqrgbybr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvhwizh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uibbtmro.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rkhzcavf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nuqfpuhd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zayeeoxu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gwkvcbyx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rouqsfql.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2juhvmkgl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bxkcppby.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bercsllp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2awswhlqn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xhncxiws.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qkmnkioo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qdsatbyp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hidumkgu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wjqqgnou.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2apubjvop.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bwmptpyt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nmwbznrn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zyrqfhkq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wwqznyjm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2iwmgwxld.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hcrcniwx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hcskohzm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rjotjsqa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgwvrnk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xarukrki.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hebewphm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bznkvtze.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wyfqpvht.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vwzrazer.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kwmqikcc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sqlcfzsl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vvsffhom.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fhkhdksn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wbgckzeu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rgzlfpki.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ggobvzpt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2getdpyrd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdcjidv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfzcmnum.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cupincen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jheeqddd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2sepbvfge.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdenadr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcddnoge.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sarqwqeo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xibnublt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xiygqigs.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xinccsni.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bdlkiaow.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lnodduyr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzxvvhq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mczxemcc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jmlcckic.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zcvrqygt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uwibgxcg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dyutyref.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dalcsvmm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwkcynvw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kvsgyvdq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rfksatvc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2noviepyl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zobbkeki.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2njikgiur.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wylgfgbx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qcrwdvan.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2inhggrqc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtobdnys.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tbpuptpg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oiweyozs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bqfwtwiw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aojazdml.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwxoiymp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2oddclwsf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2razogkfw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvrexyju.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2blggacus.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gyjowlat.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fojyriml.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mixtdldi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pgyvipul.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vecjahye.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gqiciqqi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xtuhnydc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wffxjlca.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fwuommsd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkfwffoi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2reabvjzh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xdrqcwtw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ywwjlonf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhkyluow.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uzmfbccl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2aijocpcl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gquyxhub.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tylqubwg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uadqjpte.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ctgsuefe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ahgihuvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vtchifuc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kkfahihx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ufyurbun.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgainsr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ohafknvx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kjuatlya.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2feggfveh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2srvywudb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ovceobkz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qjgywlfd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dsyoaqsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quwwmixa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mpnqybgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecrwabkh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfhapudo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nrgeaade.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rybigehq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zwtqqijd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qbartxme.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wofydvqy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2apzyinhi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojxdzbgn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2emzmditn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hiichsvg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nngplayn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeqpvxgn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2arxabhfm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrnhdzxv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xarfrjrw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2oleimqaq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2eldixixl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxdifkrz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tssynnxt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kfjpqriu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ccdfaenb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ktrgtdmi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yoqcnrvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zshuiojw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jgwtebvx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zrnsgpud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rwjssqfn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2phticpzc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lkdgyfsc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2olularrj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2imyxsdnr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xvoaadkv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jelsaibi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nkuzoajy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rjofebhb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2llvmotnb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fapvushh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wmxqvaqf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqefrzhs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvjaehyt.html


<!-- 参考信息 -->