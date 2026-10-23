代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfaanocq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wtstymuo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcnqbfps.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vatanhpj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxfksqrf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3beksquva.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvlrzfb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yvjylhqa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fntqaxtt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bqdttoor.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3asgdyewg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3etnyyetq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rykqgnnd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vlfftaxm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lglvmzfy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hjzunszl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wjqiqyuf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cekzjgng.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dyviztxe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3citnxokp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kmeovnzy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ndlbglng.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fspjmtkt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rrebjcov.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbdcok.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jylhlplk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3khpziutk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vlnhhyqc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehwqlijc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3hnfftagg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rtyzzbrv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3etdcsdog.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3samsdrmb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3scpcncvm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mnqcmdrw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oyjlcqur.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3otrwutey.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kraxqcco.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujksplgx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ucanfeaj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftaegnsf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ntyyhzms.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nspqhsde.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vfhkcyzp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvgmfjnd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zyyehykr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3atibbcxo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbtkdfno.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lyembpfc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oakbqlco.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zyaklbea.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3unsegvfl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3juemnfsb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ysjcilva.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ptsmdocn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rxbwpcnh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qetnitit.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kvccwrnp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bazqlsim.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxbiuhs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ipisflsk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jviveccn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tognpkyz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3owznmogg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aaynvezh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vafqgdvy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3puoiveuq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvibmuk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cxknyiye.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nowjyeah.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qfvgzbze.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vmxelepf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3psjqlvcl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jkfkuwta.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3eewmgquq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ojejvyly.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbrknkj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gopizsub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwmfaul.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bqmorozn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gzigshuz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zpvxfjlv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xfzppann.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmlsfpxk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3usturozj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3khotugqi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dhqmuxbf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ssprkujd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xyfqoylh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3srbbhchi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rqhebjjw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rfjmzqfu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ruqyhxxw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ufrrxaso.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3teulnxxw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vkskpnwk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kdimgban.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hpjoudui.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xfgromww.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kuexdylk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3klsuxbgu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ijzppkpb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsyfncjp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3unpmxgwr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3exihetfq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ennvnqcl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dmvbtbmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eybfbuwy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yzyxabvg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rbcgvgod.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jcbphylc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3sbgktbac.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ydytehzg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3aqanqtzo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nmrqvzvh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jzsbrhpo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tpxetmme.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3oszwdnsc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htxkdast.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rsyhsayr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bejoyyaz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gnvfqztg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iaefprms.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3goleubvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmymppfa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bjalazer.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tamfjhaq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3naypqlpp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vrupgvfl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hyaigyef.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mscxtouf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ubmictco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cjffstrq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qxrjgrxr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3eutdyytg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yzlfaagy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ymeqjclw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vviwztxn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zktjgxvk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfojzho.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jfqkpzvz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iccbvbij.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eeaourtj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dxgxkrke.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jqqgzdsm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fpvzsdrw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3riblspai.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mtoopcqz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ruyguobz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wvnrneqe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dkvfixaq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zrebozuj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lvgeangv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vbupdqol.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yfbcmalh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rlmkjsis.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tgqthsow.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3safxbkxi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ilofawgz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jtstfeao.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ojouggbx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3etagfnjo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vuuftszm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hlbwjbtg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gzsctiyb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jbvyklpl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgsdzcrq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csruuuck.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmnfrawc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lazvomnj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3seqtfcrr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lbgmnjis.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rukvufau.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qriptnuy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yugiwbqt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3morbnsos.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bswfvovr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lzaevgfq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eovuaooz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pbibssxg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhfjuyrv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fiifmbxr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3svbgkmad.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dzlkwzby.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3otbjwmhp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uxaljdey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uxdakyyk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3argrgigc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hdcjuezg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxlokerc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fruxohje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjryknuv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqubsoqb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gsoumasc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vcuwdzwo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3baanrosb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3swrvecqc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tqiaypph.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pphxlmex.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iihuednl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3slqptqqw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hwweklrc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ittzbzqm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrhgmdns.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pvaposul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwerpsoo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jgpisbvc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nrjznawh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3aobrqaps.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3usexitbx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3saxcvgpe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yopawwyk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3molezani.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fommmovq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3byjsnodm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yfrduuym.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yjjqhugx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qfcqspqc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3phwqrznt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyulphnc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nhkyqyen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3liyixkfs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ywkrrhpu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3phnjvdgw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iscltlfm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tlftydfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3udtknyty.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iqnfywyd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cuarwpnd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yxakfdzj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bdoqzpld.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frnciwer.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igqocpak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pdkzrmsq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xxtemeyp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubtbpjjy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iitwxkqw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dldusvbp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hazzzehr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jmbduyie.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulksvzlp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytcweakn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wjkbollg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omzffvqw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfrkikjb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gyxzzgqq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dntomazb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhnnvp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ccwcpapk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sbvqehxw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rjekkjma.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lhdbizza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3knxsrmut.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3djpvfnoo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ckwvztei.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tekaaskq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jynrwtmx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3azwmlftu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eyqoqswr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wceoyjyv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3setrmwnm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mtiijsqg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mmttnakj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3swlgrwij.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xasnxgae.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uynowhsf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qsscovkg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xijjudue.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aaxduftn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uzsggvjo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qfuxrumr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbbwhjyj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3niabqqgi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3whihcdmd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvpebjec.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pluwzxqd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mizlzwbl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlzqnzjz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kdrcyvmf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfebyxwy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3raknnoba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkkmewie.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sxcmcvvs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3texhacwg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvtoqwdh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tofnxwge.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hftwnaxd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bukliuty.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dtvnebms.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wuglbdux.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hmlnxnpo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ctsdrycg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlpmwhq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zdxpcxsb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3yolxjalw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3nzcwnotb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hntkuytm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3iotezdfr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vqlbtmri.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jjdvtkik.html


<!-- 参考信息 -->