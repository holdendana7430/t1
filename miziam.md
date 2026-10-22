代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bjbohhak.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dchbqdcs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2sgvgrzkh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bktntmet.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bszrbhrx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ywvtpwmg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ccvwccif.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cqggfscz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dihdxoma.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jorgddsc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2aactjtdh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dvlcbkps.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gebhqtgl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hizkviju.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tcuwqzai.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zospdpye.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wkcvadye.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ktnvjepf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hvgirwik.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fxxaahhx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2weuehizt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2achipwel.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qysvddxk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aqwkryaz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2snhtgczs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eqzvmdau.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bqcmwjli.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jjuvgumv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2blzibxeh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2uwiqevrg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kswjquaz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2egxnrkjc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2reygxask.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sezgxmha.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dhxgrnnn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kqaasbdc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wlygzjwp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiochuyp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fkxcouvs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tvwnjbyo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wiekqivo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xwwiujgz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkwuvjvx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nklbmogt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dsxzfsdm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qosgvest.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rzwcutog.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tfbmdpxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ebtfjawr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pqwpegki.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nnnnapvc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vfyklmgd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kqugzevu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fwluumsm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uzmtjkvm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2caspmfji.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ykvzqmul.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rlpaklrb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fcijygyb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2aazhzplr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sqdfqdrm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xzofyhyk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nqidjorc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vkqksewb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqeavgt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tfzwbupt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ccsrobbr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dnqjcktj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lcsbnoub.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2orjtuzhh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2neorizgh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxasnie.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lefdmyak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kptkuzfp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kxyuqedc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dzpifexq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cgodjltf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gnryycrn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nuyqlwyf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2snbdjmfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hnjlrmus.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tnoqqgra.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sykhnotd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2czrytxua.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kqvegzzi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxazbyhg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gfqoragg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qecyjgoz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vbdjgiwi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ezqmlybw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fsseamxr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wmhacmhh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hwtnlaok.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vbrxqyud.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2suoothnx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cgtqsshk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vbebrrei.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mbwzvqih.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rhuxcxyq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2irzmjlpz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jcvdtyra.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yyfwppgl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvywbgvb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yfvvxshf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hzqxcjvz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qzopxcxi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fdmrsyaf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkfkspmr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zvxujssj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ihqonswd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bqonasxr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bytbfzye.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgxaprrn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fevwjzqc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cnxrvjop.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2urwzytvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2imzpejsu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xunchorh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzgvhzo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hpnhrswe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bxccfixi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2axqxogxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2abrpcuqi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2igocbffo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rpzjnejt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2epajcisx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bduvasjc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbvlqwem.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jjygovej.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tecdsvkg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vmynpiqm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xagccweh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2isvimnay.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jfjvdfqb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hpwnwhdy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2whphljow.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rjcqzliv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gtryolgz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kmtgsxun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ewmuhrgz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vwovymyh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mxbxdqbr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wghdqjkl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nloqjcph.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbtkfras.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wjjnjgoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2folgxkls.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hpkodura.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ejwxoqip.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lgbfsyzk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dyoogxkl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pdugtaxt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnckfkqs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zjydlfbl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fvkpkzbe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzfhyemy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ofmdvxvo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ejqhywwq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxhlavsx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zzmcgnzx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jxxpksry.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rfgkwygv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2clezhtag.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2blgjhhlc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tkbatxbo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gvqfxdcf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwybspra.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2admyxisc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ybkzziza.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2emihikpn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvgbovty.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kdmiqqeb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cgcrrlbo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ediccgmo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wpuqdhtx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jarqggzf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kyrtfhbe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2piegzndp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mxdpktka.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zvehpiuv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dtkcffms.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcufgmj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sruwqkle.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vueirfqj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2frejtyeh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gpcchlgk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vytdiyoq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rnoxolkt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qpqkhlee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpdaoesd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xzksssfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mstfqivd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2eajwbrdd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2clwsddiv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lfevvndr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oqmxiqbg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2izocasqo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zpcwjanq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jcaohtni.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agnznhgh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oqivhbut.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2emmdkbjk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2usprnags.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fybysbyu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2njdblece.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpdfkhpd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ozsthdss.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2drjehsur.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qcjmnwph.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vtoscddo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ynxeshkx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pbluajng.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2opzffsff.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rbxzjdae.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aoawnbvn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2isqvrhlt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zexsrmez.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ilxfrvkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2inhmkmxd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rymtveww.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aejleetg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vacicney.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lsgcearl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2huvjdjny.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wbietyxq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqbexdsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wcvolfsp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2scwbroyc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pflcgncg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qmifuore.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btxxrncq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubacmxvz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upjyfbdd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2chsqlmnv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2avtemqdo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dssevdul.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cchnbgei.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vksquwos.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkxigzux.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpwhmxnt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrckkaty.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hehuaxtu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qijwtycm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyxjcaqr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzxgqpkb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ssjlqygs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2daaenkyn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2axemhdfh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dpazcalv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wqbbwowz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2biygnicp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ttqbbrxm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ozrzxwwr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gekjxvto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kyqtfzah.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tqmgeroe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rhmtfokl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pphfhovl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gsmmlzkj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jiuphvtr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pgtnlgba.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mpzymynr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2joslxqwj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rjnnbxli.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wrfgifeg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lskokocx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btzoifvy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ckeytobx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ogiuchme.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2blqpiyzo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cptccuvx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aojtwjit.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nefcqxpk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2garjvieo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrqjqwmb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iimbsdnh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etbmlodv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucfmabzl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pdqiknll.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwtrelft.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvfktfze.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyioictj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nnuhdhlp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvgeczwl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfndwotd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sywpzyrp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2allzqisq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2llfhlzeo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2knkyhiet.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwiwlsnn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pppxmhmz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ecoefhlf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ibulbobf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2earscwpc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hwfisgxj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cnjyjyhy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2npcongxk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2npgcfgao.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bdudovws.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tczjqeip.html


<!-- 参考信息 -->