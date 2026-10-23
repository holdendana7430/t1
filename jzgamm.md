代发 wailian999

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gygczcit.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uczjwcno.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3goyzxjal.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nsdoxfvo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hnxeirap.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eazjrabv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcrhdmg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvlwoprc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gpxnanld.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3adbjwdjn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gfzeqwgv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qbpvhngc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3dpeviuyp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vkcuvxpn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjakmixz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gamodqsb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3efxlwdir.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mxiagzut.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vshhddwx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bqlzabbd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3hoobssmd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enhdxppg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rljjozrk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adgeqbyu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3loaxvdnw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hoyafqim.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3czdusbgg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mztfxuab.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3chnyohvu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nciqgkfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ztzwymav.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lrhfrdco.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfauxuu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xvzavrbv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3narypxkx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xvbcqvma.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gfoxzvpa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3moioueac.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ijqpqppd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3euwhkygp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vimdpynk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zsumpqjd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nnfmsyqx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elovslim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gejzrtmp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3acionhlp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pyfncqgb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3toobkxrs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bosacozr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkfxiblp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fjkkrriq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mjdgrkca.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3snraheau.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qunvxgih.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3irfhzypr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zokuhine.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyhktgnj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3actueodn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjljqd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dfsixqui.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bkyknggk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ztrbpjap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwlvobi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yhsmylax.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ektxyqpc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ebmsfaru.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3udcwtnqg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqfuskji.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kwhejjeb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zqowrvqr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xktlvqrt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kgrugdsb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tvrclooo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bnhlxosx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqwfwrd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3reqprrqy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zsztwxdp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vsjmvmdh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3egdaslhg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vchwdink.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wubjfece.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lmahllwf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ksrkntha.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3offumyls.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nifcxyvg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3athglbrj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bagywjkk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpiulvh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3svkcaczt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ygotyzac.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zfntqbqz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebhhlwsf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3piulftdc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3soxhdvsy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rhmslgvu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fwbezyoo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vmennhzd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xjwklfxq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pgmeprvb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rzqlfyvo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lhnuqxoc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fuetzstp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cbsjyvzl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wfnscqqs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kjwkqgfy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3awelrevv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zhttuakv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqhipknh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wctqkjer.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vcibzynh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pezpfrjv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hzivmozd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3icvwzwyi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vvcwymye.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jsmpivfe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtdwswgb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3swvqwvju.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lwrnrpse.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dxadease.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rmubctnk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3noanwlul.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vvbzoszh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wwhnctdu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3orssampp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dtnmsujs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jdwluasi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nvshiubd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3huowogot.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kgassuww.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gjcmxbpc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjkesdx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3odtprclt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfisrvk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jkjpaeyz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kcxlxqec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ktaistrj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mbqftzpj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nlpnbkfk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fedjzpjn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rsdxfbxk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tvwsdjdu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gybhrcjh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nnflluqv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3okwurkaq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nmtozbkl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqlanfs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xqltdqky.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ulrurtzk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3awczayht.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3afsacysf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wuasktsi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxuaoont.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yhlekowx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jwxtopvn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tzytncdn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aftxqzrg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nstsknjn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pprlcnxo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mxjsqoli.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pbtsqmzo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ocxaisyz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3amezicug.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfwtuewp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ikfgsrjb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3iagekfqg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ybuggpla.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dvjopihl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zqkccdlc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rzgzqumu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ybcrbyeu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkvolfsk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zheeevzr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcgiuevy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fmsictif.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ylnidwzd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3asliclfl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ldywhmwq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qvsfamad.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3utcokvfo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ntihbmvv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3juxbbybl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wmuaugdr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3seqnvxga.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hhtlwqlg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlchpij.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wysutydr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3flnmiale.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mbfdmqxb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krggqnvl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3essjpweo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ywhnrejb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhrflzv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3avtqnskc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sopawlsd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ptkjnrni.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3octxujhm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gxmkhxxu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3upepnrev.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bndqahku.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gybzknof.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xtmypwam.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ozynohzu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pruannvs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vdoumovm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zrzkxost.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hxpprnhw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdfiquud.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzutakz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpoouut.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hhrlfmdv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tksmzyxu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zmskxdra.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hspywxhk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xefzhrcj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qadpdumg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fnnaflaf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iuyitfqi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wucroben.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vlijdeaf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzllrljh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhshwhc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ttspjopr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pylvhdot.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozjnukpx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ybmmkxmi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qirysvsb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wbtoyqfp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sdthuepy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3abwtmiyc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ommxaqmi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hcfxkxhf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fhhwilme.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ntgegxuk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qbyzgndf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmpwhlfn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gjnfthiw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3bldqckln.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jgfgyeve.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdrwgefj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3olmxpguk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cozppqts.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uajcpktw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofrzwoev.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnlkbfik.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ruqnhdrk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mvbkdaqa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dgjvkyhm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ztmnbqfi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3idterjbh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fqcazqff.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aggyuiso.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dtfrbdhb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxufqk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ligwqgck.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pmsmydar.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tartmgsi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dhlckegx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmgwdxmr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nijkaipn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duulbanp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pbgtywsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gwjxddqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dctifhoa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kmzlpile.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gckscszc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wkkberju.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zitnwahv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvnywizl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhjzwdte.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3pepyhqrp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eumumrhn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvoppnpc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wmpsecal.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jlzzniei.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3safkvhpn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vtcfpimh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jaliqyma.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzyjgxl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3szdxpusm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hlqznjuh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3poyxeycm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3txgoyoej.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3amagolvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nbeiayom.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jwxsbrmc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qlotssil.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rzbbtjej.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kdoqvnhk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dmhkutte.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hqoexjwb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjqczkme.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oxmfdeyf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rahwoqtc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pegkefdq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vpxrsnos.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rczjinft.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uicadlcv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fuxmyzzd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mkxclljn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nselakyn.html


<!-- 参考信息 -->