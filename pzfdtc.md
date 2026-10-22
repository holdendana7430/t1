代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hiqeekss.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gkujfclu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2eqkgmelr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zwxbgzyl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pevujxfw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2truzabzx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kpglyinb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2derobell.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2blmezpbl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bjqmkbvg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ktghpkgo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2auqwebqc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xvnarhjj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qhgiynhd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oikmdxlj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kuwodxtb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rgubxwbe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wekizujd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oscnidnl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2abwwokwq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2smrhwovf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zslayxft.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gopwbqcp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rnqofzzn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tdcvsrpo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mzgxnbpm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2esdmmipl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2guxfbepw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2azwakuxt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fxqadyhj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gnqyivyw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqyuwkri.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yulglihx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dpjymdmi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dwmaljyb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtkkimqz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rjvlcaqd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2btinwgie.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2prhwljzf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hddcgdgj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jtnumstc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbdrooc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2smnmusfm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rctcbpoq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oiyuuylg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gimoleun.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxtdhjp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xoaetzpc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwikskir.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gettdfef.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jlfdfupl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ilbthczj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iztanbrq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vqsyhvgu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uizuuzjb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jymdiyqm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yxljgvoe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xtznvoxm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2eppqvkge.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wqbesevz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zbdlegcu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jabmhqug.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zekdpjgi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hndwsldx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ktcqvhce.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2smltvwsr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zeuggzcq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gqaqoynd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rbvuybqr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wycpgxne.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cqebmwdk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2acwpksdu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ogioxjpk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tmxwijsx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vundiqey.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wnkfedsq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dipwdxym.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytauubaw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qapghfgw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sgynxmkk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ntslgcgh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2flofvnrp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2uabhylqq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ystsztiv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xkcwzgrl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qrogpcuf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnxuoaku.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hfesoykw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2susutrzt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aooojhkt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qtuehpka.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgbajmqr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2huwhweat.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mekidywa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lnjdcode.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gscmrhjm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kypvrcaj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2huoomhml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zvjonbha.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tqpzboje.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ebkrupdb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2upksilox.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzbdbgov.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wuctveta.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2veekivru.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vcveszyf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sabrmhvh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jcnfpddv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfnpnyzh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2klzovadt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gaftuqig.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxvjrkdq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gwtkwvdr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wtbngsfc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oijlavdi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hsvpkfte.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2flcnvbun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dchckven.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ljcwbqcu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ogdvshcc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ydbbmsam.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bwoxruju.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dpzlbnwy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ewmirrws.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fxkaelxs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qnchgebf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vowgeyjo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2elffansc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2njyvlavl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rigbtven.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lzgldkgh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mpilffnx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2djpllbwc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvqgkkt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xxsdzbjh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hlmybicc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xnhnwjmb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bryyjrkk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jeodvtru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdrfqaku.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpzpblg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqdnmml.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhqakbmh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gbksjtmc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2boaemwhh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yxqaqmcf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xzqvoxns.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2urypeaiv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2udoyrbah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gzoskfvr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2snxnvizd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipfgskho.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxnxoqur.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ocmfxyir.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgokhhvk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2weknnecx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fsrtyjip.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tcupcoef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xeeethoo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hzlpqmed.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eqqncjkz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xwgcnckj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2niqlaudf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yczcvkmk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yecsfqnx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcnesqmy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wqnylfgh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2usqpvpap.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eexuhdrf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wiseouco.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rmekhkkr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xometbos.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ophajlic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzmpovrs.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hsymorub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sruesxgt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2onkjgcuk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vuzjsgtx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kljbanba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hnsdupmi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xuoeqqmk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxmvomeo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2flejuwby.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxajocme.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jdphvopv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2pplqtawl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2phqszllw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2eckucwfl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpcjmvdo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkswabkp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ppmjrefb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gzgggnmq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2cnmttrel.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkqukog.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jneegwjv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhyzbns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ueqrlrei.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2abqjfdtf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mzpomnen.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iqhtoufo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qpjlkkbd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gixkdnao.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uilvfauh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqddcxoq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lkteyoyt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kglfsqxj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ytzckxvg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2leislblh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zfxtuigy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ankmbslh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2osjuzgph.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fyvynoti.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jxelxyth.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ezblrmvw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixespsfi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahlqwlrj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gynkfnsb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2akmdnanr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jkvgdggb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwxgosyo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltwvmlux.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kwnpbjqb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmmxowkd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afosdkaa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egxgwhrk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eolcmpmw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sycdzsse.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mkeaxenn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbzrpggn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2evdocwbs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gibupmwy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fpcgguxv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qwdqnwss.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2igysyrrc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kdjeuvnv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jhnvtimz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zfhmnywn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2raagawfi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rdwfhyhk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ahmvxiju.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2izpxkcve.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xutlnozm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2klzforjo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xqvkotqd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gtovzxgk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dfsnvrjc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ayqpjozy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wwonveqn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gqnaxupk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awaxpqpt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2axnggeko.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2btwvuycm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ealolbxo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zqtrdptv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2afpbsslp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuismisa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pgobubwz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2deddarip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhtjxw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bxwyaagx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thvimuul.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dihinsov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2klgyvtve.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otlwtzvv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnssmcsa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2biebelln.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2omdtszcp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2afjbdpdw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izymxaiv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eriqorjr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2twwhidyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlphhfvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kbmcnjem.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2heexbgsn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zblhwnkx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nbglpkeq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yatftyqt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hpheccwx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cvpyyxyo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gleanuig.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wqjpirgd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sqycroqd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jzpdujkw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2djevwmwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obacvvmy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fvkhmzth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grqorhdk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hlfwfnxw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ioudxxih.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emailcqf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdsxgthd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ynmntlek.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2plqnvmuu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zpoiisci.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vapipwfg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fltnqwry.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zaldzugm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jefsihxl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfolgjgh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2coeajnkn.html


<!-- 参考信息 -->