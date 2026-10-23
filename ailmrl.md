代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vweqigsw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kfptdobe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zpslgdws.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3erwbshet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ijvymfjk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ickgxang.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uazlkpbc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3voiapliq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pfiskoed.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dwhnayxq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fuikmfha.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nkbfplyy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3kgmfezmo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nxhzexvp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kzavzxti.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sbctyuqn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3elmnycmn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bdukercv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3amqpdxvu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jjlricbo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xmzsbsbk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mzclysny.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iylroouj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ohrnwnav.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ojpggohn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3esgvndlo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pphglfew.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qfxijlzw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vyavzasb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wuiaxxow.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vtiualje.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jrvutzsj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fkshffjl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zedwhdgx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sxxtdtdn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oeweefty.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3chhbnmub.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfqkyzdu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bmhbqlms.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gljismex.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3arndfhav.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jvktsaqo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3warwpulm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qjntmfyg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qpefqvgo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lhkqaggv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3upeoxkzi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nmlvuome.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oznjqdap.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3igeuxghf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmzxpakb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uanbwbvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pytqgkdt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3oaccjmei.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vqpynrjz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3setlagpg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ehbvngaq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbsrvqu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uxtnycey.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3walkcpwh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lvalrbdd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3viqpsmiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jbydhjhn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hodwvijd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wzbospnp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3avjgdlrp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qreriekf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uhmgccwu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dheilzdd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uqhiobsk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zapplqfb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yavvudrh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3webhsnjv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lwsipave.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gztoakbu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zqxhxzai.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ngnqactu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3udxdbvtx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zykxhcxp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bfvvebvu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3voypffwe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xxqadahh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tztyzevw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aowddnue.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3slqutpey.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyisvwur.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zgidsjdu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qmzwaccu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3btnxmrcr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tnjadiuj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vpavmnuh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lgqfssot.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3htarupjg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zihyncbk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3llobnphv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vjambvvv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3eqyzkidu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bvtivfng.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezptistm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cofutptu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3njvajsox.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jikymwhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3owowvdgq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iywvtldv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qnxmherh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qlubbvtp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3luabmmdv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3esxgeuia.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fktnmatd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3slunphvj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vdkezptp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ufvkacer.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3krucbleb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lomlzytk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nyhmewnw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmtpxii.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3uthacwoy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kemcphux.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mjagfsot.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ypqshqnl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sswibegc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sfouehjs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ybovagom.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lyrhqrvd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hremzigj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ivdhivme.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jilppihz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uxqtabeb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3faprszsc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mnavqzkq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xyibqgsu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3aubytejt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kohcepoc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vvurllig.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3risgouqz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hkezijcq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iufsbqvz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dophdlvt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oulclutw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iflsixub.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rvhxcgmm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ytpqljvh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3abhjhxsa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkguezkm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3shyntnes.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gmodtwhb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qgqnpgef.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wczdtgzq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sfjjedrv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pqbrhpsp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wafzgrrq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xikzjpxs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xkbynpqo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhtclafm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpifybfx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dltaeojr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bvfcdewy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3edlfvgvy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ineyjuzk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cjlninbh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mvkqszfk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cpcxdnsy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgpvmgz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xlmtvsve.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhebgqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bmkzuglw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vfctncgj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvsitex.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pmywpimf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xrryqodz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qnolggkt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cpakhxie.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzrxvcz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3etimqycr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3onkbxwes.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kkstcezk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eewuhwbv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3twzqvvzp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wlptahlr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3omcwzckm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3quyzbfev.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rhatxqtn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3eoqsdoyq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vlgwljzr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwpnbty.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3esawrfyq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lpqlgfda.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kjosnpub.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bizoeohw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3isuupjjr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3omdmhhzm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ikgcqnnf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yuvtgvlf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rshxswmo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vgbpstqy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jveebczi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yraavdln.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vcejiana.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3odqkreev.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txinijqe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vldterck.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wifkcqxd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3evjxnfep.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gedgsgnp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwwimlzl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3poseipkm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qzahrfpo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmrugvr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cliqczyq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cwigeeid.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wupbdlkv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3csittkky.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hyvdpwfe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sbagmpgo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3laoncwoe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkonpeul.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lgtjitkr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pstphkka.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfpmwscb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfbazcyc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hrvpwruw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qbmthpxl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3sdyryhdp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3txjrvsjz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wpvivalj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gyylzilk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fxyrofzr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3becfzwsk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kinmupge.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mznjwtfy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llwenrmr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tywbttso.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3aalcrgfv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zvpnissf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ayobozek.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xdesqxjc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bdliosng.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qmhotyjg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xvzkdhpd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mqcexdmm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3egfpnoot.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3exrpxbjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hpnsyzyb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lekurcyi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3thwusoss.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gxtoinxs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ytmhkyhc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wopyagmb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ohrvjizc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxwextzr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qgwbfnxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rizniafa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hljxcnds.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dyvqinwh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3suchynqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nfxqagpe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iesicsya.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqrdtqap.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdulym.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncmvrcys.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ziwuibry.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ldgaedqi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xnfcxpel.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3apqpeqwz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3potdrpel.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jeaxlhtt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uyanbyzz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lsmhzedj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gpszfqbe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3oxurpabw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wircxeyt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lcszvbvc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ethactky.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kwyybwzb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fnehulfz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lfycqfcb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nknntftq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dhchvjmv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vwazlwxj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3afxunbfs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mofyxvaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rcfdxlxu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hwnqrvcu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3orwrsgll.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ffkavjjs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3icvqnbdg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kdailngn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3smevtfzs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3khpscwny.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3czysschr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mtusbhyt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgdbzixk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgdumiws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cflxgsyr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hhyqstag.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njnndlxg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ciaqjcch.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3omhlnmwp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3butmlfws.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zqasieal.html


<!-- 参考信息 -->