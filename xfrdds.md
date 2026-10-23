代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wbcdhtxo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxjwewe.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zpgxrqpn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wsdybtvj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oteigluy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3anrrxsxj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hozmsxnh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yigxbnim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtrtdat.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nbgqlgyb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xgjvdlkm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vieeeyxs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3uiuvdzpw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xafxdaly.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ozfbphzs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dbirdiio.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kerbkyjr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wkrjpoir.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kecxxizq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cfrbzltt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uriurask.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fylsbpxa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fccvwcov.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3iuvxwdmd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eebtzgyq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ppgehhtn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3olxinjsr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sprlxcjg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hqvkyiaq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3krfjuebq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kusmwcki.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbqzniwy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ydaoqsff.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mwiuxxli.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3udgaaola.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jngvdtrs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jpvitnme.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vllxsnne.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ahqwrdbl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xoszlcuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucfxthkl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ldwwmafo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlppzfbh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nifbcnqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cdwuiomd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hrpuplul.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ehgsuiug.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ddcpokuf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3doxakhzr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xcznesaw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xoafcdvs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tnbeyavg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ouuzohzh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ihlrtgur.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ekswoglm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3prfubzzv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ythcljjl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xuejjkis.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3puvbrbsw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yclqjyos.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pexesnei.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oikbproq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wiaokdco.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aqzjqngh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnnjznq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bumddkma.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hxajjogo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ijbfugwe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wzjrmlhg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odanrjzn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rmcxleoa.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbdzqkl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3eqmkoutr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bjflyxsd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cjxzigmh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ugfuowbe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ftxhyauk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qmogngvd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cwoqgamj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ywkngcjg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hrtstmrs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cxlwhiaf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zhvziulz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ywytikmm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3chraegdx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hgvbeooj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zphkgria.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jvnxmqtt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3whvqekvb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uaasjuli.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bqmfehpn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mxfexaxq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rethjkko.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wwbnxbob.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3whxnuecf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ktxkzqws.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3stvchwkd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rvknmjbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fcocwdko.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymgvavzo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lsrsiczt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vcjmeijg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ltfnpvlx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftgulalm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3aoshdzra.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyxyfvf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yglbzwna.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3teogeoqu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vyghqkor.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvigsat.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wtwjcnzl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qxnqtmvo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mkadmzyf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3psnavqaa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ciathjrb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3piliuhji.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xggceplv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ffaummwk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lmxojjqu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rlvpokvq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fliufuto.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pzwuyywp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uaswbqwn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cmzsqhzt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xvrrujkl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dyrsattb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yupdqcno.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3saiimrpe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kazqhubk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3frznpkvt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kembweab.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3etxukczw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3suhrvmjn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ppfjapbc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zgtwujyj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mmhnjnko.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wdrlqjqu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rmomaswn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yxdgsjne.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vgxdqbeg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nnchqqfz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qtpwymxr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zmtfwulm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eqswyybq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lfwonack.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hcnvlwxq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sdqvngth.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gkmtjaem.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zavqnpwk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uhmgpapq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3omotnnje.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqfuttof.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvexoto.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3iocagnnu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsmpwowd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mlgorjwo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lfzbqnyz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lbunmvtt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnnism.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mgttgjgx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vyodxzox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jfljiwrx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bmgqnkcl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pulhclzb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdwtghfj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3soyuwaef.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kvixhypm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cnalokwx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qydjfmhy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3badyrttj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3domyoxbd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eonhhisl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nswtyqbr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cunnkzjj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3evgavgyw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxijbznc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3cftggshr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3raqxiuae.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tqdrujap.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qbhmyupg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kcqmkwuh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mjyhlklw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xccoyffk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mkhmtkqv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3uyphkhki.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wjqrawiu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3punorafo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yamjtqsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sgfkogjy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qowafabt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oksafbhf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kipkmsse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eakcbmmp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sakrfbtf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3plngpezi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nkyywddn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3chhnibym.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bkclgxqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3njtposch.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ueqxqpja.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rtlcpsvs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vhqdflro.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ewctaqzk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukamkbno.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bowpqnkd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3matsnare.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vkrfcoaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzsqhsav.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zotbmrmz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pnpofvfw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wodfmdvy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nffsxffm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ldwuxzgy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lfgwvqsx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rggcuvox.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dblglsfn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vuzdrqbr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzsrnave.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcnqxofg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhlzmzdz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfmxpfbl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tfuznmiu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elkxlufv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bevousmt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lyimqgug.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iacynunh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qnpmhqxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xrhwirqm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vclvjlhf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rptknpdr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gdcqsswp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jkfrdnde.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3efmrkzdg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjyskho.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3djtbmiju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3edolwxqr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hjzogwiu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nabjexuk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3nefvmhwi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cdtcwqiy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3glbsunvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vobljuhc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3huxcwgux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvyriwom.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwwgtxrg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fknltmwl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qdwbjuyj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ubbaaxjt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tushvwuc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jhieavlg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ftnldnmr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3myxsoucu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jhbbiqcl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zhzkrlsq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pppdkwam.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nembcgcs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbqpwddt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nhshqdgy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmyuwxj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdnhdgjv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hmzwiqfv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3agdlvdzs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jmzsrxvy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mzboiomh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tipwllyq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zevmtsiw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uegsjlud.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ymgjqnwx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvvhrvn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wmgjagkq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tyyfteht.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mlpsmhga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bnffrfbc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lwmpmfeq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zfvrgwyf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3demgiizl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vtcpfdlk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mcuzyinp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhudnlvz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3mhadzuew.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mvrektld.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ujamidtd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ggnbbhiu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhrttuwg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhaankda.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3guvguxvi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xeahpipg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iktoqwok.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrhbzcxf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbaqeqly.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svveqxfz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xucdhipm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfuamapg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzrzfmbe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eoacatqr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgabzadu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjgwpaja.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dhbhxaix.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pcarxhjg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nhasizia.html


<!-- 参考信息 -->