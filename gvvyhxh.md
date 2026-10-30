代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/goncsodmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gqkbaoklc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gtfillvmj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gibvewqrk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gwuhtrtde.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ghoiuufqd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gyxqdswwk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gitvxcfpr.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gyjnsflrp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/githubkfx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/godvsmvfv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/guszstbyu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghqlaifnu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/grnnqcviy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gdlmpdaim.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ganqcbqan.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdnxcytpv.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gglwtxgjc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gfnuzmbcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gwqesagny.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gizvbklwo.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/ggsuzrkiy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/ghalrwmjk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gmcronlau.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gnienwatb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gkmtkugua.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gvqaspgrb.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gtodngvfo.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gpmblecqz.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/guhdtyirn.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gcsyljkbl.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gjgbytikp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gcuphhomi.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ghsaxmhnn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gknjkjqxu.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gkjzcsxtr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grpeldheg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvjhrmjgz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gcjbokhcn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gcsfubxvp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gfattlzez.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gqjtczwvg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gslihryag.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/glgdhgifw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gtivkixnm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/givhbpdxa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gglcivccm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/glhvceege.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gaqzbhnwx.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gmrvhdrbc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gsqrxzkrj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guwaxkacv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gxbejuusk.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/getslayjo.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcnqtslgz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvsdcvjl.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxwtcmlfg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gusagruyl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gpsonimyo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gpbaqfouf.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gownzqzvt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gupdbsscg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gmccvpwyq.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/guriehvlv.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gfeqlebyl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/ghlzwszbv.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gdexcbdsa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gijiltqxg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/geruztxrn.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gzrkpwwag.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gcbgbbfcr.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gbdsuvmoi.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/glkukdbvn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gdzsfhxbz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxryxaxuo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gvuclbfuj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggshdvxip.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gzskzlptn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/ghqfoaykv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gdcpqtgtw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gnqkfmfpi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/ggzccwiiy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/grxlnvlsc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gzvmvygxf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gwbeivlax.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gbpgajuxv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gvibjycjq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gyhbcxumy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/glrusvbdq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gmzhciabv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gdrecxiuv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqywojmvo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/ggbgzfkxc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gdqusttwn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gbspoijqj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gtydggwef.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gcdeclsup.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gdrkxzvup.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gxecnwacs.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gxldwpeqi.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gtxlaojgb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gjikawvsg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gwezuuytx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/geuupxeso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gtqtivffj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gryavzfqb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gpdwoipvk.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/golmvcbsb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gxxdssmmv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gmpsmzdrf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/guedhxabo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/getuzsmaj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gumfkosxl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gzupqowbt.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gjedtspcg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/ghjfkwcgz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gviihdyoj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gjclxwuun.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gvacnjcjj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gegwxcqmh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwbgnzfin.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqkzijfot.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnaoyukkn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/grgzxdzhj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gxiwttkpu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/geqayfhfs.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gwiqrztdy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/ggxomfugn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gahukeqfm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gbivcrizc.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gciabfayz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gvwjbrxdm.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/glkmonddu.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gbcwsfdnm.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/ghgyljsxx.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gveqyevnd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gazaymxdc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gatdlozrl.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gawngjvgm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gwagkldhx.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gnygfmxba.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gxrqkhaee.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gxwbgoskj.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gwbpzsxxx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gcikfabff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gyscixpdl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbneotjud.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrcaiyc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbzwzatrz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gltjjfsxm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gupxkwycm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gaioskiko.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gerrfrnlk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gzegpljwm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqrfkfnbt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gicpdlypj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmddvnxiv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/geaglibzn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/glbrdclbt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gmwhffmqo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjqorladr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfpoiaavg.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gdvqxjnio.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grxvvczbu.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/ghoytfzcs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gxwanupyc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/geikvkdts.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gvvjkipgj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggpiencrd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gcldolyhb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gsjawhoyz.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdlvwqdyi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbpvwifcm.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gmfzregwt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gyhxjwrfz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gfbsiraaz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gngegxiyv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gicquufzz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/grljcjynp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gkiahvxvk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gvlgtgaxo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gxpzsbkuf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/ggdahufni.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gycfiaswr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtwyeluiy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gupxuhewl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gmwqqkhkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gdcbgiyqa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gpxvoavnn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/ghvvcqedc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gfytxchma.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gzwburmhi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvyawpfwp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/glehufulh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gjzapjfcv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gjqakkrlm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gmjbaswae.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gphxsgnkw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gwsptomah.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gmizmcekk.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gcvtxxkaz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/galplgvvd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/glxrijtqz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwuhautum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzesrxinj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvyoxzyet.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/ghmuiqpyg.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmekwjurt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmkbqakpq.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gzektbequ.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gynosjadh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqyzlrbhv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gztngjmju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzcdpiskt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsqplfihd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjfeogrxm.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaoyrqwbl.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxkzavgod.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gumqbiyvq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gqkjiuuqj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gqmceztdk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/ggxzyjcwg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gqmbgwnyf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gmlfqrcer.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gmqpybonk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/glcfdcyre.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gjcuhpplk.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/garyftqks.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gqjlsmvly.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gukvrvnsd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gbpyvoluf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/guexicxxy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gthxbxurv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gpioxhsig.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvcykctfz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gpalwpmxo.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gwazlkjel.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbvriyehh.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gichzugfk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gkulujigt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gbudpyhjs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gcnbuinij.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gxnnjukbg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtiprsqin.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gmpnnmyqy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gjqowjbre.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtslanxtd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpfkvazvp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghermqcir.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggzazvabw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gokwcamea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gulpoopfv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaienvvms.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdbltagbg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gnxmpcieo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gngvtbbem.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gwbxqbppg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdkxaezgh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwwystpfm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gqbuosnfs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gljgxnlqu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gomthxnxj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gbgdjsegx.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/godljkhvs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gjhztnofl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gvebeowxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/guasrhapv.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/ggmmhjder.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gqqpyaxwm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gvnlpugzw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gdicatjhx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gpfruygne.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkgcfaqbw.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gwrhzvgma.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvpvqhrvn.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gatxsekol.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gofhpfaba.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gkfjaymul.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gmhrgwpuf.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gnfrbqfhz.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gmyigqlmw.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gqvekdpxu.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gktadyiwo.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gswpqdkfd.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gchfnirfs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gkuleswbz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ganlpsetv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ggndqdgpx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gwsmfjxte.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gozvszovm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gurteznbj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/ggozujqta.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gkrmfhxoj.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gxnwbvkdq.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/giazkwknz.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/ggeffaxms.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gsvqkmotv.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/glsfrpbor.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gmhsttzua.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gqombtsfx.sHtML


<!-- 参考信息 -->