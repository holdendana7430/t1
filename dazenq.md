代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uabdcuxp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxnpfrsp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dtnrpkvl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rksbiqpx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jehmpiyo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cudecfwr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ywumpvle.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tpmcaako.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocnkyqgc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qvwmwwzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpymzcmy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3slhaghln.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3oycxmdnd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3copxppur.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ggilszag.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qooleqvz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hcxzfbjm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ygbdrsux.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qxnlqvwi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rgkovaiy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jrlmzgfb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iminbdse.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpqabtzv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3plltupee.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqapjisr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wsibwwji.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbrvoiiz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ymwgckxs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rilymrvi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3prynxosg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dwcsyacw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nhrhfpry.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3onjgijqg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iudmlxdw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3roudgmos.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bcgbipwg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yfhwxdfx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mrpflsmz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rijlnjvh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iycrqvvs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qukizrgv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3knigqrkc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3psngttwz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zkvkjqff.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wgyvxssx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lagburli.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3njromiwm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lxcpxsgx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gpiayrfi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wlqrrnlb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3suytmctc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fmjjshli.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lbyhdizt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ssykwrnp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kqdtpbms.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3boimctax.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bydpcnev.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgtsbllv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ozgitftw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kqmjqchj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gtwhkqmj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3krzzoqqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ccdnngwp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fazxirwy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eaqxbkyx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gwultfnu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3owzmmfib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xpjppfnb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lkyrdqep.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gxibrskx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3siutfkls.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwnkksv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kundtmnp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nkptkqjs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3emlvgezw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pxcxxabp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bkbzkxha.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yrybhwal.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3imwltnzg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mnxotoqc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3appyentg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bexqtjhr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pgxnyneh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lkaxoeai.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3plbjcatw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3onxcpmxn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dvtybpbu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3htixkrww.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3shciepzu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ztkfbrcw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jvmsuzka.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mceotowt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3bfksowmr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vsfmidjh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3smwyrker.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nslipvnw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mcytouxm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dbuhmroy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ujfcpapr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3foydhfel.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xdzjifqt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xskvjuem.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aitaciuu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqsfjcum.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mqhezplf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mzthilhc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xyaqmnpe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nsvnlgpb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ehskdykk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gxdiflfm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3huggaoqx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mctwxgux.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xwnbaylo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nuhgixgt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iywyqoep.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mmjvtzwu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ozjhhqva.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mwcztytb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qiyvffkn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yzbvriug.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pwuqgwbw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3alngizwm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndwjpvuj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lbkgmiuk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbleybrs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xzjcmonn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjmoyok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ksxokvrk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hvwnjkzk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wrxojxqy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tejoaiwr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3efdndxsy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfnpabbx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ogzhxplu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jauljrkx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zgnnwprx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mfuxyeum.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vcvepekg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3azssbrfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3senjqgtj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drnhaock.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gadlcwfo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xdpdapbe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iovwblxk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntzkmeho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aohcamca.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ujrmqveq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3baflbeei.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gejhiifj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pyzuxebl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwuwlft.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rtijgfin.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mixrgzqm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lyvgacep.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ujfopgvg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fzenrclq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uukokcbf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kblcoazm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sbqxergu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fgujxxym.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvwbmym.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3stzzewhe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hkmhiwtq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wqtornqa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ynrtfzor.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3neakkqsb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dyhtgqrt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvmaasua.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3enbjtwvu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lfygicbw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vvaqwykg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzpcbfkd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcvodzup.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yvvryuoa.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tytjffbm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jytpwlbc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlltsbv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3awgilrqa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3txokukeo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yjjpsinq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qrovxbfj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3cxxsqoen.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hxpcnsod.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wkncagam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3onpojrht.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3naujznli.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftkghtmh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ztrccivn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxavoqca.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rdxyasia.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rspgdctf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3soexulcd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tdnfqebn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xclodyii.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qjhjlonh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pvgulema.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jlbhqbpj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rzgtqppa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dapgcsjk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aosnzovw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3keknzbzt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cwpauobi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zgdhfvsd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mftsturw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3doqvahgv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vprvsoag.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wugbpzri.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xreebkfh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bdagcxfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmeusmwh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zvyybwvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfojspuw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wcqtxjfr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kqrzqfgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kowsdvdb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zggrexzg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wivpsbrl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3scehgokp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ercnfklm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgzfuimu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfexeklq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3suquyllc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3atciaxqu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvqbbxe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sfrggljh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzexbyhr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjlweht.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tbrnocho.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gkbjidyd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mhnpoyhv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rciuczzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vajsiqns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mlhjuhyj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3prfyhqfk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3llaowetn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ajqydnzi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lrxsjxkm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lkboaipt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3muffiips.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3acodrbqv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jbmkbhiq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gkoqhuzz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3czzoyxha.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pteopbwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3atvpnmed.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dywddavi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kiqkeluf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3onxbsgmd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zttqheeg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xrpfigvm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3skzdbowt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ierynper.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ioapdhnu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mqaaveua.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3orqoptiq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iajkvgku.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrppzyxv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vcgnggiy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isiubdqn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfrffmrn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pusnxyoe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3saiizxmv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gdqjlhec.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3anjwttpk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykkhlrpp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3trpdmlik.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qaioexxd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uodclpgp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xeckbbrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fhhwkfbl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kalqidmu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xybirnkt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jbsepvds.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mqegeyvy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hfvrjeqp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rayllzal.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjdmaac.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdtkcsye.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yzwzyhrx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cmhzhbbf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lmpeucew.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qnegqcrx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pkzstslk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbgkgbpa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dgkdnisy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iuvkjijy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pdyhplac.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qjdxxkgj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xuxewbqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qvxjwcza.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uumxybqn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cevavfuc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cjrpymoo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dcqwulbn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrdcmmtm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hmgchsci.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hweqiwnw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uykhgwlg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3scaeject.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cczwwcyk.html


<!-- 参考信息 -->