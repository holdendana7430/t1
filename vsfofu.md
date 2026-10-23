代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dwqedxqj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ymgwuhvl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vsymdryz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3spvfrnpa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjosukic.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tupjfpmi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjfsflit.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eolhiieo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubematnw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kkkxxojz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vmgbwbjz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tchruxye.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vqmldwsb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cvzhkutw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pnfxtjcx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fxffynxu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3syfuenpl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vrmctsnj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vxckeryr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ppevborh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wfbwckxl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmgohwam.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3atumyzuw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eejlfcwk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qopvvddz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnueenca.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qujjftra.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hellurel.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3snhjvkwp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bygebyad.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gcwsxobk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fjrldbqx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qvucoexy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nvhhnndq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zthcztsz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtrtufv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jvijnecf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fzcyiglo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nytdcjmw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cgluhyrb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hmfsrxlm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3izxvdwnw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qoybexny.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xovglurl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3etjsghxd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tctfhedz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzienbth.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fppamhjz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzqexcv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gcaluzga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cgyafnpl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zionbxvo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbesntr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iawqknrv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3quiaenot.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pjfvmkrk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cbikvfqz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ffhymbvi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3utkfwuhg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qfsqwonh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3rvjgphjc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gphihzes.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3exgxuplp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xthqbqjs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jecqthus.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sevzufff.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3apsxlbvh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fcrixxqj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fyvhycyq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lhlypaqy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kwdvslar.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txjmejao.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hzlxtewv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gmdmmdcv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vkkefcbt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3azfpmvpn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3cxibazgs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dzadafhk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mskfhzfa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gitkqqxj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hfxquzzg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kovuuxch.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bxghvpwj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pzybmzex.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3daysohze.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3csguvipv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tmfhtrwk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3htehwggb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ptulafiu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wuyqbbbs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qeixlmew.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3evdzgmsu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3flkcrcsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sdihwxfk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ioyrujut.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3byqiyqlv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3avjfiumy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3npoctgfr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3plkdmdim.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ifbmvfrj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ahiwcdgn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mhonrjbt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gsbqalws.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cwpwobby.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xrkiylbc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vokuvsqd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pbpuykaw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iahufojn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqcbshax.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kcoeuuoy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3saeuzorh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilfwegpb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lthvqkeh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ybgbwecg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dklipyij.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3edixbzns.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jxzoqlor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xmzymwaw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cgurgwig.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fadhnslx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vhcbqrqk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mnklxetl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qpjjuwfb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jeytmend.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jcjasnzc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okldhyte.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zgkbuzfb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3scdyteuc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnwjtle.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vntxqmhd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jgwtdyou.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jjbvtmin.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mpxihvna.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hsxgfbbm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tnhflmce.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zowqeatx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ofmtrjao.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3awyjzdcr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zrivjhrb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3efbhcenu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kpqidcie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mazyytmj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rmfyiwrq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvyexbw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okccgqyx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gljzpttp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3noermepq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ujaxhhvx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yuqlbznw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zgzzqeba.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jrbiqlqv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pltdhana.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3faflbpsf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxpxriac.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mlbsedvv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3awctmlvn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wfumwmij.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kirevhlx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yrhfocru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhumopvw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zeeaszqu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kjnzzezf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3npcmrrbh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jjqiliup.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3asmmcjck.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jpedskvp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tboqrmsw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3amofvqne.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lmeziinf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3yszsrirg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pxsmhxko.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tgymwick.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcnlfdhx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rmzyexbm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pnppgors.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3altrlkdn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ldbynaxj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3brmfkxnc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3erzscndh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wxhfkobs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gcmxdlom.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jeyljjbe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtkiafdb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofljxtfj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mrozffiw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpznqxi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wifcimdy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lbzqviyu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qegnrbjh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kdhorlfb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fbpmimqa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lcczfzwi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gzhrdyik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaoyfpai.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dtqluvbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmtvpngx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3btzwjntn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wbclxnkk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fyywgpcu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3julgfzvu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3chkmwjut.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjfqpkjt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qzwnswar.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdnytmjc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yjzsgntj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjrulxhh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fcqkhqlh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaxppccx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sffngiji.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwqddbbe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qapjagtk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rgpsrwli.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vfswljut.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kdagnoyh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cusgcnvx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3glkpntxj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ycbvcshj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wnpedzkh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iixpoifm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3usxwwdvh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wqrgejnq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ugvkajnb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ymnzsbfu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoraejub.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ktulghad.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3owyqetdw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tgkqefwr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ioetesyo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fpurpeyy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hnzugtho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vuxaeije.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lonskkkg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bgkvtfnb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lcvupepm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qektykpy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsebiqum.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbigsumf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3esswfugr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hmvbyimv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sttlsvyv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmxxmnak.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qddazala.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjyhvfwo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgwuihip.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wulhjtmf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdbgespj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cpnbintt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhfqnvgr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyqdsfiz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dscjnbdf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3guslnsic.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3subfrrxp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3swlrwxwq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yofpbenp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3whhcttgh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3llwuftpx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3omoadvbv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdirrta.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3btmzctvi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nloejksh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfaeiog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3azurjuou.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kszldsna.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3igvbpskx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dinuvgol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shozvhbo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ukauijna.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aihyotdy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ogzslpfr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svhikubh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ngkpkcmf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nqgydlln.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gkyyxaqw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nzcjryuh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hqqzobhj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfxhkban.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gsgncglv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hrdvkxen.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnhkxpxk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3feowzzcr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlbequam.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfjywqrw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iggmhcky.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xeoblswp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3suxfoeoq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chlzmikt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ktubeudv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djlksvuh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dvhotgjs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shbcsfwq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3putowcej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zbiclwoe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bzuqriel.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjhomtdu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uaikqriu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jgjjyivs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3iadoyrro.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3piwbtunw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ctafiixv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qcpsxseu.html


<!-- 参考信息 -->