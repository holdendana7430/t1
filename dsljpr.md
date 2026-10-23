代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dszgzkiv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cofcwnaf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tjgkwqmx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vmvpzzrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxxoxqei.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dnbwuqfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atadrryk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bpohsozb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wxnpbirj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nvzqnmrf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ycrvmckl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xpmzykqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3psfquscq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vhpzvtfm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yfgyjhvi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3amemexqw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nsqaxkff.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tqopxonk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3odsllxcf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrtfisu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xmeveutb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sctktrgd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3azseaoth.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3halpaejv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tccyvvnu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jbxwqrpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rptwojdy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tdebzjvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vykmjpno.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yzoepacw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddxmbxxi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ywdwogvr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tznrmase.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3oeeutypv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jrfaimnj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fofzchhj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xlssontd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fdkiuhur.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xnzhprjw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nnmitihv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyhuiulp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rchyuezm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pdrrtwcz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3regzqpur.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xivhnnfc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3leodekqc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kbsqftoc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bucqawfc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hmpuwmfv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zllncyqm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ooldmzer.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nqgmlors.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3igbzanky.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzysmhts.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wrogihfq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nplcwytw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gybcbzsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tnvbalcj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlboafkg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ccygsfmk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xaehelqf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aypsmqcd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gsujaoqq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvehylms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sohxegfs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3syemcdqy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ljxmhmet.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3erlrthmv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gybigyyo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ktluqeml.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ekuvfxzt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wdragtlq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gkhnllgj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uhmijnqt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sfzpsqjb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ujssldqf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3aclpjbtn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vdlaokuj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfmtqgu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hrlundik.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3brxmodsd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xagbxcmx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hhnsdfyw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3btfecvfj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3impmqzhu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wcbfzpaf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3clnqdxut.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dobnxyye.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3grooxnpq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bxlrxrsi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ekhmvswc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mfvmmyuk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pjfgsqxo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rnigffuj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dtuttdql.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ezewbvsc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qkelaauv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xienjsgu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lfbbgqcg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xajfinka.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oodnaozr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hagggnjj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fjrotjhv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3deunuwcu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xkyqmkhq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sbsfxtnp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ueqwlzsu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xmritwls.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mcseeqtj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lixtzgro.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3owawpweu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mfpailga.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qxvzssec.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xwnqtlvv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3obmbpats.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jcfiwjtx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fjjzdxdr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pkxechay.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzktvpil.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yasuirep.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kpjztdto.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ykekskqw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wbowlcdb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jhevnrqg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3agjrqmjb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qxdfvfbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jpknvpqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zzhgtzcy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bifzyvts.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xgumayzg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3uubgjied.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zmdexyld.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kkrahjwo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gvjciysx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mvawhggy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ynhpfsdx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jfvmmxal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rjgybsyk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3aojmmcwj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsvwufcb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3renpfpdh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wprtlbqw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qijbmgzz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kpqtgyre.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bhufcuhk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xknxzlhu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3krtxivla.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jaynxdmx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3macyfaqp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3htqaquti.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zjuyynbt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3doixvaaa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yzodtkac.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxffsqma.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hnhgadxy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fltazbam.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsiziwpp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lllfazww.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sdfkbybn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3iussxuni.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3watxhbzb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmeypbs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fyrfapaf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3onlrbeai.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dhkyneap.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fqchbwxw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkdqrk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtsptpnf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcwgiyni.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ebtjqzna.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wpohyiwr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtxgcfne.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xliqxooi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aoolshaz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ziybvikb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ojtroxol.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mwvifytf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3icerfwcr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wthpfpjt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3egjwuvlh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hzvtkihx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afzywtyc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3czbybctm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ewycurkz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nlqkuulc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wskwthtd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xpsxkzbm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3svftqlrm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3shhtxbyc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fxmorzge.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uvrihljt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3waupdpik.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qflmwbwg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hufdykrp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zagnkccg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3elixwnel.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3velovviv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zeezkugl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rtgfisoq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pxgpariz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vpvhwoxg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sgrqgpkz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zxcfpybd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jrffqkam.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cgbhmznp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbvwiodu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wnnggkcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlxotgpn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezcvgryb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pagapgkp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lqxkyhlt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pltizmey.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3avsjroor.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aqnhjusy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3aynpyiae.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwpxikku.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqwjaqxl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ioetlyel.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qhpofzcu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vqaolpht.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uxflolzn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpnzxmyg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3firbudje.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rzrsbjju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3drubozdk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fahljuol.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3crbvipwa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3molsjldn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zectpwln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qdmirdbx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jgfkgjqj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qnatgmws.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxchcug.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dokjzezc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3txycuusl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3khkiknlc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xorizhfl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3twylulig.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uaypijab.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gcsuxnhh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zaamyufv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3emueoxxh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fvrszhmu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zzekagqm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gvlexxmg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ooyydobx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bhnidhzz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hamdfyfb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxwvonsx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbplkwqn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tqsxvaon.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqcekflm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3baqauvgg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cadsjlqq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kipbrzxw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fzuiofxs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtvmauv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tlmaqfhp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tlunlzzf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmkuoyke.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exnsckmt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gtnjzogs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rjaoiopi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3amccbtbp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3binyoqir.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hiivsjus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3awwuksls.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3unoxqdoh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qixvnkep.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ghzzsrtu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3iibdvimk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3exipcyeg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3juagqqrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ozjwmgcb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sawtdbom.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jllmhctl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wpitjrfs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxjhqdj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bjmqscpj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3swsjmxfe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wmvkitpd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bsjsrkrv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cqmjjzqa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jovkjvza.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eqfmpnjf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gplxujnt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dhnsrgjr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmcqftay.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xcxvzads.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pvqlosgn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpgmcnj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hsewphky.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3laonlsga.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsredyxr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ipcjilnd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyiqrmst.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3icroucxj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3perbhsim.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gizefcjx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxdnsctz.html


<!-- 参考信息 -->