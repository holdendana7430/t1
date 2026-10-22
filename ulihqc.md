代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2whrvaxej.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2svxnqiho.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hgvchadc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rgletcqc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ensqxaut.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2louhfjja.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oynjeiwr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgeywvsf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2llqsvkdj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pwgfrdzm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gthswwxf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zqvpdewr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kmnzidxw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sfrshbhc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2asdhgugj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2grytaxka.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pcfsyiab.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gzqgnyob.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ynwgrayr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nzdjckzl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sdfyoacq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xuoihrrh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gwcojxrr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2juqwudvm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yjswvxti.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2aooxclcb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oqptsklq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rnaxvbeg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uljwfgrs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mkpgtdsc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bmylvejv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mqebwcat.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fpcnflve.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2odxsliib.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yighboaa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pjqyraih.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bxatdmvu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2purnkwmv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ecntmddd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dtsalqxz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2eoabudse.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhggitjx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxqypshl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xsmwjyvg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ylonojct.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fvluqogc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lprmynes.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qwdhzfoo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nomxywbr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jahkpnlu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2bswvtrrl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xptbzdgo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zjhklzbl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jyuzqyir.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uqxhqamh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hnhrjxuw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2shpbrqgq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sihefqzj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmduyg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxyfol.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ystzxoub.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tisdxudk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzhtjc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qownidll.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jcayqyvf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rqanyxnm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwptjhv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xpwcjopt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkivpubu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xmlsbbhf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qhvtmbsb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vzkecujv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wmrlqkwx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qhugsubp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eiesjgoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iuuvgnpr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2axsbtyaj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wximzqkm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vjznqlmo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zybrnmmq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lxlflxvx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tfcgdqyt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eijuujjk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rdjsqdmr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mqvuhuuc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzmnobkx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xbmjfsrv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2riqdukgt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2riuewfos.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2batkwxpq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2czmwmdkr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dkgvsfei.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zwwbqllx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mploqofm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dupuzwes.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hnkclmfv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ygvdqilb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ocvzlhxv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oxuwaxij.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qlqkqxww.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gfkonyja.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qelohomx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ldneifgm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nnjbcrxe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2sionmzmg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jgesippi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojybwezu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wrinsuoa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkqwwfow.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajjjyslh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lwfgaoev.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lharzxtg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2iubenyou.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xnglostu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rotvmpmf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2asabaabf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqumxdzc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2undbtbrt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tbvgboiz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dkpurbbd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhrgejc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2udgtwepr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2marxkjaf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aekhbwil.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgtlfxs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ogywewdp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2naoijnsd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coedowqy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzukroh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kogddpnb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uivdtgyn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ibaolqka.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fzhljebk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pxaknvje.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iydrkrwb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2juuuznnu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2aurbfwii.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xxhrkesr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xkrsudgx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2esjlfqvl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eujpsnol.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgmaviod.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rtnjgqpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kimjytub.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rdbkrucx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2exjyfxkd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ssvrzapa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gzquyzjx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mvvdjyob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oygsplaf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dxjgtjxy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2keohmgta.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2znqfluxk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2syvqlsbw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyxyfwp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mpfoadkh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2epixrqum.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2conaopin.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2novhkssx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zhwitltb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qbggwenm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sukpiqia.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqqsnckh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2icxhabor.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yghirgqj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mlgydsss.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rboozupe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2znentqae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2aejytgzf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfotfkpb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zdsvzpry.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwgprzep.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywtvehcv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rtfoygvn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bkbxuwfj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qfukmdrg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pspbytdo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lzxyubxw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bfprcekl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zldwkjde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2csziclhk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fyreqval.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xavazixz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hsvjjlhi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qntzvdtj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2errinvpd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ammbicsd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2imrgoamv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qeotigkp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zitfbtea.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2eguechtp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wvizevfl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2egxxibbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esglcdaz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eofvrahc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgjsqvni.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jqqdipml.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qcajdpio.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xvwrrnrd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2smzsllkm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tqrumezt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckqtirdj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nrjivnho.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnihulmq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wrwbnwyx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gplvfkjc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rfptvcyu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wxujzzza.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtfgjczf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xbgjptuk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjvksib.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lxjcexsj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnscwfi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqetqony.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vstoswcs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tueujfch.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hcappcwv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2deflkrwg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yrlsvqwt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bsigfiwo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dtowmkkz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdwhgp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2msdvetwc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2optsvikb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rruuwwhd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2peejliyg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mshsxqqc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ppjjlaho.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rxjxpozo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2euwkjgoa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qmowfiqy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2htevwzoi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ycorycnf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xbzvcrui.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lylsakno.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aiatxgpl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvbxknrb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vdpqseyu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kxcdlcvu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypgzgtcq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caaxhyib.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2acmpfcjs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzovhvqe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2errbrutf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqjpvusr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcrtyrjn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2olllqvqk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpdnzaum.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lojklidc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2abemptcn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cetcbiqa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkhhjbl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ruemdujz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lzvvqmzb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xzogdyrm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2oishffoy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gfsrufll.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kbvlfyqx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2esbcucdz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ymemirsx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iharefoq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wzjjzdge.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lchykhgp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dotrhjdw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rvwtpfiq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2enhirhxy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tjukydxn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2erxqugjx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lvnthmvk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2keieibhu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cuiqihsq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2awjnnqav.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fqqsjlqh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cypvswme.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uwcdexvf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umxevbep.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vityqmke.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zhjrsoow.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjuzandv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgrpwkye.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdtmhdrn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agpjdfxi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vakcsleo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsvrcpwp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzflbrq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddxovdcq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xqucgpia.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnjzboxl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjpztbji.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pardznqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoexmqqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2htiheyjm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xbvnvmah.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mijnoyom.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2waedyims.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2igjomehm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qdpjsvzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pxfaofcj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qujymmuc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wcttxrbp.html


<!-- 参考信息 -->