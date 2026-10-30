代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghevejiml.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtpkxhucp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gppkiypda.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghtoyehhx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gbcebqwgf.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/garexawbu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gosfilfye.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtxqyghcn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/ghqscltxv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gzaabftjw.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gajwffxjd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/ggnkmmcdx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/ggattjnfl.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/grroijaru.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gkdgxekwx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gizwihnfh.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/ggytbxwou.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gnhvmbdcw.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gtsfincjp.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/ghyuuiehq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gykhjkhqh.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ghjuuexbx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gtanrnybo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gimutjurb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gvftngbrt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gspxybqks.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gvkjmpdum.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gqlpkihiz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gfgoglslq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gbvjittck.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gizllrgiw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gjobouyyu.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gojsjwfqv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/goozhpifv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gsymbjbqj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjrtbosep.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggjsxzphl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggkesohtg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gxunuwinx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmawlofxh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnqzssgji.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gjoeeoawa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/grfiijhst.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/grvdtsake.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/guyjaodpv.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gdnvmouel.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gxfuljqkn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gynququjc.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gelkmfbkq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/goibporuc.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gfkojxznd.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gtizxfylg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gocwmfeqi.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gpqkuxejc.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwyoqbg.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/guikkhzek.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gfebwehju.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gamejcuua.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/ghrdpsnmy.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/geqhyeexl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/ghmdegmus.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gtftuzoqx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gyriaxtqg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gutygepok.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gdcuserns.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/glfmqgspy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gyvanlxvb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gchiqevvu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gujohcxhl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdjjrujxe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gjyvcgtel.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggljdtxcc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gowkeqwgp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gozyqxqto.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gikfkhfle.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gibotprbr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gwewzuanx.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gzwhyapio.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gdfwiumlr.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gnrdfrmxb.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gizlgcwyz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghzugtdmb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqoprxxur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gykirlvet.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gnpqjvhkv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gitsrwrwr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gvmvotjyq.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gyrhanatv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gfuapmrpe.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gxgwefiyf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grgtverlo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gqcdfmoar.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gjvfefhqb.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gqtaotvak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gthnqylud.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gpnrvwqta.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/golpzvuia.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gmdqaxreb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gzeqdxvqr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gxtxndjjd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gcihqrdsz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gkazrdmoc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrtrnpjk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gkoszrkcx.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gdqkxeqez.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gvxuldgzv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gnrapzjzz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/ggmoywcvy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/geasfelbn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gyfhwdtxi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gwkrhmwob.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gcsabunxk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gsnfhuaxj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gnkjuybco.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gdzjuwbmj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxipusqsg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gmqqgxuqe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gkvwrljft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gkjwqnzaw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gnworllgb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/goymstrgy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gwmvwmour.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gjwhftkel.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gnnyuwgpr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/ghlxpfaft.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gxatxzbmq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gfzgnwuwj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gcwofeptc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gkevwhhdf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gdemvlcgi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gjmaquion.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gyostpcmt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gypjzknoj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gjatksoab.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gxsuotran.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gvqgqbvwp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/ggwdcmijq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnwslrhyq.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/ggkebwied.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gzaimphqm.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gvcjsetbn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gpkylqemd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/glihzbddm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzblguikq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfvhirfie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gajyepdbp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghmbgxjrn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/ghgucmvss.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gytjcdbkm.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gzblozhdn.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/geisrmmyz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwvpsvoyb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gtkgftqsp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/ghaxdpsfp.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gsgldgrbm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/ghnpylqhk.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/ggugnyvdz.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gbgjocbjg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gsmdhjtxw.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/ganojqpae.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/ggebmbnxn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwyizirgc.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/godrskbrx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gggodunhs.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gcjdnteop.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gohxcktyo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpzuplaei.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/givflrxxs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gnpsgyxly.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ggbbivjbk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/geqwpenex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmkfiidks.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gsnqjouyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gyvououet.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/grnwnmydc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gznbivhmm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gyitzqjnr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gyqwqqcui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gewkqcucu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/geobyvibu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvsadebrk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gkfcoxqfk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gmzhvkhyt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gwqzzjobx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gyrjzeimt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gitpztrmt.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gmbjlqneb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdlwityxd.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gjsrsatdt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/grhnfsxew.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmqrcjhna.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gohkfvsrj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcwjgprwp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpqozmxon.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gpghtvjfe.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyfylqinq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gixgtbtsl.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gsfndlbft.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gjynntslz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gvrgyjczq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gcfmmmtak.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gbvpvuyux.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gktsctyre.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gofzmovrs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gpcleauaa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gwcgalxqi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gzhedcgia.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxcmehies.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/giagngdjn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/garoiddaz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gcazywvcd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gpelfnepz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gcplfbepd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkznlmznf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gszclqemv.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gzgqtkjmx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gzhegrwta.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gqjymvwge.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gsdecizlk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdswmbozo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/geskrxfsp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gfukhotey.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gtdofieio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gmebbeqze.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmuuxaxqz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gzgvozqnl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gagykuurl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjmljfxzp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnhjulzl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gjaqucavh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gikikhobg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghmxvvnim.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfqonlofo.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gaqlzaeet.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfftaloy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gciffdofl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpqkdnlrb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grpvtjxvy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbpmvez.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxnkxdgqz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaxrudlud.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gakdtitcq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/grxrcnddf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gyyjsmlkf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gruyraahk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gvzimdsgq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gxcajchfo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/ghribpeza.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gwfaeqpls.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/goxkzcixo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gcmnpgbhi.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gtcccrqrn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/ghhsfymmb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gvklicnve.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gzebdimnc.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gegcglkmp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/glsqnmzbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gpoapxlxt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gsfqnenib.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjczcfgsy.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gfeiphbdn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcyijmhke.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggoquwmmi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdiikxckn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gyfthdtym.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gjmovfwri.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gxjitmykt.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwelvqjri.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gtbusjvvf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqnlhuz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbelkkico.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gygunqfxr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grpifgezi.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gukbtsekj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gssszoarq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqxyesnbl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gslpeupve.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gztqqiagi.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gomqbhpjz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtbtceuar.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gvowhcjim.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmlowmdpv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghjjkduap.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwdancsgq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gcperutep.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gojoepbzf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/ghpwlgjlt.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/ghnllwszo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gvdfuxjzq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gedsmgqxs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/glldadklj.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gwmicbtyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gwvrvswfj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gsphnkokg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/grdfeuefm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gcghlwgkv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goyupwcqq.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gasugfxyk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gizaecdob.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gagooblht.sHtML


<!-- 参考信息 -->