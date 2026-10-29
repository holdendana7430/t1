代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gtcishtdl.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gdafeqqsq.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gvjmpcykm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gfgmiiqcf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ginyutwph.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gpdjfzwlc.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gkueidjzi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gqsdqzojc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gfzvdrwak.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/ggftvlrbh.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gunsipbfx.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gvprhacab.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gmpveyzij.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/ghnpzbipg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjjdyxgue.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gworkuoij.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gcndisqec.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/guauqnhta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gptdvcxnr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gdcrtthlz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqqmjmixj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gmfsohsjo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/grjscbqck.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/grimbqkfh.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gjcnxmfhy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggolrdgai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gszxgogrx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmkgkmnyg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqrtpdpjf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gktjqbzpy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/geiomglbe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmgbqpjop.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvtdefunt.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gybbscubd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gkmnljfkj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gkhjkgtxg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gunrczysf.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gbjzndndg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gvtsjsuhc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gidgoxlou.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/glnseyvtx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gmguoycwh.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/ggvqbngkv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxwoexy.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gmwfjcnkj.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/glalwqymv.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gbipcsbgb.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gqjqibmnx.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/ghlauuycq.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gunagubcy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gbqjavlhh.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gvfhxunhk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gudliyrod.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gvjtnxuht.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gjmxwtjrt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gluztqqcx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gccstsmsj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gmcynqxrb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gmcenrgkl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gxlyloxqh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gzahjdnza.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grzaxgmju.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gwhmrcvir.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gpiwujohq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwkmqrcce.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzjhpulmb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gxvdwgnxd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gomgaruyj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gcrgcqcof.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gjszcefav.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gxwgnjefp.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gkgnogigj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdvggqunz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gpoimblxr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/glqnmgkpd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gmmzfycrp.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gakshnuma.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gvuqkwlsd.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ggeqrqlzm.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gmnxgvjyq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gnazyallg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gocfrgpbv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gsknopqsa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/grqtjxjme.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/guybnyxvs.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gscpeqlxm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gygrjyrfz.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gtixbjbhr.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gntvgbesl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gbsbzsrig.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpvuwtbue.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/grmaauolw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gefuhxsok.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gypuogzxh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/grtajgkhe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghvvjljby.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gkwezdold.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmorqfndi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfxpmttfq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gdqaiulcg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/glmkjfbpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ghwsfbelc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/goacgxhkq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gkrsbiofi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyzgbjscn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gpffbipgr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gnfzzrary.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gpovhkqdn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gojjvcpfm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gsyjwnpyk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/ggztajasa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gxtymtnqe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gmdgyusgr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gflqnyjrs.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ghxxvnqfc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gywnohgju.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gbrjgnddy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/giluakrac.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gwduxrrdo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gugjgulpe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gnsufozat.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gbjkgkttp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/garztjnvc.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gcxafubdk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gontxmoiu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gxsssrgii.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gttpdtkoi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gmzsymhjf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gcjredwqk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gimxbqorr.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gofsscnas.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/grhzgubja.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gxqwjfdaq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gxbfbevik.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gwkyljlqu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gevnzjsif.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gdxhmwssw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gsvoomhpo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gumfyszrz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gcxqltyhv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/givhblckl.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gamqayagx.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gvmgknofd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwqffftri.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gijszjqku.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gcwmmxwvn.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gionjtchz.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/giszlcyms.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gbowxbcov.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gyacorppj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gfaouvqeu.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gwvwwalth.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gdrxkbusb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gekcvvqyu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gbgmjbopo.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gwaflsjyf.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gfyfhrame.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gadryfxuq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gdbbcxcay.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gusiatnkv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gmdzaidxu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/giumckdnx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdklhpcqz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gczynxyqk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giafuvxys.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gmtbrmnol.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ggpxtjtsw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxaqxvwfm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gazmplcyp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfvkavynl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfwinwwts.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gujfibcyw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/guyvmuycc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gvtxcynbp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/giyjjjsvi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ggkvnlmoa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gfxexugld.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggkpfqjun.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gejrkylrk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaxghoetx.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gdboenkzl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gpfhbzpky.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/glqbmatkf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/girrbznih.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/grgqgzxxt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gstynjbkx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/ghvfmoztj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guunxdgyk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnyydbpzl.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/guzoovapq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gdwwwogvy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/graejlvoy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gdhslidwa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gpyifqmvy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjhktkcgy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gxoloespo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gtvlcwbxx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gxzyuuvqm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/geiuaplth.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gwdgfmlfl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gxggyqyqu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gmkwsdyfx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gurbznfqw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gncmohzuh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gyklpepid.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/ghouvbnrv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjtepbzrm.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gpcmpyqdc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gmcurebiq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gvolbabet.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdexyqrxg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpniaerxq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gvblyyths.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gxgrbeeqn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/ggwgthdpz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gjgzyujkg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gdmcaphbf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/glfyfovhz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvnshza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjhyhhsic.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gidzhwjsg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gxqmytxyf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/ghrxejafo.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmssozleg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbjaxjhxv.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/guoclwjwq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmqtlbjnp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqtopwtcf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gydlatvve.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvmykizwv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbsrdrtnl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geamutvkm.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqoxozohj.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjrlchoeq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gpseapbsz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gijzchece.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfzkdruyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gmaftloqf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gxasolsbr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gpzttapes.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/grxgssepw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gkmatiyph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gfosekytf.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gdeidzeax.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gwpflsvqy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gjtzmvqlt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxjyyndji.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gubtgagmj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gyfaelitb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnmijkvyj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsmaqxqsp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtqtgjjop.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gzkuskbve.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/guajefwgc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/geqgsnzkt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gcaeowlgy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtryqwwbb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggvzkcqui.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gfqffmbaa.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqgumkvjk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gdzrgnrte.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gehgfwnpj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtiiagbzn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/ghprwabhu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gktpqvpnc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdzshroec.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gifabwoef.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvsmqdtdw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwxytxunt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geohjzsow.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gmoricfhe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjlikgfbo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnvwgphwe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gevebbpja.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/glfueekef.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkvodwnrm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gdzraopev.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpkqjldum.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gayqqvhgr.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gxnthxxye.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gbaslvuhv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gcnzumtex.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gnethyfwu.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gmnsjapli.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gtgalxpsr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gnodruzby.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gnxphzjxh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gokezkwiz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghmwxliou.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gixbzximt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaxktufhd.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gkwqmqkml.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gyhmaksrm.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxdkqselv.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbpkhkgei.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/guiknoljx.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gwpsvhtss.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/geuljodjh.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/giddrlrpq.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gjzbcgeee.sHtML


<!-- 参考信息 -->