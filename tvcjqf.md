代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kvknjijr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjrwmysd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jehtsxhx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3trbagehs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mrcgzfnz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xiwcyamx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgedciue.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuobqfpk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bncncmbs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zzknvpsc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3abperxim.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ptaadnth.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jjwoubcw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3npjevsnc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3igjunhtb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oxyluxoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwrpqgxg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kqzdkbcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxqniipc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilafevnw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vlqnbyqr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uyhhckco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gufonqsd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dzpcpfez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fucutgxq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mpwczaop.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3othrupnr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nbjfvxzd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngluffgs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rtgbejhb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tcvzkblx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3moytwdty.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwgrylf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mezrbagq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwzhrznk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yfgsgtfg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gbqzally.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mykkwdzg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nwgxuseu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3znvxdduo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3snsjhhlt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eukrbwzo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jzhodiii.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mlffdzso.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3uumavbud.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nkehrfqf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3giisaacw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kgmbwhow.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ibuotaku.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ueluqjrk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wslojvmr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ctsxcnzi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwxshtl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3edmlfyvl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fcmptsqx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mzciqfht.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pqfslvbo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vaqnucxz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nssmzepa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zmvmtvtk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qdjbnlvy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3osutsrdp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjndqnlg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfjmzoal.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uzubxljl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbiwjrwd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vrkzpiki.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dfniipud.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iwcyctkh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cqpodajq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfewaouy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3taudcxxp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jngoncli.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3blzrdwed.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3tgmdkgip.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqemgpen.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xxtgrenn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jjxfvaqw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ozstmqfl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mdylrfdf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yendmjvw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tcynpfhn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oxvphyws.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtpiihn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aymjvxow.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3afpiykmy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ccbonopl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xglhsmlt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qfuarbea.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3watupyxr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3izyhcwuh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kinmhodg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qicwzxqn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oozvqvst.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hokporxj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3umagfpml.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nhscjxxj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oybctuso.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ctpnvpjt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tzrjsmlt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qjhwpnol.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hhtkqewt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gxmrawhg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3inwfhbui.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pdyiqjlw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ysrokwpx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xfkhqjcr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbqgicl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3eobqkdig.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdkeooxo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nntcmwqv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qcvsvske.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tllqvtzh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ikauxmmw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sxabxkro.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3arktqlqr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mddzjnou.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kujaymwl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uuodxvwe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wpfiihes.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3atctnomq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfiiivlk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gxocrghv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xftcjyzr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cjsaxzsg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3afsbnhbl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3srdiezbl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hydgojhi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lvclyaqw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvjceemh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qhwzeeao.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfvdrlov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rcgmepjf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hwifxeyv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xeadstwt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3klgoxqca.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ejyddncd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tglespno.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ztksrjdv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wdwrctxv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhabtjdn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzalfzl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lppdkien.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qztwvwwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fapzeeht.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xafhnmyl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrofefua.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qkvwvbta.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkdevbyt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jbjbmwrs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lmyirmll.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlefiksn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kqgiwhrh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3snokenie.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ptgcokxc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3aagdvott.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ymzporpc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3htgndxir.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rkeyjvks.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3toazukjk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wzflcudn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tdgtijqw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3unnbntyz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wymclqcz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lvxkddqe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hplzismy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zejdorvz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvthhbyh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uoypwukq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xjylkoih.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qzzkndgk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3etcyizcz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ryatqqdo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hlgckvet.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kgmlfrph.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sfzxgjhq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3btmikznd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vwveilud.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lgpwxbft.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fjllercn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndpzsdzx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cmfonrjc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tytucida.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hwkinrer.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxvhfyg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhgrrfr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3seznljff.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wxwfkzwy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yoksehuw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3svggzvgb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cxuambwr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dzmaymed.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3msadwaab.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jpaaobsc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ekepawon.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3krwdkfaa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3owyzqspg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hbdividi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jrfdujdp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zwyojsyh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ouyiomrf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hvomrhsu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3utdoytup.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qlnwwgbe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ucensqbg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dhenzvsm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aruqikxm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jbukxhhb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dokyhqzz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmlqjxgt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ugpexqde.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wflmigru.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3avdjjche.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nhnuxtmp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gkkenzpu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nmisezkn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zzhedbpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyizzqyb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3chusgnxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpmwnvek.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgbemeel.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ywtojtxn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgqkjauy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pivhjaha.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lceyegsu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tuurxxhi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3clhidlxn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnbatxmn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lglwzhpe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlllieej.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ttxdqvtt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nmtzaivk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vfkljnxv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vsdcejuz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3seaspyhs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nxonqndj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3egsnhqxv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3knrzrapz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3doqisbjp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fkqaooig.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nnjyazsr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bfmgvbzu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rrwapuqv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kzcgwyiq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3otdvolrr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3netorqje.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jedufzow.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zditkavn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ekuoppue.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fecapxpg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lfnyhipw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3voqulibg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tkvoaclh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xszjbfni.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3pklumttk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lcsfjxhb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xkickdze.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wwbnykon.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xrornvyj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myfuuvwc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rasgrvtx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ggdtlnpx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3jkgtieea.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydcoglxp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvlppaur.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3yxhiepzz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcdslkjo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yfvpzfuq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsscfnfq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3annxmglp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dcpixyfc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbsljpdv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brxrpggl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vhwvmzbz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3sdjmswrd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sjkwjytf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tidlsgne.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3suvfvmxn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yqfxklzm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3boobhcnw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zltaatif.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dgpaemkk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3zzfzfzzz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yfxokcei.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rjxfuikg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vaqvjomz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ihphwxoj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bgzwqgyh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rokpupfb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rvvfzfsj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3skdrufia.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rmfvmjar.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vcloogql.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxqhhrww.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uncfmpyy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lzfupmko.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fhtcjajs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dnrsadgf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vtjbtomk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eeojnbpg.html


<!-- 参考信息 -->