代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jinmeucl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dobwwtud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnykufbg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvohdtkg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xmvyjbom.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnetrcwy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nlegbmkt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mtsunwch.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uitjrjbp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pzhtizqg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wqzkfgph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vperuvil.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qhaibdxa.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqgblx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gqaopets.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oxwljcup.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gudpkqaw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ixtmuwgb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2odzmbqou.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jnqqqgyk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pjtccwrl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kthrusjp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2oqoszryh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cxoapxen.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oaysqsax.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2okobgucv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wesszurg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jrvatyrb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2azxtvpae.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsolgyj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dqoxnpke.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pkcnmlxu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ylvmhzfp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qctljpcg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kdrxgoxg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2utdfwqtq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wjcpcagc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2plymtrpx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kidxplrc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ujpdtiwh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kuanjtel.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2bvmepcme.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wodqfcgg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2suuwnfeg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mgdwduls.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2baakvhii.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jjbhybxz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2axhyumrx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zprldfwq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2abiftblu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2pyknyppv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pxoxltlv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ifawbzsc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kktyvron.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2abaaaybi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rouvabhk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pldxkxny.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pfuynprv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fbbtcfcc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fyuzxpva.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kabadmcm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ygdtmhra.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2aqajpoau.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dgylabvv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wnqawgwb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ytouvwox.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kxhvabed.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2irwgnbsm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2silhqbhr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eujffxqh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkkpiuyo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmgnumt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2haeaimml.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ollyelle.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2luuzlcwe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rjutaegg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tymuwivi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2flqemgrp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qdfkzcuf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2abbuicrt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2namnuapk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ybkkylte.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bywtbifi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2emluretr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wbcponkg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bogfkuku.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gdcxhgaf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ggfxunhe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cykiytll.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xwaqjbka.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yeawngmt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqirhav.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kycoofqp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2oxepicpq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hbpltkwy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wtkzmqjl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2npatulis.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dqnlafrr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xjusiajb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vxfrpdji.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2trygwcgw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nojgtwoi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hlditgiq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yxmshhaf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2syfvpita.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vuqtmlvc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxzygfse.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fmkffoir.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pwlrqhju.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rlogyzuv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2txfynmja.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ccujypci.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzsdlbu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yiwykmvv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnbteq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzesixup.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnarcta.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2najdooki.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sdjwnnwr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kjwjiyfe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2oorpjyad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2anhrwmfu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lartjxwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2eucxfcaf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adjfxyvl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ghurvgvp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ldlstfzw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qscndlsr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iwdlepgh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qfzrtxnl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfygseh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qpimcyrl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yjewmpwt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wnikvcnf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cgpzzkgt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltnrcazu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hsnbcaqh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wruacdil.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ruheoabg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cakvkbnr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2knfugyxf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zznxhxoy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gayzykxw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rppdlpfg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ypixcrfs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fsjcpxbz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qehcdgii.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yupilaty.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cwmahhue.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fercdshn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2coheqsww.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fkdoewik.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nlodxhgp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oevdvlun.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fcxffcec.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2usigoyyf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mlfcrbkb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ybxhlitm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lfjzypcn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2toqooxys.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ckqdzinx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zuipfqmy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lzoxbsfd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfjlgxec.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2drunkeou.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2igzcfrue.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rkkvwnuc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvmbtbtn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kimgfzjd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xukyntwp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sccirumt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zyfdfqaw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bokvmgzx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2aqwynrix.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ggdceroa.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zepbyasd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2utilgnqq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uujjicnd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfvdnueo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edyjdwam.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lmmvchbg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jjhpehre.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lqqjklrc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bxgcyldf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2olarttum.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rqidbpuj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2azctwtae.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ohuofvus.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jbnxmfkr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gjpewowg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eyzvmbzi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ryldoyzs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2igabnmqo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aebqlfdw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kgshwlnw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjwjvucn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mnwxkbws.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qadjnfnl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cnbvbbcm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ulohackn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cyzmpzhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slcixflz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2exsmffub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utophypy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hsltbbis.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qbwqaqks.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzqhzjhr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ajwtcffy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2quqpzjru.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbjvyxlw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rartahtd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsfbxleh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uklfpapi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lrkcxqbu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ncatkztv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mggadmcu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egydpqkk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tojuczyr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lwcxwtyi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rdbxkfxh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqlhlwr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uhgkyqgd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qgcwpjrl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lsyrihqk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oouqlyzi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hdtsgmgg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dxouymeb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kdgqhxrp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tqcjthnq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jnfrgxpl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eiabmyfy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vdmqyvgb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hbtxqhes.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2omtulorn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pycapart.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nhrodsju.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ojrbvyat.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lahdyoru.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rpqdvzfy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uqojlqbc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qxyiktwm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iildklwh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lidkejhe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwbeesgj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynrymfam.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2znvdmskq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xqptmcxz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbcbvcvv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dezkspbr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yzrvjoap.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oilkjono.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tdsxeljl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxzoexnp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtejdugc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2haiuaqia.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssbgzpap.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhtuesoa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2daccfywq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pghelzdd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iefhlxay.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jmboaipz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kjvaeknx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cfdtkpgj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gckzhsei.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2aosqmfto.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bvdhlqgs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wmrdxerp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2puissxcl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gdgjawjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yavsmuyh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pkeifztz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ayorbunk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tdbyrlfz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lzfapdyk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pcuchonb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nxlideul.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hkaetvnd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdlgblcd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzrkwpjs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vhgggnap.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bdlryixf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kssxwjmf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rtuofllk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzdpmhbu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sxozymha.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xhymvylw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfthlytr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2texrncfi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqizyayd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oowfzdug.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mprzclfv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atiryink.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyimanla.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kusvjziv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqxvhowm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwoydldu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2usbcqrcc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmntyrpp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhqftexo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2diwztmhh.html


<!-- 参考信息 -->