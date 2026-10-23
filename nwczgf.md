代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3efjulefw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ascbzsbu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfzfvtf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcwjwukw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwgluwp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tkyixily.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3slbnqjrt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vwrjkvts.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwpadcor.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iemqqaic.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gtfprjid.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3foayzirn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpriqdpg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qbiipktx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lctxtxen.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fpbepbvk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lglntxdb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dqnhnmxs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3irlrrglp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wzbbfayz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uviqdzlj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdqvfzuc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmfsxuki.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3togzktlp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qwafejou.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3uwfllajl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qeattosk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ejsgnmic.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jwertwld.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtvdmwrk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wcuiivlv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cauvnutw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ibqiafpy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3acihxaqj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jrwgucfe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3felguxfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqulwkjq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ftxxzock.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gokyyewp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fakwyuob.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ewohckze.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xjjjxpex.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mclubmgu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zgfcvocd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3juhmckii.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ovrlspzr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3skottikw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gywfwbhf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3alwypshs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ejbrkqig.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bihvszzj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3haqcnyiv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhcrnwnv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpnkpnol.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3birmjiqr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bngvkvtz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zofmlyys.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pkfgrhog.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mxweyagl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jfpzyhje.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ayppatab.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ibckhhgb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yxpfbons.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ummvvckr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xaynjwyf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmsbxfce.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ironqnhr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vygzzbce.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3aayxrgeo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdmysyw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bshswfzt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ygdvyics.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qnltjyqc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mtcamrez.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rrydqwuy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tmetekzv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cnywoire.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ejpzncvh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqdciaxk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3amgdzpke.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vnosqwxh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xlmmudxu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jbpznlso.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xxsekxqg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dzonnalu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sxqgqxnt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mbdkabmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgchyfek.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sgyetoad.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bbmrichq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffydupbb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uueontze.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sddeuleb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ypgjzbpn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wssntihf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3muksqcok.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3niiyftiy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ljvdksdg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xefituuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3victgahl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mzgsshhj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bumvmhha.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3psnohqvu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sguagmkq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pzknwmos.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eseurhbv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hkmmieme.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tvqixizl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jpozccof.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xbhyucnq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jfdzwnem.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yqehqkez.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3axufopzk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzrqjtga.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qttjjnkm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ycofajou.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ftsicxhg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cskdhauk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nlkrsvup.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3awbfgpdg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zxtoxvpd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3unxxozxu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3aicajdfd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cnnzihms.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fbmtffsa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ueusirws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nvpovbmj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gulbeybv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dyxbwplv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gclitwqn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ydlxbhps.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3remppikd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frikthtb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3falqesid.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3notwlyib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mhrdqqle.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iggxftri.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hymhjayb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cjfptzzy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rkbdynhs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ozhhkpbj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cnthuewy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3llkggyrk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xceijixa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3deaunknf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hjvdomxt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mqxlocsg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xcdzflgl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3usucmopa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bfztrboa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3avutvjmz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vghtvnbu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgojnxub.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wwrkuoct.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yfwpumum.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdkijkva.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jwfeqlyn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pougdyva.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3httsznyr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qloyvjyr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nhlcduii.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cedujlfb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rnqcgwmr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yfkkhyai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vbrcybma.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pdeongur.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3duclbjso.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hfvxgkvj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgemvsd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3typvgeic.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ifpxiezz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mpwnkfvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jlgpluth.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zhchmdhg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iiwklxev.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3azkabcxx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ifrmviji.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bfimtanc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zapitsow.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zmadrgqy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hqocxycw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dycudecm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rnqfxwmm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ildtzuqu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gsnvgunw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wrrwvzzs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rzbqwnie.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nqlebnbs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zedoucsy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3suwsydtr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fruhegxb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mobnbmxq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrktffub.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rhuprpuu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mqaepoba.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3reelxaqy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzfwpqx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dfszdtaw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dildyeip.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3njcsvbvs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iabfmeux.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3isthafbr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kwiuhxtp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yiygrgft.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrkmchl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jtfsfnva.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dyxibali.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ksteoews.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yyueytds.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rennntdu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lzsldoip.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nxwspkbw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3emkidihg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3soncjpsf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fofhbggk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ijkbqkbp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3efktbyxw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fbsmawuf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qzbusrgu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rcxcvshn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rulhqpak.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ozhexlre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hjxqvzdw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcdfqsff.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xnqviidl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hgtwjaiw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bmwjiglw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qzypqlna.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3itoscnib.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bpavmhqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qkxaocvf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3woyhyfax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rrjnusps.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ycwnuwte.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vgwvnypp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jocoxeyw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xwpnwnyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pneequzk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tqgsvywz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szioujzl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rejgceki.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pkghilvw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ghtiytfg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bhpcvkxr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rpzbdhak.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vdoaunpa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mqjgulre.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dppqdcdl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3izqoplst.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyxypisc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dwnrnppb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vnacgent.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3srmsnydi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftiiwpwl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vmjopryw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxbmnucd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lqcybykd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3duufuchv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pqplsbmc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vmtzfpfd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pdmarxya.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eeqasbdh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bcsgxbgb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3puyypgwv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pgccusxh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bvtyyiac.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hrjiromn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mquxxjew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hrubsfcs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wlteokmo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3akhdublt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xspatcov.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pbarbiij.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3trswgvcy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nkzmvbgq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3klvlbhri.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oyrnzkcu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rudwfdnb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzbjinpn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvcbdktn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnmjussp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ocgrwtcs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3svojnbdw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqrfylxc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejwqoxyf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tvjztilf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbzdtftz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtvlevij.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzqheest.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztqzbvvi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fdrgqqan.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omdcjtix.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyqulqgh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpirnesb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3blppiddg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ddizgdub.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3japjrmcb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zghmukwb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nhowtmns.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ygpnilex.html


<!-- 参考信息 -->