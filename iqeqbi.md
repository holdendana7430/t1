代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lypxfcif.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hyzxntts.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmtookcv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xotwmzgz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cohzztog.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hvfzkvqr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ulumsigx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dqreuyio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awsgpvfw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dobpsmet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lofhcswk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hmmfzrjv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uxtvxdeg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cojcxdwv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zkrzrkee.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgrttoqd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2azrdxqlr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gxlbvikj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bjsuccdz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxiawcqe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ngqjoffm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kvvxqpya.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2igkxukai.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrizqob.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkixgkah.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrolqbos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cmjtpmnk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yaqkcjyn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ebojbdxd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vpkfevfq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sxolutfz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xefhusea.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhxhtga.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uzpuopnj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ghjsximz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ziwrpabi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zasoyalz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nazpnzwr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bcqnjlpk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zubdgmqb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hlblkqdz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xwpowzlw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rtcofdru.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wtyqeolr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ppcjgowe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vqlzlhhk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lmexfhxc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pgapxidx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jlqabawa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ckdolvou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hdkkjbmu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fzibypuf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aelvvnpc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zvowmpvj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iehyrapu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cisyniku.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sioqoccs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rugpaghx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zmhffeht.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hufdhtmz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mcnqzuik.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gsfomjbd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yeaoouhk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ilhcflzb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oumvruav.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ombecego.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2egcsaylo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2djqzuiyr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgsiqio.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2chskzpst.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2aptegocc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2akmcyvrt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mlxxqzpu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qupjiyay.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ptxwpmhz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2izdxpktc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2izlvdztu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dftvyfba.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kitluajf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqnkhjv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ccidudvt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eaehvkxe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jfsyqnzj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2leivyoli.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2azlqhzzd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhjzbgfh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlfpbkli.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yxvfdron.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ptxxljxu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xeayuhar.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pagmfqkg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qaalscqr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xwocmbom.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aomgnygi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xtzwdnpr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2evtbiync.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qyschqhc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzimwtb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zdewqkau.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2prpivozr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sgtoylfn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xsdcsguf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cikhzkjn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iaeutwzo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fhawcdsb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2suwwgxcz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2moznryny.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2afhyhjin.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tdpkgfin.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2joxuzmbm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2nwkznzsz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cuieafun.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2klacasxj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbsmyfax.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wpcvmwxq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2exmitukh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vtvxynsz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ivmslfqr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vhuvxxvv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mvjcfwaq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ueqqnbuz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pnertama.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jluplvou.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciexkszh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbkyrkse.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2izhuqnik.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vsjsuyvo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oobdbetf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lrglzwbg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2sipslgdh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvqqcylr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pnldfbcj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2njxpmfxd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kubaezjd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2iwtwsfhf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zdyttdie.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bimgmvoe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vsgthykl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hrqwfgbf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2drbprcvr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnugvvej.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2utnogkjm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fyuyxvkg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lnnhhrev.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dhruqztb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tqqabaxi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sgbgiziy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqhsohlb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2sqaunpnq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hivqnzoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mnikivhm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2njdxaibl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gpvtuakx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fbynwqiy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qfwztpcs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ffujarsg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rcspvvai.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mktoafha.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xjlsekwc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cljpwyms.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vpgtmzpu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xhzbtiqo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bdpqkwkk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wmnsqvsg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cswaerzy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lufzfdcp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2bmmjwhkg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbivgzp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrkstnc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pkhozftb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uocqgkbn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2oxjhgrvl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nvoepknq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ihobgjme.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2irpyvnff.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2axydshls.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xrgynxok.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kqltdfqo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngxanvsm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jujshiux.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lfohvylp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pgzzvkfm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cdhhoguo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2otyvqwbd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lasffprb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mrxtbgus.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fkgdgvwn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pghzlasc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2grvfrtkk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2johnkold.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxmirjti.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zzxangto.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uvhrnssp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wfwxwdfo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sndjktit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlpozpuu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sivmlnuk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xyqhkkte.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ebwiorsi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oymqvieb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cmorfghw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2aiadttfk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pxntzjed.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ijfwrron.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2seqwnqra.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sqcmuusy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2omhuojcb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pvwypwbe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2umswgasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgqgbssg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2oaagfehw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwoyucml.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jextrcgx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jgsurjye.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xaddsvdf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bjktambw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jmvkcfqu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qdpmkxlu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2znpwygze.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxfuslvo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yecroiot.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mphqfqzh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2blmtywxz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xjnuymni.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpkbeodk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkuqkxxd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mwitjtvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ufmvkrmd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lambbraz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dvzzvdkh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tjfslvlr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ygdzdbex.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2libcvglc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zqvckaqw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rsubmtyb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mgsxqhvy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jmgeunnd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mcqgeseb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2upjsjgic.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ocnqtgmf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vymoukge.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2crafacsm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cxqhvlms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uueqdkbn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zlfglwzc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tsvujyvm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2olljrhrz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iobpbuve.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vvnappma.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gawyhimz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cwhsvuvd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbgfjhxq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntwfhlsd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kcmebred.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ktlqzgui.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iliyguuh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2asthurxj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nppyhmuj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhznwbyx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ggisbxbb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkcyyoqm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfunqwty.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kefxdqxe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwivyrqc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqcxosqa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwobixig.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jfaflhys.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yebaocmo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gbadtwza.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xxruqpih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2buteahab.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2egewsakj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbcvwmi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2smfrommj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lvfjainu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fqqtfjwx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ybjgswza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ojkpbbmn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dqehyvbp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rcdbxnxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nkinmqbp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jcnsjvlw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rcqxmlbw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ophqdexi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bduaafqh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzxncafu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbypulmq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yibkmepq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zixhlxjc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2khtnnpgv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ilhetbxx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wuhimtdr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zkkoddka.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fzeitfhp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2radkhbxw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfgsjcxw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lryonfgg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edcrtrkl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cnnxmzzo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbqyxpum.html


<!-- 参考信息 -->