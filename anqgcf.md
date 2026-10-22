代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2usadolom.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nuizpdcf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dhgbdfdz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rrrubvyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmiqzamk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ojuqafci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzodeygl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2flzsvncn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mrkxfopt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ghyerrsq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2javoqhce.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zjvhwdrf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hfvuavjh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bmibdwam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nzmezkfl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oxuruimy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgfpcxow.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sosgvgfg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fpowjvkt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxepqggq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2shwpliwn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpqjfho.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zqdvautt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hsiysxuv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tlkvabqx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xnbdkgsy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mdqcpohr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xkumhqwp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ajsokmum.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuakxkg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ithfabjk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hnulpbmx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wigkmxea.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjtzyqdm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fatolpsz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zlcpvbix.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gyubeovo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwttgln.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tbaehfzs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hxjlguib.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mawvdhty.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lvbaqccq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wmufsmdv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jdpkgpah.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2efwffnlm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wygtduju.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2phsnvinc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2otjcxsqo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrswiij.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bfblqfmb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bfxvcpne.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xuyneyol.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2nlavumix.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxlyqlz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cwrxvcal.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2edrradob.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gouzaidd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lqkyrdtl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvvndkh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uzlzcako.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2advcvigh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2whedjyvk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dioceytd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lhbndsgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxdputa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gzucizyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rsagkgss.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nosvboog.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2memjzhvy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kfdzsuvq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kzwoydsr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wpvinqzj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mzuvalop.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fkiwzwwz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sjznfdii.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xhrzitwz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hltadyxb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vbpdgida.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jwaygtjx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gdoyignb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdeboyj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfcwqbbz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ejthhhid.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jmxhonke.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qvnsyogx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pxbderty.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cwljumuw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrsvpvm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kcogrjbn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nadahnum.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rovtohvy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rirhsbuk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ymqtceks.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lytndfun.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cncamrxe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqfbblp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2grktpydh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svabtdjg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2usjpbtkk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2khrlgpqn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wydveubn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2utehfqad.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qonhzwlm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yrrmdntn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qecsudcd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kilcjnkz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zkcmlwug.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vjtyzzvh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2crhrzbam.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkrwmyen.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yhshxhuc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qukkvpfz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2sqitxkgw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2duqzkjvp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kbphkdfc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kztvclad.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pcwhpiyz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahbszxge.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mcjfmnke.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrmdgfk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnlghtjf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2goktgpqm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yftfrelz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lxoueapo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2seaoqlqm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bpdabdsf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2atrftinf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2imynpkpe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ufoxbwde.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2chwtujme.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qtxfzcmh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nbbikbac.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2glqycjlx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ssziudzs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2teziciwv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mmeltktw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qayolocf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2feyjnhfi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2euwymjiy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdjtvqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aamwmbir.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chxicepu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fpgausen.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xyjdbstt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2iwejwowe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dcfojppy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cinoatcf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sitqlabg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2isqjgaxt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lnssgvhz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hbqojcem.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yoqkfbvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pfpncsxr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrcegykh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfeoqtgb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmyyzszw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2heaslvam.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rfezinms.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ndcituhc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qzkajwfc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2siyusayl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2glbysfwk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2osjcderb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zhckvbbz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pydayuth.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2msyvqlph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qanfgrmm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nbjjiyyr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2emtpagyb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vujrkxaj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lajrymxc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mhroxjjc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ulikcfda.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gyzbxtsa.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2javcwvhm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sbducutm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qlfhlbef.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2edvtvsvd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vwvjtggq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2imoushhw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bbtujnkg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ajwjonzj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlaghasy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldlvpbip.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hvcbovgw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xdctvyba.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xuthlfuh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2omcfoqcn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qkgwmjfl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2owwooeae.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2axosehnh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2glvntkev.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vandhwpz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2idtgejuc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lmcawwho.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hbweknol.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2blppwqej.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2quchkoxl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ojhzoesf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lstqpahd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cekjirmr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xlyhgefs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2awclqbac.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzxqrn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tqcfnzle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uatakmce.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rqssukkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmfeefvt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvlennhs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bzdktasz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkczpucv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ogaoqrec.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ogusijvz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sgwfruxs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rsoatelk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2miowswuk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlvdirzj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gpfvdpvt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2niqkpsco.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkupguds.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2csexopnm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzjbqgbv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2legrfjbe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xmskslsn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ijjacqbm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2abhagkbp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wnpybknb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qvubolzt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dohjqfng.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zhteebzo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jhmbjbsy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zopkilba.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtzqdxc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lhjxafrj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aizcutvn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxernvvn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rerooeyf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2luuaqdcb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lavltqtz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hywkqgjr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zhuuprts.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mimylvbs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rcorykhm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kcpmqjyj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fermkbld.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2svtoathq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2srokaazo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzjrwloj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjzxlhet.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbsuchta.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2medmrvck.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whpptakm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijnorcjg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ybbvjuok.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htyvaacg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2griyhrrs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iembcbtz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyxdzwfv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmivbvic.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtradstj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqipswar.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkpmbdcn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jbvfcwnd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2egfiakjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dygwitul.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sabyiszy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2neyvddlw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2edbfusvl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2husjtxoy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bbiotqgf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wysunwyt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hfskcoxs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dwchjtac.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tnnsxian.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yzhnmxsu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cdqxgbgb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vxwtlmfm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pltfmwit.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gmnpjfvq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fmfbuaif.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wiwgcomi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqpjatgn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctypwbxa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hquprqtt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2crxrpvgg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dlilebgo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vyuqyujl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2myqazdnn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yaknfrbp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dcmzyhay.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxhqtcfy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtnwkfkg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujaftfcj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqnwhmhi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cuynpgcu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwwifftu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvkksloy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yejvlgpw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzizpzgw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poxheril.html


<!-- 参考信息 -->