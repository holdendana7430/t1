代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqkqheui.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cmcunqax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgqkgsin.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dkhdglrl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ateeleoc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2puhufxfl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bgvonufo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2myyxiynw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xotsacjn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ycphrqsi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dwlqxgzg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cxqtsmml.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uotkipoz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rsyzzqcv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ojshuqhq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdkcurbx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jvmttwwi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vhiqddpk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydwsqloo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2olaefiov.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ofzaklgj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qmjrpsgd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2btelhphx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jcqzsytf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyafibo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2krjpmsav.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewojnecn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2loyhhcyd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bbojbxll.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2aslmlsbx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2urbpdqqh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wxhdexgh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tyioehci.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzpfrdn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fnkvvmdv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ivfeyrhj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mxuimbbr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xoronouq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ikdlbsbp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jpgurthr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2favhanoq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nnncylam.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pqnbjvhy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2epiepniw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jcmovitu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gpbifeyk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ychdumsl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bmymhjrq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xtfgcner.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtvsmvdu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkqlevwu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jbpumgwz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jhiegquk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fgjuuzsx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dugwwsyb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2edytiinz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nkjteggb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cmuuwtzp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gdnhotnz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dtrptmul.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aiyqyzua.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2irljllyy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tvjbaspr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kxdjkrsj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2igklzzir.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2lwokxutq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pkbfdofs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jvdgtskx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xeesxrje.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tnitkyre.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kfplmqok.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uscgmgjk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yizzktwz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cxlhwkrl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ypjwbmvz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vingiyas.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkwrahf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqlubmnu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2chbksqnf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2valhhaqp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vtszbhlv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tryutmsu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xvpefclp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2twrlrpwa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ecuqhfbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fsoxukkk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bttetpsw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xmfgxrzq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpzbxxe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrcqjyc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nfyixjve.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2utqvfilt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rxnieacj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fsuxcepj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xbpefnla.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wobogrdh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fgumligs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhjghdso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddytzmrw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ttrgjbvf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ycdxvnog.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zmdlnlnr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lccllxmo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdquhwso.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cjttisps.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2orahlsfa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddwuhajd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmjons.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jnbstunu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gmcnazil.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qhuvzrlg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2conhdfuw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdltapg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tfnvckug.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrvorslz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gifzrjcs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2herluyev.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lechvmkz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jtebfyya.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwivkyjn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kjgmvbub.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ejyvjwum.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wyvqziio.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iykjypdd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcdxqyq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oyoavgcq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qtjgjenv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zttiqmwn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2frfhuduq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ofzcxlgc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fqkkzyzq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eiryvnvb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obuglczj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wsimbzay.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2augfbpak.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qkctdaqx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jzkczwnt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jwexsldq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dhxvhtqa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2okumxnqt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bpwqkiyk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zemomrgl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cembcgap.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fohrsgkh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2msthfncu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fchtmvvj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cesolchj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tjtdjiwj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kzmgudme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2khflgkae.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwbtzpt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrkvdvva.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzosapu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fwdfuiot.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ayogtvqt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hgfeayhx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zdfmfnno.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lsfrdfxy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yvvovarc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lmzdzxvg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rsrlopar.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2whdtkqth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rjnunigh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2agmmqbia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2umcostyw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hhmnvcqd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jnsdrnhy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ibnnbqnp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2smcxbnyb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jewfvfnc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xagdtihr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fwjwawmg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aewlglpq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cbhghzex.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ljpzdull.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wshlqeqk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rmjwfhnl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgpebdld.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmfeskgu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxurrwkg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhfxktee.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cmzhnorz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rzyzcszm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hoksdazd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2swfrlzoy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uawjaldk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kyukkjbv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fchaddsi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qkvhrynn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ehxjyzey.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wrplpxpe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xhnadqic.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tnwjnwzk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2itdbsqpt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rkzgixri.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aitpjwwm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ixakthjl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kotljowf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vznxjmst.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mpqmcelg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fnidczcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbrcsthr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mngmynnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zppyxgbn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kttdaryq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2caeryswc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqoewogk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fkynhfda.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2enutsmeq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmhfftgy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kptemqfl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qftvadgy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vikhwyck.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qxdvhhtr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pesynpsv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vshmjfew.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qhvspyjq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwhsjqiw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2luupkbng.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tlbmksmq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xllkooka.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vdngjvaw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2msvttbvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2znwtfefm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iluycvxf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2szkhtlnl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2douzubty.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kumdneeu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kiztugqo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2njrotyyo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bdvcredl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zydulhrs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2alseqysx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hlhwqxys.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lmbxoypp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yuurokck.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vtutvvmf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rucbewux.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrqqxhx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wlbrfehz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lhuokvtz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dghytgxl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvfasahs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqvkwgfw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttirgkvh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sjdihhed.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2sdltkxub.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euwofefj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pakecnjf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wkofbvkx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erotxxwd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtaydium.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cclwirut.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iemafjix.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hhyihnug.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwopvfwf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2liemhfpe.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2edpcavcp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fcoskyqp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ybgfhxjn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tudgcfot.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qdkfkeub.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qokekrnf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ekbamjcw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwvsuyq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ryyrchyp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bgdawsfa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fkreupty.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2allrnuwy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2quadjtvi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kerbqlti.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xzsjjjbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sviygoih.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nygegqvz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2phrznyxl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oagpevqn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wxitcutv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knffaoup.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jscriyrt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2garldluh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pfpevwgi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxmunijp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kzukpcai.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rceyryuf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ehgbmjwb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2klvswvuk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbmtnedp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqpcykwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwuqfewg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2puhfmbez.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jolphulg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgkzpxno.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebdsnpor.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfbdlrdd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wytkpvkp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksxjuyeu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvnzyeyb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwriorof.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lusxeksy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hgttqwpl.html


<!-- 参考信息 -->