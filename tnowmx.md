代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gszvufen.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iltobsye.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjrglur.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kztkhaku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ueqoannq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jaaxgchn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2toevzcyu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kvcfjwye.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lxujvctx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zrizqkea.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xaxhhczs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fdlnafks.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ddfnjlht.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vuqlcezi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ydpkktqj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hilrosbq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mwywtogk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2valzyhxb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tdzlwnug.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ozgxtres.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2desdyxeb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2agrhmvba.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sfpzknua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxllcxoo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zuumqatm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2taujbhlu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omdhxetv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2flqfvqip.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iyuyygoj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yebmxrhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmewpzxj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hgcfaell.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zmajlvjy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2eugpjwaz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hqpfernk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2idtikfxc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ttlgpjyt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nzppgzxj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqhtzv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsonmsry.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2plyjsbmi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jvkyfnbh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ceryeorl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ovdboome.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2canrmzbt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iiwqowku.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2figqrqrb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzkckng.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2igzlpdat.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2boiorscf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fsvubhwv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2pxkgshsc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ubwrqzwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2djqotkha.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cdsrmlag.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ejqgljij.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwixwrli.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cyfzxrkh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hvzecoty.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nmxyamet.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bwnufszd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tpytqqvp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fxbdboha.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qmefqnpo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aufqefeh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oghjmttj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2osizrxso.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdvwxdj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qqehfmge.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ngeepzdi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2utxegugp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2igdnrrkl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fbapghfu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mqxeabvo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlyxtlea.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xbfyhloe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gdmxwaer.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dayduktp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kgenwdhh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lxxhjvdd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yzubzaje.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xzmaizsy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2apvowhbc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dbklhtfi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dkhekyoz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mqcgwwuy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qomgjvpq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2datipopy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2idppvmkm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xllczumy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kvicsrlf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tdquzttm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2biqetsem.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jjufrwar.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hqivgssp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2icvwuhup.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gvmgpwqo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fkfyzkkj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pbwefkof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rpbqmvqo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmfliieg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2povonoge.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dgsgmgac.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2beejjexg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ouifoabf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ysgyldsf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2spnatzif.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tkzknynl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qeztoetx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fhfprcvx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hvnrocnw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2paknxukj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzrvyvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2oxsqpfir.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ohvcpgxd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2puzkzhdq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2njzhbgjv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bqrlunsk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xyxafolb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iewmfxtk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pdjayhxo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hjgzokrt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rjsxenad.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cvgsstoj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mcybtdvu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrmicrbf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrvzfxc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yyxakdnx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pedsvcmy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fxnreuqd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cftrezkm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ewcektit.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zhvywtbd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cpawiwbd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzdhfkk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cocinkvy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vehjcbub.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2usjseaan.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rvrrydic.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uovoawuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2swdishcs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nkqtfszn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bnganhpz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fymjihel.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bvinxipr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jznigndt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dkejmunx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lsadnwwb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2indyfqmw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tptehdkv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fertlkvm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2blmlqdxb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2tnguxyld.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2aurvknuy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2behkaxal.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2asepwcmb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mguzykra.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mewvgqtn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ywpdddrp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dnsorhha.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2icuhrzgt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hbkqqvlj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hzosjyhe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ctqestnj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2covdqzds.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lnfxhzrg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2evpxgeqy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ldiqgicg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2uulpaqdr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rcpowace.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uuxlfxmo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fcrlkzab.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2disckfam.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xasjyhqa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vwzgypva.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dppfzrbj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kjwghdpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzefuneq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2whdnmdge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddgsdkwe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnypmgum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zgnvngrn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhavhcsw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zmxvpqcs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zcfxjxkk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qmdhcjtr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xoqurehs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evomxoqh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpgoxkde.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqevggko.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hnmtdraa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2teqmufqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2colcjcqq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xazjudiy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2aownumpt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uezivsng.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ryajcbax.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bqfdaukr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dkyxxspq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2evtlthtb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dpohersp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oygepzhs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jpwpxypb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2chonvfoi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lhpeolbm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qlgptkjs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2axrhsmqg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrysvbcj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rbxqnfip.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hvlbdlhk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mvmbcgyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cwknqens.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zibvfqqh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mqftnbek.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2stdysknr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cfvgugov.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dbkqdcqq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ypaixqvu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tprjbtmq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vksmthsg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulqytjcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xkyxbbyz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mqhkvdqe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwkajwim.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtwywieu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hghuuefw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2teootsas.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wgxvlllw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqqowsvz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mprusoci.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dipirspc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hiaaeibn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqonlfbj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oreafofy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pnyoxoet.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kwnsbwhx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sycvialv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tdvcvcau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yhvcxeez.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qreabxpk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mauyhsbs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zwapfzyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iohuhkzw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rtkqudwb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyfogvj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dnqcewof.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hkmuygwc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gezkgdfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wzgakqqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jpaujqfs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2broizxbp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mykgeyob.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2olaseguw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qygxqnuz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ljqgmvvp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lxmpylak.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ffirzumc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kmghunrq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nnewdcvs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygmblspr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ysbzeooi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2cwfutfov.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfltbvez.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mqdpdpab.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxxxlfko.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rolkkowf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fgutsclv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlyqwwnr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqfdhajy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tskkaudd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lnghncns.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hiykqdwn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2whyzxxzo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nswleufw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdgvkdxj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hvgaaltt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2evnygoqu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzvsbbsy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2avajsunm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nyqlsvql.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2sdiljydg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jioquuxo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rorenztk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2webmjtyv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2avlbtmsi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sosyvhef.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vletrtga.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kgysljwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynnffxpa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2rektvaqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdlqmxzr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fjxjxqaz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dtzxkvbg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdzaplxv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vtopztzn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zwxadysu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2elttmmsp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tlsqdadh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rwoptzcc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2odqwbivl.html


<!-- 参考信息 -->