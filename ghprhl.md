代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgelmbl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cinshbim.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3glzanmov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xqqsdfkq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vjgeizxd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vswgbxth.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rkenmyew.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rmvtuoin.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ngnzlbte.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3muxioxeq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nwhmvotg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ztlltnun.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kfkrlswb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hcmlyudc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ilutpzmv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3frxeqkjd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrlvjqq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uyaizfcq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3holryhko.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mcrvvqos.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wttvhpxd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3odahycui.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3grhbmrhj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oquqxfhi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hjodqgod.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eayaoacm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pgdulcgr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tarotiis.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cmtkzamb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ladhxxie.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3posojrmd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3laybwylk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kamoollt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lvwmsyqv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rnzxbmcp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zgurrklr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3luorcuxr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pwosmrgk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fyihztid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amrsurmv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oqmtwipd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qwvkerxt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vsevnfeg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3skqjhudm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xgtgxnib.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3acnogdct.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3igchxopy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xttwvroe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pxxtnwzf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eateylmy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kiivojfa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3iulxdrcz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3oobjenjy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrofgrpn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gfscjivt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xxwmkrmv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3oekhoijr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mxghpcnr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pbkolopt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qpmgttue.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qpapbuhz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gmxsacts.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tolsaokp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3shdpuapc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hkjuctmh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tsdeqqpx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gleqveby.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsfiiem.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ptejlpiy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otengzfz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vdaunkze.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fbcaodhh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qnkigtnk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vvnaqsrg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cnoguhgl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pogqlmlm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cxocudtb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zqrxyvfn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jnkidxst.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3stihqgin.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wrsamkpf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nfiijqqt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uckkgmyp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3otsjhaas.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3swejvcic.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wtqbqait.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nimpqknm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qakjtzey.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ufpobwij.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iscrpzor.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxgqfao.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uuygkaqv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlichajj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cowhsxgg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hqhwnuet.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tithxkit.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ihhcbbwj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xguglyep.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmcclalb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fdgdhbky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycxmnzvt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sjwagrug.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lwtlhgia.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jwlcxzro.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dvnupkzm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gcxpxiwq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pktqapol.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfvuudbf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3koujxzam.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kbuwrkns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tmhkabwq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fgidxpiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbsbzvo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xubsytdu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kuncsabo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ojernhee.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhrudpa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3frfyhgva.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uocnqser.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gdmugjfo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3sqgfypxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3neojveiq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wlsffobo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fwbhdwll.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fqnjtdkt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rtpujufv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vwdyarbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbmhxhhb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vnxinlld.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ewzjovfs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3chagkcfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3thldwjjf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ehundfrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mlefjwhg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3beltyego.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mgpnunom.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fvviuxes.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kwbwdmzw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vfcgtquk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpurwbxy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqmmxhnn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ibatvaub.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3aojbdpwc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3psjsiwkl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3caeolhil.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzqhtws.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qnaumyla.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lurjlmzs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3abqmkbyj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zpmlmkuk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ilzcaltq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qxuewfvy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hwkvsmik.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgocpwxd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrfthmng.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ubbyllrb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yghmsiir.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3twspkhwj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tigfpuut.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dstspjvg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hapnfxun.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxlltbej.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqaxfxnb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3begwotgh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tdxhsajn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jsypadzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3apqfjzsi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yfleawna.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ulhgthze.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xstpwjpa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gosodrwn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hdhhfmhx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3swmerbus.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kvcmxyhr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bazwzctu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bogjtcqb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vqmzslye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qinovcfo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cgqxqgoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yngrvfxx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3evanefea.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3brhyovcy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iyitghlw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dlzmlhnt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zatomrvb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dtzisuon.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nrczncst.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3witrhmti.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqalhp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3eschcirn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pjsrwzxd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mlajswrb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hniubhpd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ssgfnxrt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jgebajsd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nesxzgqa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3aercwqgo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gvkifsmr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3spqihkan.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lvhypczf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3junwqihv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3agmdqfuk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3edmcmoxp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3enszwkje.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xrmgjwge.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vywwsqnh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bvsrrpmp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzzcyctp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dikqdvxh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3htzqwgrb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfsityag.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3woltjqcr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3btitcutp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nnsqfyxb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zpjoasoh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nxmeczmd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3aetqjeop.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qhflfrad.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ycnikefh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tihfxgbn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qftzytlp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hiuwpypp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3escfbofb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwxqylhr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bujvlecv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rulkwoxi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxiuzarx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3poxsgmnw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzvbqegf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmirfggs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vynrxsuk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhtopgyw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gajhacoz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bakyzzhs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3codbgior.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kgbeybhh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gdavxrmp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zuyqlncu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rrhldozj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sggpiqbo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cbpvuogw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jxbcyeid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ncbvpbsu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pejkikxe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yeodzcki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehkmnitt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wrxvhqmq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ssnytbov.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nhijeahg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jyfzsjtw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xolwqoeb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3prdeffzd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nlkqwrpv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfcyejnm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmwimnbf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gtyegxgw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uudznhem.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ildrtlau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kawomdbm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajetppjm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgoeitwg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ihdcaksj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3joxzlvrj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbcvxwex.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxwjmcix.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apretens.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zgmodfop.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fntyhugk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmflnyzx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfhpfdat.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfweddkf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylmznzyx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nzzvzkzo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubjgnkhz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbnegzur.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uxsjnqbo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wimglrtn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvwprqbs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uzzzywdj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jlxieyjk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gwgiaojr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3guaaejiu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xhizfgfl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bilsvtwy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3truqnebs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bgdvlerb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3njaympta.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xgfhlnmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omrprvfy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dxopdyln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxocsmad.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wkdkcrts.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qzggkblb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fevgtbug.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3byctsicy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qtxytbda.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ickxohmt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3szmdtrwy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pldjhbnq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwutmsef.html


<!-- 参考信息 -->