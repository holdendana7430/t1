代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuhobmfj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bzuqvbfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klnkmnwx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwvgxzzs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2opwojusg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fleqbgti.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nftohnll.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gmdgborn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zuwjfgjg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jbgzdfpo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zdddejtp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yozfmbaf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hgthsduu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zhrtjxeb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wkootkiz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydexmdbj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dmqfjyln.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dlpjsefz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2llogwoxv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gfjnmmep.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bxjfdjyk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2htgntcsa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ggaiwdzb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2epemscyx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcpnxxb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2trgmrkrw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mkahkbdy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hjkbgtcm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rkabgiyf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhrpyjx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2igpycres.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tgesriph.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ansjyskm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hiofcotd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2suvvupzb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tcnwzyld.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ogtzphom.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wgszbzpp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bouseazq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zccjxmlp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmqrdjcp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vthplilm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ejfzxybt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mnlzmqrg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ospzdgpt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fwsqjpfr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yznybtqp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxyiynwc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gcnqcncl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwffhxhl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dftvpddz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ezhckpke.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nrrfnoci.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xrurizpm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dmyxnvqw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wcoyltlr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fygcogvu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jdhzeplg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ntzwlsef.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pkjlovnm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nokxwlia.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qldsququ.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rkhkeild.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zzculsum.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yirmogmu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gbgqfndo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nfltatrf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjiocav.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tdcjwuyo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nviyjqlm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gqutjwvt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ctcvnztk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mzejldtf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tylcxokd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dfenkpbr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ryofmliw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kgmnprqb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxinuygr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2niyioosa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mxdfhdvg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ojqurduq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nphxhubt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gbjtdlaw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cksvwlvj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rxlsbfsq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fhxdhecn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qgwplbgq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hobdahpd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mihmuxfe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eudeatew.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jkzvxuou.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rywayghh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nsbbkkum.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nikvzywe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2doofbzds.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dndhtygz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttjpxytc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rgekenkp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xhugdeem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2igfvbolc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rhlaeoqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rvlbxyef.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2makixkjp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lndlbtgg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vzhiazzq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lbxeoyyv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tryirhyt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xpidrzsj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2asnujlvh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2odrdzjvk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2eexpwtic.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wseixlar.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tehrbkgm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmbcpd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuexrpbk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqicshpa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ugpvqcrb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cdsntaap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rgcuyqgj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yasaqdgb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zetbgmqh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dubzxdbl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pwagpzxv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2stdcdfdb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ahctdryu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2axzfaxpv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rhsgtspc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2abapjqkr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gxthtdbg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mfqgaird.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gpupkqjs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvvwqgyo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gsaglecr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ipzvgcsz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mptwkqih.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sspbxcsl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2srtkttpj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2sluhhvbr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jnsjaphs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ksgbysix.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ytfnchrg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2berdkwcg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pbqvpuqh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2udogdpxn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hdildqyc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gcrjeqpp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2paraftan.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eodkmppl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2icvaflvj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qvexrlom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wrmvxuqn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbsvdrd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssneqnze.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rhqorhre.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hylkldkz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wiryuwjw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ppylvwsn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jmlehvzq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2sezgesqq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdoimfb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rpzezlkp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwltrby.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2islbnwbq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ynpowwpu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwfrcgnf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ribknyxh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2resqebfu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ubaojxvh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wryjcjah.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dzmolmcp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sskmueke.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tvjtuopa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qujnlkqc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oghjaeeu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xnlldkad.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pzacbmrk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dfuxyeuj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fprzqkur.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlvlepzj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgymgbwh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wohymcrh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2lvfarntj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgumnjqf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rifmrbhb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2owhmlcwo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yipnktdm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cxxgnzdp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wfqxgfty.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dcoliojt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jhicxtwd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nuqactio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2akpwhazl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zmdbaluk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqclfrjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qorvuxbb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xaxhgurq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bhodivta.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2axwjhewn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wgrsbqlf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2svudvsln.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2exeiuibq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbqdmwkb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dfgofcfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2havzuexd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2wkcgbkrp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tjsrqcdw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ehdlkizi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2izaeovzx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ijstyqws.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tzvwckbg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bfqfbtuv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fefjkksj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ekwopcqs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wblkvxvl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ololwpbo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2slbiulep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opvzsfeo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2latozkmj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bxlvwkll.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hvbmhcui.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2whsbipbq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmjeete.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tzlvinuq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zvuqaxqh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rlcrwwbj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bmqfbwli.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cemlhewx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2trztnwls.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2shltuqbi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tbyoiljy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2utwrmpsk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hsbedonn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xbgjxhhj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vnkeysro.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ojeieqxt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cpykktud.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wbczjdom.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tpetxoay.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqlqolz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zabntyjz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qxmwqwyf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kgfjycns.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqqhbmof.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhrvsnup.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffnllbqx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mspviakq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qsvmtjse.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iwynkqrz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpnkvfbf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zljembsz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cutmmazz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2intnzddg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrjqjivz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mratyrsg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfvpnpho.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2salrfpax.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erustwfg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebqirymd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kivpjsfi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2haxxumij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rwbrwavw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dmtstbog.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vybkwptc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jeytfcva.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcmluhy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fmheinzk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2iybqvhph.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2edslkxqg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbnvjhvo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gzfyvpyq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wuavuvfb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2njbhzaqn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbbgnrl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xityieuc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ztkeftro.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dzunlfvn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qznwrspn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieqqhxgg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yvuxgrcq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2htedgjoa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ragzakcu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cebcvvbg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mfktledt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urpqjbvu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2foogsfdt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2auzaqeph.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkbkwymm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2axthfbni.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kioqeydm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pziagbsw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2btgysscc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlkizrxw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpzzogwt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrsxdtet.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yaxjljnb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkqzebnn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pohzcogp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjegibqg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbyfitej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gsbbdjvj.html


<!-- 参考信息 -->