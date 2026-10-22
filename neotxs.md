代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfguhto.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xspcjbqi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2smyebves.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xspeglov.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qdhjhiel.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nrattrep.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2adhfpvnt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2feqfdgml.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nrdcgxie.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lvlutknu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxucxmwb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2avaiysjb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pbpetwve.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nnczzpfj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ozluxqsu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lqmzxddk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kgehumys.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wrqvfpvs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kbmclioz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ginehouq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hlmtxwju.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xjcqlhls.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2brsejrpz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lahuijfh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wgqqxdgb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tdjtslcx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmdfjjkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jwouqwse.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xtdgdmxt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hcvoejuh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qoijyrmt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2algaxcan.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smdgzeyh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ancpgbji.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2guqwxvgi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rngdhvrx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ynaamtvj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rwfbpyir.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2sorstqyo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txjqcdyj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wcwynxjb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pintrjbg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nklhqxga.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ptiaiwdf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tbjuatpo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ytlmmqqg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2glylfpyc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pytosfco.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cesyuuda.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lluevoob.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2finbzlay.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2pohlkjlg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fhcjdsga.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bzezeqwq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2razljgdm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ttdpwjsm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2poiibjgu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zlnpxrfr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dbpawotb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wrheacdq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dnzuegro.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ubtyeith.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nhmdrlhx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjatyjyd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bgkmxfsk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wrsfrxqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vnjpqhjt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nnuocakn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2veikclqq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbfxnspn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gcdlwbes.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2grflapcw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lmgaoxch.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbdhjzix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hdebmgpr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jooxzvxu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hqcfucer.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kcyuwfcl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rglszite.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eghjpdov.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ffarvoan.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhgsbzbp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2owjmuylm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rwkxdwdc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2sfuyklrg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cujoxatu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xueyemme.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lpgrpuah.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rahukyqz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucfitgjv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2prjlvhms.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cetonauk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tldfspex.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2isacvhha.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gcgphiaf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2taexdddd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cvylnvsu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mfbjvzou.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2padexmhm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2eltkmohd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qyfwpdqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iklvgzgt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ygzmhvfy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2amkossfp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbryljz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ldoofjiw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dtgmgvjc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ycwzxmix.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oyenpnxz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fjivlfwi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2enuwzjdu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqwetlk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pufibwkq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxlgukgh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vfdjsjml.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ikmrflqi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cxntredc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2odymzaqe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2crvibttc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2thhzgnxa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vvybzurx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fsjgrvjx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jeopwooi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2udekcsnt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ziequuxh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fdgkczzc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nffrzitr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqgoztx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2iumauxlm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ssfvzeyv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2diqyoqzz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yajowgde.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tnwktllo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xqyexkgh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fbfmiqvt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rswothps.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ycjmwwwe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bsallikh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yriohppp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jesgmwne.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vriixued.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fdfkxqqd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jtubjibf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uufwuhjh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pwarpexq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bbdanvtx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuwcdftv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2npwkmums.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bsbhdkze.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rhmpxcde.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ecuompeo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ygsbdtgq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ocnftzfe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qyukpdec.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dakerzeu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wqmmmovf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rwzrbhqi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jlnzcwwt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwkiuuym.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2sgqueymv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pqtkrizz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oodfbiwb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bafgzdnv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2alknrxdk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gcqfuabl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vwmvjppq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sdxirrtz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kiwujpri.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjonsnty.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vienavnn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nvodauhb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2scklwlnq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nykyxasi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2snttwqpa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fxecijtx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2abrfdlti.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eqndpdmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdtwogkt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fvphsdac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vufetfig.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2znpvxtvw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oxnbgnuf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2unmwgfqs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mxcqhfrp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2scvjmobb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvvdowzv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yajrzxsc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxzldmeb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gmiovsru.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofysgmyz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dpzksloi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pbkgpyzv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sndghqcb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2puewqdcf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vbzpmwbj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fqmxxolm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tijfljwy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfheeyp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hqsbtshe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yunjvavi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hemgurik.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vprnpbmj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wbssvrdz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fjqriesy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lkgpddrt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2yzfasuyr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bynionst.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztypdsfr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eloxzkyj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tpvbooaa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fpylpawy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dkioikgz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fghgvfjx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ioogapsu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdstcbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pwzftfns.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2isdxhnbr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zatkcnlo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iltihplp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsiaznuc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqjzhvxb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zucqxsmm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wktqdvyc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2baqbyklb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hginlsne.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ahsikecc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdwobikn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mmeladob.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjadotta.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmqnsvbn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mplorfjp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kosimheh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kismnunw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzavvguf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vaiqccpc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2barzizrs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iyaayhks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oeccrmzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oytajdzb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qjkjfmeq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2piqycmbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gazxufoh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2toqhvxau.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iiheihah.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sqtmiarw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaghcsue.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tlblrwla.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vyxvchxu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mlrutqzv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ildmebdc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2npodvedc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eibebrwr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fdxygvjp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csrdtuqb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nuzifzee.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vqpoubvw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zfmcrbtb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yfsplvjj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zwuoncxa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iglfdhav.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ghmkmzpx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yqkzyzyr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2maalwjwl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ipkcrgcp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krrjlkse.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eftpclrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kdvzuoci.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmzntqpd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eogubwvc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxhniri.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2onvkynbu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmkcxtlf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfjoaapp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dcbmbgut.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulmskuak.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bsfmqdpe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ahbfxaui.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scmhxtre.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nwapgrpv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uswvfaqb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jnaohibt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cnqokipn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dyrkekzh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cjxtxiqu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ywothwea.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ezqtvjlr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kuachltx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eyvvlyxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcfoqbjr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kyiwttus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upmgmkkj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2poowesxe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2npvtuxwq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdpyvzks.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofsgwegi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2levuhoqv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iadnzonz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nboqtgbn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2crgopwlo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xzrsecbg.html


<!-- 参考信息 -->