代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dfnhyndo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3widiscgx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vdppltrh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tlcmfwvz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mhwovqkw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ltvyvtci.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tvfgteic.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xrdqfxqs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jpnoktzs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lparkxgt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yiyjlqeq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ikzavrtd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3odwgctgp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwjdlyn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3svabowmc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rnoggjnv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3holbfuru.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsytawe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sacpnnax.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rpnrqdbp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yaootijw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wpkgxxqi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lxejdiig.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oniaryaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3urdadtuu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rowshwxe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kcasswbm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3thzswvnt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zvargrtt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iazdlaxa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yvhtwaji.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lyddjidx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tefljunw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gpsgbqoa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxennyr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hqfncmvs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jtavnmlx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vxnakdzq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ojacsryj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rxzjcegs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kcpljatr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3emkmtyhy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qithurbo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ymxpslnl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iooftzzb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3urvrjqoi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fcixphop.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3bdcppfhc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3moobvzdx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nretjywa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zqmljglv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbvwulq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jqnqxoxz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3epiyqghf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3edsholfn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3avramddm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gskvwzrv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aeenemhq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tbkklnjb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3txboydaz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tohfrczd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mbujgzxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgftzffl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zorpkxgl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3llikygcp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qycslptm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uzyoyazp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ahqunnmc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lmxwrryp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwhaduf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ztrrdeov.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3knfqimhp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wfaoyqjt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bqosjvjj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jtosjdne.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cztdvwns.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzihsprj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wzcmxejr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3toouqzog.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hxiyiefa.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ufvwucpy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kporomot.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hrdlwxrw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gizpuzfs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sgysvtll.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikdclecf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfynkvun.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mhartxed.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tksuambo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3roygeapf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oljssljq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qrjczdlu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gumxzorg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ztoqsqxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3puaiaagg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xdnujibe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhxdwvzz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zzwugtea.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bpdvjcyf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtyqnqab.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rrvnodyi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3julqiqvj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zprrvycn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pxmdinby.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3grtxyuwr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iwefdees.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hyioskcc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gmfmaiym.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qocgbntz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rrjoaieb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3maogyfkn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3erykxqbf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lnekklpa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jvnryrpz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3zgedfvfx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awuntvow.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3teadyvds.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3koekxkco.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zjibjddp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mzuqnzxx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3grqcjgai.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sdguqmmc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tmggqbmx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ldmukktk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ujdjzuwt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lyjcoymh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3uxinesxu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3opctznfv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yhdpyuss.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ockjtoke.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3grvsiqud.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttrschkl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3smsxkmxq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rzqzpswe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vtqcptil.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tkzeqzyd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qwrjwari.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ihwavlem.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kghtdxru.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3seymsynr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfigccyq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bshzruxo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tfifmkew.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rzvwlfps.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oiwbxbbc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gaoiwkzw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vpfjgout.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ckzjcfsy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rcytmugp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ftmsavhl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hsdpgzki.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wgcezzfl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cvvhhxbw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ebmpphqw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eerneyds.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dgwxxtvk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3chaxudwj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmljkned.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyjunkya.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yfjvoxtm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rdoruxpn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nwfvbnxa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3trelqdna.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3atwcfnfp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vhdzobux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vktbiyis.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gvnmbqqu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dzjupvjd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nhhxyntg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3exxuljik.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wftkvuii.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uqawzjwo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qivibjwi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mezgimvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mrriizkl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xzhiogqc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jbajvawg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xwuttguz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3czpnhfnn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wyuprmre.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uimlugke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltrguwge.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uiqzctgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feinxfcm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtctubyf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3sasgeuim.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yznjpwau.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rhpjezsy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wrrygrlt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xwqacvkz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3uutpcioy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bsliuung.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddehdsud.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kuyhdkev.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kkqorbbo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufxepcvd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxntmlxq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewusssol.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbrekfm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ulzqenum.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zxqpboxg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmxbmjdx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ljpblqla.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qrnwccfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qkffeivx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kltwxsfm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cwnxqszy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ibyobyzg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pwkygubf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cphezsnc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3apmvgztq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaypmjoz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yuqbwpta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uipjnrjx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dmzuygmq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hwkdickg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkjtcfh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fdzhekxp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dtjwqccu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gkhafpma.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oxlosaxb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wdgovncp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ochteorr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvstbmby.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyzsqavm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdasienh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dmwetvqk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odicxkns.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfbskcok.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mykeurxc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3heawahtb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ncckdsug.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbgsjiva.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuvaccmc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocwmolkn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dngxncnf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbwswhde.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctolriat.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gvbhnnrn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnlnroa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3knscrxhw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yyyjstzn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rzkqcvfn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kaneorvt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gnpmnaxi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3egwraapy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xultdvrw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3afrstskk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3islnzngg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wkzwnpki.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xkdxsivy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mkopisne.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3acthqhbx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vuzrbgcw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3agjdzipf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jjqemiij.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wkfeictj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlocswvk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ylppexwr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ogfavbbt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3znuvozoz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nwxjpmvx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tyxalgtl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3httjepnd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ptvmldar.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wiijtgze.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyrtkgiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3orqjbpyg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlzbwizs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kumzlsvl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yvnywpci.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nprjaugj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dyciqukv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mesexhzu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ejdrnijk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjliywwg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yckkxkhb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uxwiqofm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3haemvsok.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwptabqj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3exxnvbzx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqrkrfpu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zefurtms.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hmabefsm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zdujzpbi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qgnyewjr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3irrucdex.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sdbdxbno.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nzmkxrbh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fqazxipj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ozisylrf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vbvlbepw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgmawjdm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jxevhbed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlgefjlo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lbqbznsb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3oeggkmve.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3agjinoxq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtqqppbj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmmdande.html


<!-- 参考信息 -->