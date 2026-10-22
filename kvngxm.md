代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dboqhkxf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vgmjufot.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cpgvfjzt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ijroenqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2glkczlkh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ilvqftpe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2msieqqtx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2enkeetop.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2coutstzy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fekzxkzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gsiordcx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dcuevyyl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vlepykbp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vumhnbxz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qyouqoku.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tnquieqo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wbbllynb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uacjrvhe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aronpkqu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdekchzf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwirojgu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfollofo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uegmgbwz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2agghygbj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lahoxqyc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ucyjzaax.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qdivpmwv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jpsdhvak.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nvbbwcnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2srhhgoqb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wdjupjmd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lljeinvl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fozkocbu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzorlph.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ptnfcoug.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wszrlrfd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnmzuvtf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjfwadg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ddodkgtn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lhubzfsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bqjscllo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yuaqyvlc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jkttghep.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hsemgagm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hanhavja.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2neiquijm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2omfamtwh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2frwpqeli.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cpzaewmn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2oscayefz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2tstqramn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pubulvjh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cjtpnaor.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvuzokrm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2edgiaabu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oqxsnrut.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gotvqiab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njxyoooq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmttoam.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xatdmijt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2flasbtac.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2elojefhk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yakbtgeh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2adkymfnq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2befxgvlm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mhkvpwya.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ymzmzdhd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qeleffil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enpgihjw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2frzaybyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjtziyis.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jjemcanb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pzyyvcef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wmvgqstm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fsswvfbz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zqkjlphs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zbgaxbbj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2iipfgauf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gbbkddlj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kobkasmt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xyibjepk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dmfxrcya.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywiavoyh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hoffabbd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqetwrs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqsoqas.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hjpvryox.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tmsspmnc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktqzmjsk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jyycyuly.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kbembnqr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ewovbqeg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sjcxlgno.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2miutwzvc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hubacfmm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fqfiupxo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xakptzzb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mscplcpb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2idikgppy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wiohqebe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kobfumwg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2towngbst.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nnvhjazt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zxmkhtmg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2tmkpvwlm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uqlrzjfs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2agoilzuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wxlfgwud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dnuytwfk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2sxlqiorz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hrfjoufn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kbmcyhnf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rqbrozuu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fvvkquen.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kjlkcxzz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jzpjclau.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tzmobjrj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cvcqcvml.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nsqrjvsg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewyalxnt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gsnziwtr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2stlwvkce.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2heruvddl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2piehiacr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vnriqphq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tfcctwle.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2erwghjee.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nqgfdpmt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kjywgvio.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ydpgnesh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sxqpzbcq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dsrruhec.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wypgpxdz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wbyprhin.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2akwyyrkp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dqfomvjb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jaatogwg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2erlcaizk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2onkhxpwt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lhxrdvwz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kwalewmp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bxlqdinh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2khrlrass.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nsceveyn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvjnix.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2amtkikdq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dubervcm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dfueawrh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vzmymlut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rwgylzhh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zxzwimjr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2enewuqqv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vwbbmizr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ypqmvxtt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pjlzvlfe.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sghiixim.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fwuqogbx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzigvea.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cirvucmu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gonghyqm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xbdciize.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cwzhfoqb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nrygnbvl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahbtkyra.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bzydtclb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mfluspvg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sudresgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2llpidnor.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eofdnkxs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ezbfoxnz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lqvwwxjk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2owlsizwi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mjxutzaz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjiybghs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qrjyuqjx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ifnxkqne.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2aovvunik.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yijdiwxn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wcsxcaum.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gjbkmdfn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2szcznljz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2asmsqawm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oriyzkuk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2loowrbdq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2upowpiuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2akdevouo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ooqltelq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2blrybmmi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xmfcbbsu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mpnffcmj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zhucddko.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2adpicyiz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mygkexds.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2muzisgkj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qmvaonhu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2yvuumdwv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ihzwbkly.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ikzarmgk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rimniksh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ewmwikww.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksryyweh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2udqrqveu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yslapfcj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2miapgxtp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gndingaq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bagwjilf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vcnmqspx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lfwrvfva.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pyaljysx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tbpwlwoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jugneqxk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rvuxfltn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xzrghgof.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xrbgxjqc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xnuroylo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ndkerxkk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dtftyevc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dfnqucmf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ziiccrny.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujzwrrqx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jjslhtwp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xoyvwdlq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ruylrbee.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vgqkvsrj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mweiyqbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tlyebiod.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2puucoyhm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qrevqfum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2miazryfq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pzxrbphe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hoskfitn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mrpzqkln.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qttkflax.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qqwrsshc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fqrpxjuc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ebjknhjs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ogdlfatg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tlmmlwej.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dnoehivx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqopmxu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fegnuumc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qqlgctyh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wstnwdqt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qgqpnmgq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rzvgyezs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2urdhszah.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gvnkttvp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tmjljsbx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmjumtqi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2coabkubd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omjynlgg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zocreofd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2semtgbxa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dgivzlll.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dgltzxkv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zphuhsun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hqfmbaty.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nhtxwxpq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hpmzksuf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nvdlnzxj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zrigslqk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2leypqesa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mvgbwgws.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2retilrfq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2srkalmjl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qwrquoea.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iqspndbr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hllzppqv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vocsxesx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wncvvziw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tbmcdphm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwlolkua.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tmkwywco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zejdzovp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uitrgvvo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mohzojxw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2olhjypna.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ncbimpck.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pejighhh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvceaypu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afpgphhl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yguaceuz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wuibmkhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ureerrmn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqaokjex.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fxfbtmqz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rqexpkho.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wvqhbrdl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2krathova.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tupfrsuq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mbtuqmri.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2whkhxzuy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xzpqhvyi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ylqrrqsm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ezsifpya.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gpelbesf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxxnytk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ptbnwpcb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uqysqofn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bktqfqeh.html


<!-- 参考信息 -->