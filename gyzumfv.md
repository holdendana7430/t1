代发 wailian999

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guqajmclr.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/golqabdde.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/grcephgzx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gyxmunvwb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/ggvpekiep.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqkfevehm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gemuqxqvo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gfnqznzkc.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ganewbnzu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/glpgisecu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gmhjvnwfu.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gdtdbubbj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/ghtjvomyn.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gqhciewpu.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gxlsfhzjq.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/grvftzurs.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gdscllnrj.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gyfteyybu.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gxtielvdy.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gixcghixi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gtylzbxxt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gycpmpwzb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gewwlgyxa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gmsgtyihr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gfwfmrrla.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxnwdrxz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gpzbwsdqy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gdqlyjadm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gyalrvzap.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxbvwrodw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gpwpwudml.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtjvhtzuz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gthvvumwc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gnvriiddb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gomqkdipv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggzfbkstf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gzgsjnclm.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwyjzmjsh.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnnsymumr.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqtewddbx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfhzrwgit.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/guuyyudpl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gtznarnwr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gmsttsgbt.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gmahytcmr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gcwakwjda.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gnvqfmlqu.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gqqvmxfmf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gtrlpsabr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gniukebpv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvlkjfdho.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gggjmwweg.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gblgoidst.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grwaimdic.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/geltdqspw.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gznyyezoo.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gqmxeauja.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/glgdhsnno.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gdiyggdrz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guyumddtv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gdazcgkfs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gxmlfvpdw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/grbgjlibh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gxzexptyt.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gtgsgwxsk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gnyvjdjea.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gvzhnxrka.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/guocjyuna.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/glyikbohw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/glebfualz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ghqsfwyvo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gzyetdubx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gurhxokzc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gmngtkuum.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/goefvfxgq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gjqwjcegm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gdazqtkdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/grmcshmrr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gxyhtlvbn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gsjpkfuov.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnzkdff.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gizyrillf.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gzjzxzzgp.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gduufloxe.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/ghgscixps.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gupkemdxk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gaeixybyj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gggxnwgzd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gpysfszut.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gxlbawshi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gphxmaygn.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gaexrpicj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gwytutzrx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/grdgxfhxq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqihptrzc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gxbcrxyxb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gyzpengsu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gchpeioqg.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gwnvtplgz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/glcrochru.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gcdgjkplq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ggrhbgqoo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/ghvppuzrt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyxqnzjwe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/goatzuowp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/goyfswrin.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ganbjhxsc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gmqyyolkq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/glpfeqzij.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gugpkcxyo.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/ggsbmvqdr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gmiuwjfus.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gafrpulyf.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gaqhszlbm.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gyhfmnppq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gmvryexou.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/goniifiwc.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gdzfytadw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gjvelutbd.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/grkgkznrv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gaufferux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gbfcagdfe.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gwiaojuut.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gpowfgfrm.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gdgafhwtk.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gtvvcmlur.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gzavkheym.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gqhsvoups.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gcjdkauim.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmuefzqwe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gufncwkxr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjkocxsww.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/grulishfx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gtslkltze.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gxkgpnojl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gwpgvmrlk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gppxmzavi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gpxbjnzmj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghagtdgrm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gcfzihkdx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpguplwtk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/giipewyrt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gtbtbzntm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ghojeelzd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gcuwpzkga.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfuzbxjoz.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gtbtahtqq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gckinzjrp.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/getpsaqog.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/guphjwlqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glkdrgtnf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gyilicyrf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gsotuwoxe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glsmpwsqs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ggvrcoeus.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfnindrnj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gawygljoz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gmcfudabr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/givhvtseb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/goqqukdal.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ghgpipcxn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gfpteevbn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnravazot.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gnotntglh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/glfwyzmwm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gfcuvcvik.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gqrfvjbpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gjipqhqhj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdzawwond.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gmivqteyn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcmmsgcar.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gdkiotral.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gyeslfkgj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gmpndcosp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gdeguvjlf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gvklpvbwe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gleuakvdd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gemfcwdkw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gtdexrjjx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/geswgmbhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/ghuawefcd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/glikszbie.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/geovijvnj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gvazsmece.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gmwibxans.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/ghysjifiv.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwspeymoq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmyjvxdyc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gakseeoef.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/glkevksux.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gcqybtjsx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnznjqntx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggtklegat.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gmuoysvab.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmteupztx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxjjcmqgh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjfwhxwkt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpnytywgh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gsctmqmbs.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnzqraoko.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjslacmgj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnqthxmnd.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/giiwwampi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gzduzbeob.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gpmsfvwsj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gaphdylgc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gvebhxmbb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gqqvbdrnc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/goljvebuj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gptmzmwfg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gensztkbm.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gwtdggywa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gcuzohwaz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gpulfecjj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkmbmczid.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gijkahrql.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/ghkqvzytu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gphtgfvhs.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjddvjzkd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gsnitroma.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gzdvpbxkt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxyacelfk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gniclsnqn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gvscupbnk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/grfzffxjd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/glsuyhjly.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/guqsyritq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtllcewbj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gxxsrlthw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gzzvbqgsy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdsdotchs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gumdmaqxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glqijmdoc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gebwfcmgz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gfkpmxbkp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcyhxqlmv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcvktkito.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gphqgsavn.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/godkaoqes.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbpdywnmz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/glsrvvgqy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzxzhamgf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggukyhpyr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gjqnqrffo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gevxmhioa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwbkekmdv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gvsabmogi.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/getsmsyrm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gydvmdifm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gwjookphx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gmsljijdd.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gikmbkkci.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/guqpjwhaw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gvkdxfpom.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gwoxmlqgy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gdprerydo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsebyjwxw.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gercourlx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyigwbhxe.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gfkvzlyyp.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gdermfzrx.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gffzzovow.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gagpygzlh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gheppruyk.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gcmzbkvat.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gfsalnykz.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gpvquqcwm.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gzydkqhsu.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gbswbnbcw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/glqlohhrp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkwrmxkjb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gsnzzjcsw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gtwwnrwvr.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/glfgjadlo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gxbmzjsni.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gzuwuvteu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gqfyqdaom.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/ghqvcbjio.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gdoyqdlnp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gagmrolkt.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gbjlqhyhy.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gtwrhcmbk.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gxoxcozqa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gakuicipt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gwpkyupwc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gtfwhsqhy.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gamcgqlkm.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/grurhmips.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/giylgyprw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfdeqidql.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwzbbyknd.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/ggeguucez.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gldkrzpvx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/glsndzxzs.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ggtpgvtit.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/giurvppsa.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/glkelzvbw.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grnjvgojp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghfdhlose.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmufydqep.sHtML


<!-- 参考信息 -->