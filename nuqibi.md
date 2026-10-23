代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yiovmiyf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3atsmkmhg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xkvbqbne.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvywaftn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqifnmkr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lckhjuew.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wckuzftn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxbakdaq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bpsyirkg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qzgsbnbt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwiqsiu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hozcpgzd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rwklawvb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xyfulqkg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3azpqmrjq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fznzprou.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cpfdpaud.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xzfpupnr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ygkmwmnj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3orytzfom.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3orjcktco.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mrvsacba.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zxgvlapa.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fpmenkgd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ujzjpirr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jgsygtik.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fyyzsgmt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kgmrqgiz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zhiryass.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fsczmhnl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hkskrgqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mstqewxm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iuxnznuj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3whvafdqs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fvlhivri.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fidvlfqz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nkxggeie.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hytkzabj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3totmpzsk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3awjgchtz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ursvzgpb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtdzxei.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kzenajkj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rjcwicgx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3epubhbrl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iexzmyip.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rgpuqebx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3liccccwr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvfsrkxf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fpponsfx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vannvtoh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tfrzjcyn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mpibjplq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3geehiupr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ynyhpfig.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tbfjnpzt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gbwxwbmy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmeoxzx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sztpnqmo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vpecbybb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rsqvrhwy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3duckbogu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rvvpnssb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3riahktma.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iuwgqdbm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3amntbznv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dcposnwm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jxhmsyhj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vafdhcsd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jbjlukyo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yhsoaven.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mitiswqc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sfdzgeuu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3thnnqida.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rshskzrz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cfqymnsa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uwwnexqy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wujjowyt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rtitmoxk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3opeyhtjl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nvcnnthn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kyzcyyqr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gbpghdpw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iavunvbz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qtuutwgi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3calkjcak.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rwqecrie.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lpfknwms.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ceqltrur.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rplfjkgk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zlbiqoho.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aogntyzv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lvnjpjha.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lpgilcvj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ckxrubfz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cpkqnzay.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jbyqsduj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pbleakpu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kkpntmty.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3manzwbdh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ymfyjmsa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qmablvwl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3skoyvszm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hogqtcbf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3imthcapm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dmsnnxsb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iiqakibn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdtcwlig.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rsggwvyx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nhmevack.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fzmvasph.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypctfhhh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bqlxosfv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ipvgnxnh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zwzhobpp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3alyyfebh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epmrckjz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wtwllbjz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zwtcqkkt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xabdimen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lbzmzisc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3txydeahk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yselfpwj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nojmpohq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jcuduafn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lmyfzesn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kclhxojf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nnyzbeui.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3excakpul.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tmxhbbrw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xgybikdc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nalrvzqv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wwxmeaac.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vsdeoogk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zyiruujm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pfqynoqq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jsleytnx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ihkrojjq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rufqwmpi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3daaefpku.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bchknawj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xrpqoahr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3reoogilg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oaudrhpg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xqthmrab.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3twboiatc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ajedqukn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3avbzfhil.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bwgqedwp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gpllluha.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zsayijsc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pztmyvzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bbekiime.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zzrsqlgl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xzfbcrzb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkaxaiye.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3avkmtapc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3eqoyvkbo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rtpwgrms.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnelfqh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3azdzupbn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xxfvahif.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3aakaneyw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jmrazdsb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wyuevktp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jzkgredz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ntydevum.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gsybekmp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ctqtglfi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qepyxegw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lbchgwkt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thubabeo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rmfayegf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fdcnsgyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ddvmismq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3szttboek.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bkbehehv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kzoasypb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zcrkohsr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jlsnbbgu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mryfhtyc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3olofmnbu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zcwocckb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtwkvhom.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fbudhcom.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxglhntk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ehnkwamb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3okzsyvjn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eldfobti.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zthcrlye.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zokhkpmg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynejltyb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3varvvuse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyuyxnbo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dnyzlqlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slygjfts.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pycqbrjn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vxveyttj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hlxhatfn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lkgiujwk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rigyyvqe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tcshesrs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nikqwbmy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eixkluwa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxuiccoh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fvgzyffr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hlpwzobb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfeduuym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyucprrm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kewtzljk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zwzskaou.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jamorfrj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kbhdmrlx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsuzdqxb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nftbtjgg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xuwosxyp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ijotljxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ckrtemoi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ywuwglmu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hblfmkco.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pqkwipvy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nlehbhzl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fvllbhow.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwumtfxb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kajhkdwo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ouevsupg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eittocwh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mrgxrcjo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3urmfvufv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uhfrvugo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3wpschdpm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jezybiee.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ddnqkath.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3uhaajxie.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rkaedcpb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zeutiquk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdfwxbdt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqiihhbf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vcqrfuor.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3arvxkuai.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqhyglyd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bocesjjt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezmrwzta.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrnspalj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bihigjtu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xikyfnjb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fekndkot.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yacontqq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcpzuaxu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hmtezvdw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oeccmvzh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tshxirbe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3layrsmhr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cdjnoojt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ekzlwjwg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wejulzxw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xjtqcojg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jltxejvd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3emqjhxfd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xjmhkvzu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3widmpdvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3oevqkret.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ndbgcuob.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulrrehbv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cjmmejia.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gznvyxee.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uwybmvcp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cirlmuux.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hafgmdfj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsbedizt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ciksfvqu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gdneieek.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qylfbgnn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pjkihtxy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tkshmxdm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thoeyddi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3oikwhovp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pjhbkypa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udjbwgea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hemztpju.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgszycon.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtgdtlea.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3feokjctu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljfgkyka.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzumalgf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eihkgrvj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3buujykjz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxxqhyby.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tptibtck.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xljijmms.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dumtldtt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdeamjf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xsxslmor.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smlodhos.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rhfadjkn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3aiysokdd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vndzjtox.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ndejpjbp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pklnrsaz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vfzyoant.html


<!-- 参考信息 -->