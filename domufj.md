代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3twzbmzux.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hzkjnlrf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qeyhnenl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fmyidujm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gcsylwxg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qmxuwivk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gikluhun.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bxmzvkei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pjaxuicb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vxomnnvo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wyehlpxn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bakevqjy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3arooolzp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aeryixym.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zzklankf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ndzvltif.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sqiwzzvn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xbxbmktr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cqhnvpza.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ooehrned.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mzuiuwvc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qnnvmyqx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tgethpdz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zjyeftvh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fcpygpxd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3trailrdb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ckcteopt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3amqnyery.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3asjwiehi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3aznmyeuc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jomerhbg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vdbwoleg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oyweifvr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3shyransn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ogqtlqui.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3auhjhsfz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3spzlqftp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kfatkxyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xydkaytt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3udappdgv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xblfnnxp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3suvxoivf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3frkbjnyh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kslmjuji.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rjoqkant.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3moywkoua.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jishtrsj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fpipyoqz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvpndgi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ljwwqccf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oquwnzun.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3odyxoexo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vfgvhyxh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fdquldda.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fhrfspcr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kghpmxkr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dddxjwkc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3llwhpivh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qifdhzci.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yfnwioan.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3blkzzwev.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qegejvpx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yojvoeju.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3juaepehm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3diedwsse.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dsvbcpei.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cjqoosut.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eifqzezt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ffyvefon.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lfvrbwib.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vxfieunz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3agbdlwyf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vdcfhdew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yonvnfrh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nkczcalf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kawcicsz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dpdiosnw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3phrprfkg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fadtagqf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vrzxtrmt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3oqgoasqq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vpajmojp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vgsncfpj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3brlimzgf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rbjsdsvr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zuvcyjkd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xtqdbikn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bekgtznk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fqxcnfjs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ovgbqdsg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qnbgtbni.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3isbubzjk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lfehcfnu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zjpuxbzt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aaktsihl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zfaerlwv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3madwnvoi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eufethmj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nfddmkhv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hhumroso.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3soukkwju.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwyufrk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gklchzzj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqelfyfz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vkzkxoxl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nrushgnn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bdwnovow.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeeswknw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pkgoqkzy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ehqtbxll.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlonbxkm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dsobztoz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fesmufmy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zknnzkny.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zzxbbklg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3szovwuzn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dxionrip.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vdxkwmsv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3egclcljf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufzooice.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvskmcq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3avksogwv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cyvuzchp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbknwdtp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hzszenzg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3yagnizfd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mdufjako.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypuzcnco.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tdugcjhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cddihkcn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kgakwgph.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3awytvtuj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xfakkytn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nnfnxivg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lptzerdj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ukndjkjx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zvblwjcu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zyanlowm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njawazgy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dbuylanm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ucnfgvpb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qbowujzj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3djbbrrek.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xbdhbyfr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mzvhskvs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vjnrlvwv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3iwgseewc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzlsijb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyfpsueo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dgcakrdy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxxgtfv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jtatlwil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3czcjwwxf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yquvigvb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3afwpnhaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gehvkduo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3waserbng.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrehbtf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3putwtdor.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wrrbvvio.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kisgjjtp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dfwaqnwo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ydogzgsm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3beplmrco.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pfrmcqao.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irkjpwsb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ixgbqtiu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqmyocit.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3daphjmwq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zycqnfzt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veavxtpr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ftoxzlhv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3oaznyuhg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rbolkmpf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wqxqaowm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3shomckdk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qehvfobt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3blxatpyf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3einiigbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ivogwdlr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jtfxqnnt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ypqnbyyx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hryniryu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cvevmejf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3imwvdemr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wmckihbz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bbptaaai.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3madsfgrr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eulwdynp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exxysgue.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mortusxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlzkaysy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sezmqivc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kmroznnm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3awcmpevv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mjfagfvz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nzckcacn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xboijnqa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gbmptaqf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuqyeapr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqvargtr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dqarbxzx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ycchaapf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3swssfpwa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kkbbzvsw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqsoajpl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gckceagp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtzsgny.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qruttjbg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lctjljmo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jqwzuqds.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xnbgqzeg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yazmubsi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3khxtjczk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cktplrth.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nwfppamm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qxcwccie.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3axzteegf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rcahrlpq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3oruhtnar.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfkkemmn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bnnoogxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uwdkwybi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vrhhdtvj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ohbdrvkx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3woqxoqih.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3btdvruhr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zrsvflts.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3waocyesw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qifmgipa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kapfitdp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yiutjcla.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wguauouq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3miwwektv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cmpldlmg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgszalhk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anhzkudn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wptnncic.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrzdtzwc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dpsgdlvk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tusbtshl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skzfrgxl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wzuophbu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifnjrbob.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jaqispol.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hlnrqbdz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qmaggjjk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rqdhzljy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kktdrvda.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kuihluiu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wxvcvhrh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3keespgtv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3twchybyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3miavrmoh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wkwwxblf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mjkcnxtp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxucaga.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fqeqhspz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wcwvqyvk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wdwyjkpa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3msgxjerx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tjavxowm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqsqvcvj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hmmulhsw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fukyljoj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egbsrgik.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbpgbzwb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hxlahuzg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3euqfgwyw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gtjnkubp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jeeqgbda.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oanbibcc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3usahrrmj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uzpwekjo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfinqxav.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzftigjt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiwsocjb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pryhwkac.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ezqwbqde.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ervlfcrm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mdgldkvb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqqtneue.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpefnsgj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3extgfhvq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dqabutwx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjpejfry.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvyxjjyq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pzjtukap.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3stjlkjaz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnvfsnqx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mifbduow.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3znesieij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3swagivfh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vjodasuq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pgoeprpk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lvafinsw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tdvxeopf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3glfqngwb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hwrlrqzq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qdqvfrru.html


<!-- 参考信息 -->