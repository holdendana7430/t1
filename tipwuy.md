代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jnmikqyr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eibkddzz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvaaeepk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynixahvt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nfbewgvr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpvmxwie.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kegxledr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dwbarddk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zbwsgaux.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vezgqrug.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ewrcizct.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kbzhduvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pugqhzlb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2npytkfbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqdmlfoc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pbcbibpu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lsfonoyl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dfcoyafb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mohttnik.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dyatzadq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vglywrxy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ipmkrhxe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nkavjsvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yutkwnwn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxcwgkyg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2isgbwrje.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kcmzgnvb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vbwprynp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xnlbchrs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sxtmghlv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bitczuvm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2migltfzl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ndnkxlgr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lrabmplt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2iracypnb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ptaaepnp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bmonrbra.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gdlytihj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gqvreqql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vithygee.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qkkrbqoy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ezmjgalm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2adixzatg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vpmoqwgx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lomredfk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2buzyziud.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xfngfewo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uitzlobf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bbpsgetc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cgmthpxx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dmxtdcdt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rrrgxnyk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lcdqhjng.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2haaaksbv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2upnqlgbv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ewqulwlo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2biihxqwp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ecpclmry.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vhlwqcpu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eqlrmizh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hlglplmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dzzaxzra.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dyksulqe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fbcoqqzi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nwqkeyjd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2urpkbswr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jeorrwix.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jqpdnvsp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qtgokpqy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ojrmltmp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uastwszj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksjmxdfh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nszerjmu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hcswqlmr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ipayefbh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2erffenyo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iaxtecoq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2szweofyh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pqagfjme.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2litnnzgt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2uokbvjrr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2saftjaep.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2stonpvud.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ujsccttz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mbwpsxds.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2brrjzbwu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jphhzmph.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dujiztpj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gfsfxhdq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjxrrrui.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhqhfhl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxrtulw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzevsxbn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wwecezik.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2addqkums.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sxlccrmu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2umqremmo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pzjixrmi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jpqidxrd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bxnuvyep.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yzhckuiv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tishbcqp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ofeolfte.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fhumjdhj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ctzjcjan.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjhkjqmm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xovzabks.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rtpegtfh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xtvcwuxm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bwjyjlvi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bvktjdou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bzqdegze.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pcttcqgu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mrywjlyl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ojmcmzof.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vyjzhfyn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2slpgasqr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wzfpujly.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ixlbfbaq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cbvkqstt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bmqgxcdj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nezixuuu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bepfavfs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tefwhgcb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2seoqvxng.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvxnuwdw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxrbjaed.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2psbmlagn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ehqfchfp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2prbnnknc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sinmjwii.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2udfptqur.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tluismre.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xsgqgxdo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cthnqgac.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xbgzirir.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ealjunhd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hrlbzgmj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rnoenqlj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wzedqsxz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tljucjni.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nihcfdum.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhnyjxvs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhafbpic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njrmvoon.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2idlnzipd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2amuqsdrv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhiulafz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rswninad.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qugubpmi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kxfdbcep.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fvdauwuw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yifasutt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jeyhvsqo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pdlsicpm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2klpdiqrl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2sheywnbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jrikawfy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ktclunpy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rpgeztbl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2usxfgvpq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xbqfduyt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izkiouvr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcqwzc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aleakjfj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rvwrksco.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xfkmqtfj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rflxteat.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2prbfebfc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pwbgraes.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jwlrfaeb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zsotrosq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ydepuksb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oklrlyct.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cmfeezqm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2amcnvlnu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wjjutrmv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vzzwywpx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qamapdoc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rfywqsjt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nepjixml.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxpplwc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uiabffkb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bspyjjnu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jaqzdhvb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hhplilay.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2altdpeen.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wycinrfn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hequfjmg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dslnoqof.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fbmjfoqv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhsauzri.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2klljinxn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2twqhypgh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kcifkwxt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qmxtomdo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rxymwnwo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2adtjfxpn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pepnqtlf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cgvganzn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ruepaanj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xztojlnj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgeqzvxp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xnteocqf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gaywxaka.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jfjxuqhu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yanfhwmt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ikccmthv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iggrtjbb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bassqzjr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ueqdbnky.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hwmpsieb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jzwxspdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2befuzoks.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2drfngnqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmmvkipb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2wzebpkhz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hzrbtzog.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gyzjyubo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vvrspzia.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tsqwumgr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzwafezo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2usqcbynl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ildwczop.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2knzxcxez.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qkulacjm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rcaffwer.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnebcjzm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdadbidl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2crfeprre.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zbkyyupj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkvnipf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xjzpigni.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rchueyth.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hibhvvyh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cbcnpoqn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sedxmxns.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jlzeyprm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgabswf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2grepihky.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyudrcy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hahbmmfe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vviimdha.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzeecpns.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bhakaevc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jusynqyy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ifztiedm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2anjwqtkf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nwgyqddv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gzqgdoio.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bxvawyhe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ozzyalje.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qhzphywi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qkiraawt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fziehoum.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxtajtyo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijlcwfbz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2enrkrsjl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mixubsab.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdfwfyjo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jozzcdjw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqgcylej.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vktmzeem.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kagowmnp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqrpmqgi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qobxbirq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aenfvpxg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htycktgq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zebcshcs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhokmdpz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rplcmuge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qwbrnzgu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ufgyviox.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zzuiofzu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2plvwswwj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbjfiqib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ewfhjogo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2valvcyvt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lxfhhtqw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwagllkj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lehxeeir.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wexggaej.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lwbovelr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gownkmii.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kyylnhtn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tzcefdwk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rpbwgckj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qlyxyrwi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gcubzclt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtgvoybn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yvnvlfht.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2itaffdkn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iwycyiuh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pqqxvnks.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ityxogmh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nleflwbr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2frnpcqbp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kbzjascq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbqbldyb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owfcwpnp.html


<!-- 参考信息 -->