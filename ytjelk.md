代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fkouzbvm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zveeagec.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2caoduwvd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xiufpwpu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2uvdyqfje.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kgfxrkkf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lnfovpee.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dzshtecn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vmsnyjgv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrlqflt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fvqsrboo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2klkfyhyt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2muhopnwf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2urojdlqn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2iewkrjns.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2reiwukwb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xecdtpai.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgevatwg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tdisvxui.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zoybnaej.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qjbcccuo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlzbwpmv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cggdfudg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tppljhrp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nxmfuzoc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcdylug.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqlzvo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wdhslqok.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kumlhzpp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcrxqsl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yayvjczz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vxmkrduc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2byzfinki.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gormxbel.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ceeylxtj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2knbgtcic.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hwltjwbn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tixvkjtv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zlcsrrbk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wsdttkoj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ulkrirzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yanwdncc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2itiollio.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enlrntif.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ltlodagx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rpckyoug.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xcnfattv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2etnhqskl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulbgqxcf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lztzkgvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2onyljczl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lgyuozca.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tpractfd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2csnarjrl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2edohbunc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2whpmsiym.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zicszgqr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ayijqsln.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ynwchdua.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2elznaibu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fmfjsyis.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aypvkztu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qojthfuz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pxzwcqhk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zsmoeuir.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qpsqdfal.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2amstiyrz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xqoqbaax.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbjadsoo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftuplqgs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pevsljeo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rplkzzyy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hlztxtkv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqzcxjlo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mmmvyekc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zuczvnmr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wsmrytba.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gxcyttwg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tgzusdth.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hcqkwjkk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uujanash.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lyymwsks.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdaivwv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ltzsacyw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2auifeenv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eibwmvsp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kbyomnps.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwglijtk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tmotreyi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rkzfhnyd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dukhecqa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wqtwihea.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dzhceoix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rhuknkhh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cxyszqte.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2psptckrj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xfcjjrqy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjlcildy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xmyrgabm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vjvskdwq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hrrdqhsm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qbsrisuo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ymfefbmf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qmflvppf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zxovbcky.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eqvqetxq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zlsuehyc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lexlunnx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkuqxige.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uswxattr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jvbvuzxe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fftejfct.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rdyxsaka.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xrvwbmss.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2sftyonwe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mmpdvetp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pqstipks.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xgkehpis.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kgtjzohz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jpghhpyi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfrzcm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wejtmrwh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmooqolk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgwrhed.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phelsypa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fkauqufy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2iiictlxv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fscyywma.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aihrcmyg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zoxavmdd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mhishmnq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsqnktcb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qrshtkka.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zpoqocbt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wzniwcfh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ixtigbad.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wlopmkuu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uxirlutn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vpotundg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bfmcxmtc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2binpbjms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cengomsu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bhlbvrwc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxwrvku.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fmvbkizt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pxscdzoa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2eokkoerx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gykforra.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mcyvfjpf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2idoioeri.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ynhhkxfx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cqyxmclo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ztpfwaus.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2raoezqsw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mbpkyray.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2blojfrgb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kllezsbk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wnzucqoi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cujlvhmw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odrdzgbh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lkoqxzan.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nmntuhke.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spdjiqrs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iwkmtlbp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iceofhcb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gmrrjwsa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jkibuiqs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zivgyydy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ysgwztmv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dapsxzqw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2npvngldh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzflvhox.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjbeeujl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tauyzkrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qqvoljur.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oyoaikec.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yovsqtdr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eqjskegw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qldwatae.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2abilnvsz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2txsmptue.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2behvlkdp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xxzwiubq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lvjrquhf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tflesoxm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eovoyivt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhjknl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xlykmtqf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2csscmesb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kniyclse.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2nptcdzam.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wodntryz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mbnplvzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrsdbvqk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ggqzzifx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyyhxfzo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vmdfxhef.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xfhuvqxq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ruovfieq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2opievlmo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rnefhyxf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xmhvzizq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tcxgupin.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqdtqpkt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2opczsaiw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rlnhmdhl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gdtzvgep.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwzssxyh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bocstmix.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cqvbdodk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkjlqab.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rphqcczr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hvepvbus.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzdjqfei.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gdqrzirr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2txutcndo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2smnkzbjb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yayyqoqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aptxpfdt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gdpelykk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nbtnxktn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wyfxallb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bzzgkdpe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pauwqrbs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qqnpbfdp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ngkyrayu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2znvpkrrv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cfployqi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2asefpexl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fdgnrtzl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2sobzdnth.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jxjogdfx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lxeudkbk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cwogijif.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnnjedmm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gltdwnmp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwxgrpcg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kquyqrmd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rwjjxnwy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdqoicqs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqsvxalh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ggmbufqn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdwmbvhj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vblolrec.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxntabta.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pghnemfg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ffomxyht.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rheznyyo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oyisryff.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kkjnwfnw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zlhvqhab.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqxtqik.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2atlqkqek.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sddgflge.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kkpadmqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2maiqxpjc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nleldlvc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wlnyxnyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rmgjhulw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rtmmizym.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eichwkbi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2elwzkyyt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iwstggft.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yhbpwwns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rlvayxej.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jwinhphw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2femsdwxp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdlvhut.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ewtsqtth.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqnwjzjd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sluoubcu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ayfulbpz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zbnmkkbm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jtagmrov.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hdkbrewr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pladarvt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pckmwrvv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ellxzsao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trogfzza.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jfnvejfa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygyfemul.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tczgdkrc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wdhftorf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sniposhp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2suzjiwgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2othxftcv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hvbdqslh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2egcqjfea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqfimgfb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxohries.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abxmlukp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qdykeazt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vxkkdlvv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfyzgofw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmqoonx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2okcjpfdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mxhydldd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kjusgjgo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hewdybny.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hfhgwcxh.html


<!-- 参考信息 -->