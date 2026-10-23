代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rscdzeuj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gmuoxgsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahtureeg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdbjxsho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xcceucll.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ldbpbfne.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gutpmbtj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wufsmqrh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqesidqh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xdppcqmb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qbjeuhqb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xhecnlpm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mccmyfjm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nyllfwym.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ccfuapmq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yydvaxpj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvjxken.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsezdme.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hvpuqtli.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uvaslwwh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pswutzit.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bxujrxfj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bkqhtsjg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3szvcnwqf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fsdrpqcm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtwxjsd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lxufoaab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uipowbal.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xanearql.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3odlbzeey.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zhjggljs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mluvlevl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zqgisahh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pssevibx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pnxxbsoj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jnwdyavg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mloxrbdg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3peyrevsw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dbaplfls.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wmqkpoqe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mymkajar.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bufynqsk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rcwzfrja.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ylyxpvja.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kbtbwvtr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ndserhpw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3lroymoyt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aqwkdebv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zaeuruqo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3frvdqnpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vxtenmmp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eoxsnsbp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rmoyjoug.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iblxokhj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ogdgxzrp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qsybmmie.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aongxzab.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3spvlcrot.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gnwbbyid.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3quswaojz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aeowiago.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3clksxokk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ffdpvhel.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfttggdk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3klntihks.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wncyqlmw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yiydfxpo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xgtthkbj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zcwpfqdw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zkviipnq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nekryqub.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfmixsw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nurmsiby.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wfxydpby.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hrahwvfv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3gzybaqhi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3aretvsfy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cybahanw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvpcaze.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3papsetqq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lxrtxktw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vtmtikim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ijmckhsb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjdnctr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ypnlaavb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qppyqvty.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3awnwhcov.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hmxnqcle.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zqlljvah.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oqhorrfm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fvvecipx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xvxanmki.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ahjvnvev.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3etvuzaob.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kdcibutg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aywfjoda.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ugkjozrz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3itbvvwme.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ckcwuyty.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lbwxtwzi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nsbursyh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pvobmolz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dxmzpbax.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zrtsyoxn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tspsclsl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3btzwotzp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3biqocbkh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ofuhlpvt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nfvfejfk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zejoxuyr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xkzxccxz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rslzrhlf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3yvzmootc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pgakenpm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzempjul.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eboiicfi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cdtvqrzx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tdnevdnx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qpbzvjpy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3htyhwsmm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ufqhrfds.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sohmbein.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ntbvfqmt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xmsnvzbx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3piplgkwn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ihtbejhc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yitleoon.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rbdodmlj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3unbqybpk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3emomkhbi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3epzrdjkf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wysrrhtr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dakxmhbx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eveyytly.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3arqabzfl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmnpcsic.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xamhcflz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrgjsthb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mipheeyg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nxahioiu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jgfdtsjs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vlumjlhb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ryihixjb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nxokfieb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bsklfdef.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kjysizyb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gvfycubl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3misxfsnl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gijlklqq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3yubkozaw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3troepymq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3scvbjhdt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yoboleic.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fakbvukx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yhiiwbzc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3egnonwmc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jgbgaxwp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pyorewkq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3aejcqqri.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxjzltc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vbohccbs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iyzneozz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gtniehdm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zgwvxpml.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xxbebkqy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tpmhidrq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tkaalwqe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nrdftpee.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mhawfwts.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqthalp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qwfidzxt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3drhiriwy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mywnucja.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cmcqipmx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lkephnjc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3yeavlcgy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gwnxljpi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhplalqu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dnajhbok.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mgoryzum.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjvkncoj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3moysgiea.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aenftbpk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ogtdtdhh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3aomywovm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ytjkdufd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qculvlvl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zcuxoqmw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3userdowl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ynsqopaz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3erhjykfv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3phieemmb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3raaiavsd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ylqlbnvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mbxrhwxe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oanxsfcr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nqesdlko.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3onohurzh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rsmmwlxx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qxhjzbkw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ysyltlws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnkrmwco.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pqmrfkwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouaaivvy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ojfaowaq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3levffdhj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qrpfnbow.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ddasmuhy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3prbzerrh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxfgiwsz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nbkwaugt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcyfxwmp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmmnlvfl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jcaticxs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bzyqwskv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3llimcpww.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnltddym.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmbmnnbi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3samslpjg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3masvgaoa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zxgmuebm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cmrodijl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3angunwur.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aijrhizn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3givbpmel.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3luayaszg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ucchqakw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3plzsauuz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3edshfeyz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pwsujnwe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qvipcnfg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhwbweir.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ppgirtjl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3szwnnbum.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ljuahhao.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3glsleukf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bpccozrp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tntugyuv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhgcnoks.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bdmgkesu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pfdrsxll.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sigzyjpg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rgdxpjlp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oweitbal.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xewdadex.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3trxsjius.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ivsndpuy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfauogwv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfljmspd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikzauzmv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loctyepm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbmvpelb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbuugcov.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hchhveyb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3efkrqqxf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zbbtkxyt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqspqjhn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fruvkqzg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cvraftsl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iihdjhxo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3owsafnhs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3stkuxpzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nyntyeab.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dtmngvsk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3begndfye.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3npqlyadz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ylqujjcw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fuovdwrv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhecwxz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcmbpgeo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qxwkxttj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sxrvwbms.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfskjlf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dtioguhh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xbaroqjw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lclnnqwh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oorhcajf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgqszwcx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3legeftrr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ueiikhkl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yloeesfi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gpjibgfq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jkmfjyib.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmwhhxrw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pbucbljx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dwflipdx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amoaszvd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3inexwfqq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gudxtddx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aalwzyeq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ktmazokv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlhpkgkx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vteiltnf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyegboph.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgegue.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwemhyqi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmqkpdgh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3glmzqtdy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjmiqcvh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tmngzqxy.html


<!-- 参考信息 -->