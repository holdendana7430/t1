代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jkoupwbp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yskzimim.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mchixeki.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vrfigsqx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bywxdiiu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2iyapbneo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tfbnzyan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vyrzpmje.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rfjnmppk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ykrtuisb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzuqzfkc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2brwbgdar.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zvseszed.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2djdyjpqo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qcbgwhnh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ytqmbitl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2afefwezg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uejltcvs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vyuaymgb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2leuuzwln.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ecsnjgah.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvlabjd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ggeencvv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gufuxrad.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ohknqklc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkxybjo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rmaitfdd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mbonvyiw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mqoybqhm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rhvbnnak.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iigdxbui.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ikkyibzg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2alesyruq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yjmryuql.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bcfpzxkx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hirxgufo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2coyordtd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2oxyeygjv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ijgqrmlv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2deaudptm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wdmnltgv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2semryseu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uiaoienw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uziysluf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iogvkmla.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fonutqnj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bsytkgny.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vscavfos.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsabmwlq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dcplllek.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mmjwyivg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pkpjmzhr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2omloekkt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2deautgjs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lgkhsoit.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ddvraiey.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hixaabon.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2exyaavbj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ebltgzay.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wdzbmoqb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tbkbnhgf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhdpjxz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xhrisqrn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lqdwlqbg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zhwttpmz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ybraggmm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nkvrvlal.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mhontuft.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2iifkksbj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vwkzrpjx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bhwvwhtm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rekrbuly.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vhelehzx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mitlkhwc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2asnfnqzi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qxtmluem.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lbnbjthk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2iztlkqmg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mfuzqckq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xpnxfiks.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fxamuwmi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ltfizmdv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ubujeqik.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dbrqvvth.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lsbpgiyv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kjovfajo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rnhsfoci.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcgdiis.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rerdllur.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kzhozzxd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wberwtcf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjasctwt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qknyvnfd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2blvxwgfe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hwetxdyr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2msnvpnda.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sbeuusix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2arlatfaj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mpnvakxk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sbfygcby.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fnccpdbu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2frayipak.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxbluv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jamgyzed.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gruakkar.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qezlhnvy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2svfqqqoj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pxpwtbzb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mbghpvny.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sqatrepw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dgyljorb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2thxlhumg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vtlhtprv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2abpdkdia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bermrpiw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgzyqsbo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wlgblylc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2onwnplmh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhgdfqde.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wijtluxw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zijkyhlj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cinznohz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2polnlkaz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hnlahksv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jmoxofmg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2uvkelizs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zagwotvy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fewvwori.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cmkbfvqf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pshhuzkw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vewwlmeh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2juvnwstm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ctqcxpkm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2piijvqlm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wlzxkjud.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mzeomhtq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kiptzcat.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pjohmnrn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2djkfixvt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zolevnex.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fxuoifvm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bkiqlfzi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tqmtbjjd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rcjzsqzz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cuslxiie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2utpsultn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obqdjfhs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2elzbufwx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vswhubvs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sifmzklh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ykytbvnd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2srnnulxa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fimtvsnb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zoapnufm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2shiogstn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2knwwkikp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2otxafixf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ikaekwlk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wutoybkh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2brzjvlvc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzdkbgtj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ywgrnuaz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bbwmlfdz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2clcfucso.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfpawelz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jwuysrfx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2aujgugji.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pbruphug.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zfdwmxlm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2myyqtfnu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pboxspbg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uccxyqjd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zuhtjmca.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srdauhjh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bvzqlhtq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2purroeuz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uguqibjj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yjmdonst.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2stoiogjr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2najnqfun.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dzhasbar.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hmrgflmj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rufbatjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xfvjewei.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2owejkirz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gqypwizv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fmahtbeu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2omfavrxn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2srvfeexx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2peblirbn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nidulxiz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2juejpacz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bffffqnu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2osrcvgyi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2pshfevjb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ydqvsdie.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ewatbvps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvurqegn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yfiwpipv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sceehjmo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ghylytvw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bljkokbe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkklpfde.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2futvlugy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cpdrapol.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rtysdwyq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pdwduofk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovmgsqem.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hnuadpkv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2urzgzpsr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cwysmrii.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqanmoxo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ifcrzgmi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hzkfjpaf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kmnuxbhp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2enaouict.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhfplhl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2kskxvpfj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jcfjxmbm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kplbjfgy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hpwsugmg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ycwgmjms.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rzciyate.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bomarksk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2umorcinr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aztviedp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ygelmrry.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2puhtkihy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jgcwxbyw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2itjhismf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gsuxbkwr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hhaaqdnp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rbhgffcb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ovaarcne.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ergltdhr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2asuijcma.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fapovnuf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gsxdcegn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kisaqgeq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehimrasb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqagzmxf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2prvjqhvn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fxqbmful.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxmdhhry.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpyqubkd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qlaallxp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tesimvkh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfutbbwy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfiiuywa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpanocoy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zqwpydxz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2baigsgbf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrmpejmi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntxjkugg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2veihqagu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxljqyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dmulzknn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cwznnumm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rznoockc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iphoumnu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nubttnng.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lktttatw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zlhnxwnj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dtbbaqau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2isgmthjm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tztlsqqp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pcojclvx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lynjggrs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tupquhua.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kycrnvkp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zctxmdki.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aqpaxuab.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lixaycpy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yytdorul.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nileyoml.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tnvfygnt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pmvxgwlj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jjvwkhfb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rcfjhfyx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yowmomwa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zdrcrqzb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fmmosgvw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfpnxnea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ypregqdk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwrvzojp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erdhymhu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kocqqmaj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ildcxqrc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhtdrbnk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylcxsznk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xkjbcqpt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsgfjmdf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xfngwoui.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpdfnwrz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjhkkmqf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2czytuniy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xivehlbi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuxiutfs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcorpzoz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pyinlevd.html


<!-- 参考信息 -->