代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzxxohvo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tpsdxswo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rpdinrgb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2esadogcx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2skxqwunz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2faqqmqsa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebfwhsms.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jvqnafky.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ygotdrxe.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cupipdnx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wlihlfus.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2alkirnye.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wuekvffb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwuutoij.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2welibmpj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yuiifabs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mgszwdpc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yivpicfh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bmfmoknn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rzphmfpz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2myqiudkk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vnrljydx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aennhysv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wvnpjhfy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ewaovvgn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qesfqyoa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dsfxidky.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ucotajkb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mxqsnkit.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wodrggtu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gqqgbkwd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kaowdejh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nfkcvlrl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ivbqqmzm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tfjthurz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2abpbcoji.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gyobncyp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbqroquo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mjbanmcz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enryvehw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2caeispjo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kovtfccy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2amtkkuyj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2feumzxln.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dbbgeumy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vyiqrzfb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ulbeolyp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tmksclnd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2silicwgv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ibguumwh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwexhgj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lhnhpumq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xsqjcupd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dfbxawfc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dapzyand.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dymouiuh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kzkdeijv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qrrgiptn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gtxyzuqu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qkgzdfmp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jpyprmmo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pjsmzdxg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vxuufkng.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uboauszw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2birnfkqy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qvmbrqpw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aibyuwub.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vmzvfpms.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ornfxfpa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2itkacsec.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cypgwfik.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bxmgxgoc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gjticdcx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ugjzmsar.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2oibyxjjf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mpvyphpe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2auogcoua.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yeldpkxo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgnbzld.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lccmyqde.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2izamnwsw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dkooeunm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2frvivtvs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pucpfwrr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cpcmulut.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovanmxuu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2msufwbfm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2krampgts.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qludnhcy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2deffmdif.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rvufqomb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2caktazzn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ticsflvj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2skdmxiub.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qtpdtfcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jfixghlp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2cfgvsezj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nllyhcyg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2myxvizeg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aaqlnqpa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ixfcblyo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpydtuxd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2igbkrrgs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeewrbai.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuevqpbb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ryvlgijd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2snrtzdtk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xhpmkoth.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jifyveze.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2sfkqspgu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qrbwaocv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vqsmqzbo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2firdnnzf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xetxfwbj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cozdngob.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bwzsayvc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgimooo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mpmorhcs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iszacibb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2owkivxcu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hijyukhk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mlixbyuo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2anjwkjzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsftqgiw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dgcyeidp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dlvlcdms.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dyfxkhkq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bufgtebj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2obzanzkt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2exillifu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2skegohji.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oklhnjnh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ejwoheqs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nqbgqnaz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2azqxuxcy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dayradgc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xgpjnbrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2plhgzunh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kbdnjcrk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zevdueuh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhadltdi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2upusehlf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xiouwrcc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cyqnphtn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2omzivnjn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xwyyhokp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2csckmzns.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxsoclh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2unxgvmsb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2evgbmjra.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nrvtdlzn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dnfcwhqg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlmnjqpx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cgcnryft.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nqrwuedz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iyexfwfn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqmwlgfr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zxlicotf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mxbajqer.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pwpeajag.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2srmgowwp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jmikucpc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2solojjbm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ylfnywqu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xqgisfgb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xfxlwjjc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2chbjbmqm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfltqbke.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vahildbd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vauzfgae.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gehyjien.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eakqvlba.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2japkkqkj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2spntlyvq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aydbcgrd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rntknplm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hcnsxvsw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pwweyerd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jezjpcfy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2evdmufwr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lwascexd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbffsttn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yruwmzfa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcxbsqyo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pkbaiwjr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cvjxfavf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2brkawpqz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lktmttvh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2urykytqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjoxvere.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rirtciyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvdgqpdp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2eqfnpisy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dfcbqkxq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cmtesjht.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2uwpsfawl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aeamjitf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2btancnmy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jxaqmtjt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxhghiar.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rcvyailx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lypeopjb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2huwnyijl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzeasjb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mmgypxbz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yheakcbo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kenxapao.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fimnhsbz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jgvzzuzs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqubmduc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jvizwxky.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cmuyeuqa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xeydmzpi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uoffacio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dtiehgkn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yzhtpxgb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2izkuijjy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lapmsvun.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fmxlrtms.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2seieupez.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lcvweggf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ohmngnpv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rdbgjcyk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vbympbtw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wuvqqjof.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jbpspyhm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wzroehqr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pzbxdsog.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gbktmhdd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jjnktbhd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fclcxscs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tugiyxmq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgebpstj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cyapsbuz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hsavqibp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbpwzzue.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjffuuq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuybxdnx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqnwdptw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nywwzdyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bctpmqoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpnttcea.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ztxluaao.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbnyemdb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrrpevev.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2molwxoof.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2dafpgley.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uiccjgok.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yrckcxfr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dcexzjdo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uavjjlso.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gomhmhpf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bidkgwyk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wftwvfng.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cdtysddq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hyymkhlk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kzgyzvyk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2exksglyl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tidcdvvo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbuctrlw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vtrseyax.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jbufnjio.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ppomyzus.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bepvplpe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qqpoxwba.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owmelpkc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urtpxkoi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uewplqvs.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nrrzmbkh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uxbhabbn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tymzzsov.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkjudkqy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2iqjtcqbq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zfcxteie.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uptlyxhp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gimjzhkh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqcsrmjb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcattynk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2obtknitn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlgedntj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uotdasbe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqmaohrs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjchyhrf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kioddsau.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uuzcjcun.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2egilbprz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsjcveaq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2itircrst.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vrkpqnzh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ziilwfdb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fumvsime.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ucehwvzo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xinanquu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jwsszyyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hxgehlfs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cuoulalf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vfyavbof.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jnfyvtbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uysmzvdm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ezhxlybe.html


<!-- 参考信息 -->