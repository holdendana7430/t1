代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wvkcawbo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ofszqfkp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qxtxahbe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3byuheutk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ucwjndwa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gsecipdt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3phrzrgej.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pqntqzpd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjrtxbxd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qtjjvxid.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tigxhyqo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qmwxhxab.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qxaiehmw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ucttuuqx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ejmhcrul.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zqkiwmib.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bddtvaan.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nghxxesv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmwfwqzt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lagjysoq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vnpiocqi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffrjsuuh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3neojrtmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pshtacgp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cmuxgpqy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3htuwfmik.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rulvpbhn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qjunmsxb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bxwqkptn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3svkcqgyd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mxkojnlx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oxxcaiqt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vhknwkhh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qhqugyjc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3txwafntm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkgurdkd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kgewjndc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wyakaufy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3izaqrrsr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ocqdsoje.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jogojlgl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dohlhhmo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iwobnwuk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bdifkwax.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uzycsyzk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3owuarqhc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3guitjfmm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ynxdmwby.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iibvtyrq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kaghjdwp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3szxvzjwt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jzkcnsof.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qldgzhzw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tqyhghro.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbqatex.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xpxezegr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bxwgxgkv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yhutncsa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lufkwmdb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vinqqwln.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3okvwfvhm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jggdywny.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wbsglkxd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hfjeimnx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jwyobiwk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mtsrgcxu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3giqnugtb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwmurajw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cxgzrcgf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yspgoyto.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ycyqkvxg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hxhhkfzu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qbvjldeg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lzfyunkr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xecrzdje.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3itmbdbet.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sochyjao.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3isdhwlar.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpvmmylk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qkhsqikd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3awcgfzkj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kxuelcfz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dhadewuj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzcpagic.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zjnthkma.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zatdilck.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3onpksxsh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jllqdgoc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdgmzepm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xlnfzaqs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtclooh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfwurvcn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wcewobra.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cvuokqhf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3eesoqprk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bqjepoae.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ktsshvpe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aqoaszgp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3sdktxaai.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mwomnfoz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gnixcypd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hgjbxlmn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvubpolb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kzoggdca.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngtowlmz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mrzoejtr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3skjrxmea.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbykbyd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dujocrkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3upyeftqc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fwodlplo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zjxodhxj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3trzfwbye.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lhvxwsez.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ozxobfmy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pqppjtnx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3uacbwbmz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3unabdosl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xuwbzpln.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oockdicx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3iurrygvx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3acdnqged.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfysmmn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lfumfkmi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jpqoazaz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hceolcqy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rxakjnrz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dlnaihlo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mwmunjnw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nvsklmvi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pebonxls.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hhbayppj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lrfutpwf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xtmacmmd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hboeshih.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hsjknjgl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3asvadnua.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zodhprzh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rbxjecoo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3essqnqvv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uqltatua.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yodetqfy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqcctelu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wcxdrerd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3inawlwbr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gwwsoolk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vequacdm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bcuxzypr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pilteskv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sykpnqvr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3loflarkr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ntziytzt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjhakfvy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xmzsmkgb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alhegfzw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uwxnuupr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nusbomzl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cwthtjmr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gwsgxvmr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lzdvuxpg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hltiftoc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iybhxjqq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3duqrfhtw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zazswlwv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gbxlydrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qsijjupu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3munwqqrz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3euwdthvl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3byghmint.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ltdnmsvq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gjntkmio.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ccsbhpgn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zvcjbryj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gemphszj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jqkyibcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izvqroiy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnjcpfhi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ekkwjeyg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3esxgdfra.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ekzepyip.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iwqvbejm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3paibqbod.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3degjqunt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whmrnxhy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gifobrwn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uaxxrkbm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qcltxtph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jdlvfkbq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yezfaneo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xffspgbb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oilrhwht.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xnurbslf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rilbuakn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hxoknolu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3edykpvvy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yiqyugip.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yhjgstri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hgjiepcn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eggrazef.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xmycwhyn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3tsopverj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ionsicvo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pxztoxye.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zqwvqglr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ezmcchxa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qogdtfxs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rzrysmly.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nejtwhus.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3nkklimif.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxrkpwe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3govzfrav.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3itqiqsbk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3siwztkpx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iojtqllw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fshwaqnc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfekcrrw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izitbdsj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ggdxqvec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qszlmpiw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlgqweol.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbjqdzlq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yjtqekof.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okbisomp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbhrqjkc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onjaxvta.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lavaumlj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvwzoq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfcouqkt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xleduxdq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xvszluoi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dkhyjjkq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uhopxxuc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3egbxpuyt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ipvlomum.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qqlbtkte.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lsicpnjn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mscrzsqu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bxfnokeo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3spfoepij.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3axmberbf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3oizhtwxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fdskqliy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ougiobxk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lgpmkieg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqhlowk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zadgtvyv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kwlkoeqv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jijnbcdm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3aekhloja.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clmxiyxw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jwjoasdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xzptdgna.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ihuzraqi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ymfkclah.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kdyddzcp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eaggmjdr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jduicdsf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lzssimzb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spzvepuj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3knznqipk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeswnwbs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnuvbyrl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qoxuackf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jamcjjvl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxztyvft.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sndwtsed.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ktwqflgd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfysigcm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dzcapbin.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvdiasnj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmybhsmo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xyrhnthm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gxgkqzdq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3idhddnys.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eloymlfp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fiwdeyqh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ixxeegmi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3khcitedu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3olthukir.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pvczsplr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3afnpfrxe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ivgnpslo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oeigloct.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jjdqqeon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcdhmpeb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lhraveer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sigluies.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xijzcfrp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hjsjptvg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3udcveoew.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3arweznfj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gcwfxmsq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3kialyvpb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbhueam.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mlcoajtl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbfyvnfk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqgpabbm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uijirymt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejhhmbwx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsalemsv.html


<!-- 参考信息 -->