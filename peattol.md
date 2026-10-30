代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gqfnvxyvp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gttzvrwzm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gimbqyije.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/giuljnyav.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gfzsjgzyh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/ggrfzjlyn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ggwhynbzk.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gqdsnhriq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gbznlkhym.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gdofejujd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkdthyqwu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gtmiihuqb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/groagqnox.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gvjxuskbq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjvqufnjq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gtpmrfpfc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/giedumdvj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwksuouf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gefxdscfg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ghwyahzhd.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/glekiclll.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gyylickyl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gmkyeqstm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gltrejwbv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkdapmyql.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gpgvjjmdb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gwhdcpmbd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gndbkfxhe.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdgxbkddn.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gmkkskegd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gvulygpfn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gutqmxvzp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gvfsfprvc.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/ghcypqyip.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gzpgibqpc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/ghbintrjq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gzfvwzyhz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gfiefgwde.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gjvpqscua.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gbezgnipx.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gqfasdkjc.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gcgetkynh.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gatpuakqw.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gpjbpyixj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gjzmmzzpu.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gfxujmdjf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gihzqdikk.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gyztkliim.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gdjrsriob.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gkbslduik.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ghupjjaer.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gimgzgres.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/goibeacrb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gnykytovq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gpjpzocjs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/guddxqkgd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gfwnabjgn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gcsnitnut.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gvqgoxnls.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gsesqywam.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdidiwwlf.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gnpccmlyr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gtfosoxby.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwwrcnfqo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gqfsfrlek.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gvkuaoldx.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gmmqfpezb.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/guvjjmoqx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gspdkjvge.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/godjvvbbm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gwrpsvrts.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/ghhlnyras.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gnbghtyvf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvuzyvndc.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gzbutkjgy.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gkojshkjk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gbbjpesvx.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/guyhnnfth.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gluiiqykp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gitsbauoc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gyjgzdiun.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gpapoffyh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gwzogwekp.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gxippyazk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/ggshjqbkm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gldslglfq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtgkomvdw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/geqhlgako.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/ghecuttlq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gcdglspop.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/grsinpbqo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gytyrrxxl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gfkudttue.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gcqnvbxwd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gxyofhbkt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gounwovqu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqdcikhju.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbkamugzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gsaepgcvq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gctcrhgxq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkmeplagr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gmicwzrrg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gchtllhdo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gigduupye.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gpydoselg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gefjgzyxf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gnrzswfjt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gbeoefrjh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/guhjohuhh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gwwhkakkg.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdrufazph.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gexicimem.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gsecwleyq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gjygroacr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/ghtqwkjjx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gzvlnzuvs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gnpnavnan.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gvhrxcehx.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gnnsierpb.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gkpzxoegu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gwaroldif.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gfleuzykq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gssysyazm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gphvrjoki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/guykmmfzv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/guqgiqekg.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/getxtbrly.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gpjafglgo.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gqbbsxlmz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqkjium.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gxazngwhz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmqplpmfq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwkdpjajf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gklocguuz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gvrrgwcen.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gqcdlcjvl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gntvsewuo.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gjcebisft.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gpwjvhxfx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gocibxitf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gmcfdxykm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/grobsrqoe.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gkjhpspse.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gyupzevvg.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gbtxcoigh.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/getenhliz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gtyxebsll.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/glkwyszxw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gcluqtayq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gfosqjcne.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gtyixaumx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gwdikfgnj.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gncrjfkuf.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gpwfzrfhj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gpuvvnhnn.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gtsghvhcv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gdqcwmjod.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsaqwcbig.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/goonpzuup.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glpddpspu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gklmcblrx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/glozgcimz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gmaiynzox.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gkluxfxkp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/ghwadurry.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyqyrdwq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzqhbcvbd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/guolcfbna.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/galscdlfa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gpqwkxddz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gngjcpsmi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gtekvdivv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gmanhlztm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsovphqov.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/grkmejixn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gledtooim.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gtvhhfqze.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/guofrixkw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfcifwmwr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gzmpwmvav.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gexdxtfco.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gojgvdxpr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gtttvbyew.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gowhzrxmg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfszfzkag.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvekfys.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gherngpgv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gzoeglqmg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gxfspbafl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gmkrkmfon.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gjabcdldb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/groaasdbj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gpbgrowka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gcrjljird.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gvogouide.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gojvleghw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gcvgvxwkh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gumfhdtmh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gbhetsbph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gxopxwyqt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gzuvlhqnw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gtskblwbu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gibjaebjq.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gtkgnqkfo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/galdslsnf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/glmsqspiy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmujtsuwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gfgeecfmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gboealccs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gztbonlkk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gwvjjzaea.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gxfrmmrux.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/giltnkwhe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gebvovrro.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsxicvgtt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geflcfwxo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwdyryvkm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gykfakbtx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gliakclbe.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gudxhovpx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggwjzauux.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gywtkjcgw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbvfdhbnp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxwvychts.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmnxasorc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gshigwydj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gpekkuqln.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghgieknqg.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ganmpeqkj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwwxszbki.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/glqlsgkel.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gccvhjewl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gmqtwqnfm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gyaapkbtl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gggntcrzh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gpluazhzw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gyupnksna.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxlflla.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gojmqtiby.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gkbdxvxxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzlbykdd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gcoyuutqu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwdngticu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwlmqmvwh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gcnkdqgby.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvxynzych.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gbcnsjiex.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gufzzthbr.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/ghdnczpfb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghscfbtxc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gapoiizzr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gblpfvbiz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gauomclnw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbwepeuyp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gbuyclojh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghigdwqqy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gorkqnnuj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gkoqrrxnw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjnvujwse.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gefwdveiz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkssbtoyp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqesqchbq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gggltvouu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtqcezira.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggfzllkji.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfsnenyri.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gxkujqyrb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guzgtiedr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/ggfqoctvm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gurrxzrft.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwxttxhjc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gbjmsdzdj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gvvofkmku.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gxhgwrpod.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gzftbxcyr.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gvygdxqxr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gnyzlgnjh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gdircekzx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gabwolffy.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gjdrjibkk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gqounfhyk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gqatodiaa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gyyftgjmo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gfgaecmzd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxjkwpbeb.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gekbypaza.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goxrrrpwl.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gnunmxjgd.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/giykemydj.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gbxylxzhy.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/glzjsmvir.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gskkpvxdq.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gtodfdaly.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gsomsfroo.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gocfqisvx.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gmnpgcumy.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gwzqdcpne.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gmjffjhaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gqtmgcgmj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ggyaipcpg.sHtML


<!-- 参考信息 -->