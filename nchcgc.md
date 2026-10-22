代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dgrxslgx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wullruhd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2csmkdqcb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kwnghxgp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tfzcbstg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ytxknrsy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zbsspint.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2itzzvqxp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mwnxbgbx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2txxknbwy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fhkmyzpr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ausxeeni.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mbbhezke.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zgtdwwcv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azagulqj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2obpdmoht.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gpgiugwi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2aiabycdq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2oksijzsu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bpslrnia.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cfzipssc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mufyncmh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzkyxhlh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tksjqhis.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozscysco.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pnlcqrhn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbvsyprf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ybqtzhgt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jaygueww.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uivncwui.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ogrsxopl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mqsardew.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2unyicchu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2chfmlqxw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmhdili.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mbcraaeu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2phodwnfa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bphniulg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2jjkxdpcv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wraqjcsb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mgcvdxwe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cjagainm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2glrdfnaw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ekuaxdux.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2icufgezd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fihqqyru.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vdhinvth.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wfdqgbki.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yezkyprx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqvwiydm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pdalwrcp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cchctgfz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cmbfyoaj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2twptlrkd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xfeaurqw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xvnbvype.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ftacmroa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nihryeig.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mbuwnvpm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cifmosav.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fnwdicrl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2etqrzlzo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvnjvgn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2thucgmwf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ndcwnfcr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugkrntcb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mcviwkkf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2idqebjcu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fvbpwcci.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ucyonime.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fpsryvyk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tdbmuvax.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lcgckoer.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2duqbbwug.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ybmrfgks.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hsdpplgk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yxzuyveu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgscacqr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rzfpkkhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2whvebogl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rblafvpy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dbihhkyh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2iludsqqg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2hiocmnyv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gwolfmzr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjyjyvrh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mrravbjs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xwqufwin.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2srqhseuj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rpbjssru.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ezesswkz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2crllukrv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gilqqvyr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wyqlolef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2juflyzve.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtezbvk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvuirsmu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jyweeawj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kmkkkeeo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qwaldzaq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hmnzmlyr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oxhgxibv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2oiipvnph.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyoviqye.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kpekhqhv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ettkekte.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mysephhh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjwvkkio.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qevvlkpz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyahsbkn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wyoeafjz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rxvgpjoy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gjlyxvep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sjbxdfoi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwnolkk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jyrodvrn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jtzorkde.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rlxiyhja.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pfncwmum.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gybpjwdf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xvwuyeec.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvavruo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnmxvkhe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gnhjnhcz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkukapei.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dffqnbgr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wpipvgiy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jaabidyf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hgvivzgi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ihjugaah.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uanmthyn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hifincpo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zzezhovf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gfwnvbid.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uydazvdh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcbejlmo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fhvioxpu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2adnauekn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zdlpfjca.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aevsxtwk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vfujrjnu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aeczzgod.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkwduitf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xwpasase.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fxvqxkzf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yykvneru.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kjvkxtda.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yfqxmhiy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vcnascje.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnpqantp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xfywmakd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zucnkgnk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wijtxcji.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cqvcrdxc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wdpmkxko.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pqtbmqof.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qkhiaezh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kyxhfpow.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yczpxrdf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nkharqqq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jbivgwds.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ptqmxgiq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uwrnqeao.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cfdjfsbg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tdnphcen.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2huxzvxsl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wtohlqzl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2grewpbof.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vebhzpub.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vuchxujz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hjnghwww.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qyprrekx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tcfxgaat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahllcpiv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dgbbrjdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdnzfjfq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xfekggwv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qswbeagu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2muezysny.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2igtduevb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qoshajhz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gsmoolba.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wirzasec.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgcimbbq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqaovexo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2czxixggu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xroqqauz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hedvvnjy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvshqepk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ruawvldg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2towwryfa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqsuvbbt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ansnzxpr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cfnaewwc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vhyvfexf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2eqqtjlkc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mxhiypyx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2opjhwzwe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wiyvzlyn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uokmjksk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pjvbhnwc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ehvncgeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fdjjcqcc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kvehpjap.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2njpkekth.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2svxacatx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rhovqyzt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lpoaggyc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gstqwkyw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vawgycli.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dijltluu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2efnuyfye.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jhlqorye.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fflzhndg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urlgvumg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ourpzgoz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prwkvgwf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2psizunlq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ngdsnccw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkdowvim.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stlnujdx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bndcuwyg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mduimflx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lpfsupgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2giofowyz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnarrhsm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gyqfyahl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htoswcyp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2erxjtqgh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yenkjgpq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nmxaumya.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iaiqhyrv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hgpvopcj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2afwjcsca.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ceitekkw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tgdolbuq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ddjbgpyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2aeplqdxa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ygrfjnlo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gqqltzcw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmesenx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2klzvmcny.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kswxonns.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kdwmmrtj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pyythqhm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jnjoyorx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2htvgtdtl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2faaolbdd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mzllvaib.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kptdsyrt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hmfuxouy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nscsczoy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wrvlhwub.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qwfkcpck.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lmsdnmgm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rywcrdnc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nzbqprej.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2egebrnjf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvywyrwg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onvlinxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnooslqh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fjxxjpib.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vgodxczu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkzaatuq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqkvmcxm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxfepbny.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pzjtknyj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpdkooti.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avdgyejj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxyqpdkb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2komhgaii.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2knmovrta.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xfkknzaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqyulsbd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wkmzfflx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rdulkcvd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2nakkrtnw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tlpfezmk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uutuehyo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aklupdzw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fxbgehzo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2geosnrdq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bmrefrst.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vpilfhei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqiijmhf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ygauwbhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgjzxusd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vuhnxmju.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pgcnyuxr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2extxfupr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ndgbadql.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tjcdvwuh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxsyoszh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rbltvipw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cinkqpxk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lvxobola.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hijcqrxw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rtvxkkfw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ialptbmd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wdvdpuxm.html


<!-- 参考信息 -->