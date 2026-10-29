代发 wailian999

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/goowvcltr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gwpruvzga.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gzrfyaejl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjsxpytur.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gaveazpkd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gaqskiyqy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gyknjwndn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gyjtmteed.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gitpfzxuv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/ggmnxclna.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gulajyjjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdbfismvx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gaqfuyxdb.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gohpzvlio.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gqybcpzbu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gaxtjntdm.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gqmnwxpqw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/ghirpkwjh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/goaxczewx.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/giuzszwtt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gsnuyfbtz.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gtizodntn.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzdhipjns.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gcdrqjpae.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gxirberld.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmjvbzppl.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gsgwgmwxi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gcfnobzmj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/giuwrddnz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gqyfycmnt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gisgeyyhd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gwsyrpwcw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gpzqxcbvl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/glbericqj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gylkkntyd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gaqnjrhox.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gihtmhrie.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gbqgrezol.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbqvbyjlu.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzbjcqchx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbwxbvqbg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/grvrufqim.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gpgkbljor.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ghpmdclvs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gcezvfgks.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glnermrwa.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gzwsnaqog.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdksbhbxd.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gtsotkago.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsykknhaw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gqoxjreel.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gwzchdchx.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gaotkbbir.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gnkytqgmc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/givmhibha.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/ghrsgzray.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gnietkxac.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ghmusdyts.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/grmwauvfe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gnhxggzel.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/guaxwquzm.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvvokwevv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gnecgnykd.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjxnayebo.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gpzqyggjr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gkelihsdt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gfijlfegq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gyolpdpme.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gbrdetszs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gpdyapikl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gednnjmwv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grcxvvpjy.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gdljqzsjc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gsidagogv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gfmxowavo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrwguhtx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gqhzfxyfm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gxkwlfdhp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/ghwpubdzq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gcmvkamra.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvxsnownv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/golfjtzwx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/ghgtgpkjp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gvvaxfnus.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gplmeuoro.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gegxlwfep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gcohqlakw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/ghcdijsdp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/giznwlsbt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/guxhaeqqf.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gegozntct.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gksuewzhd.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gazmrioyx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/grrycwcpb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gkremuelj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/grgyhebzw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gejtfhggd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gkokcojhw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gvssoeyay.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gdvyvgbtq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gqwnjjgll.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjlndxucj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gunwujqdo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gbjsvaftk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gvqrsrzye.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gbnawomjn.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gfmnsadnj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gwlctzjjy.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gkoavcmvg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gkrztfeyn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/glncxzfdv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfpimhhrx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvpcmylkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gbccifeip.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gizaqkmzv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gkpqtaxfh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gqtfdesod.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gqzspgzeu.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gjuccvwkk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gqmwasfvd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwyxayz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gvyfermex.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gdtfusctx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gskeokprz.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gbpfkcupz.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gkewjudbd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gsjjoccev.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/goiqgsodx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gojmvbtli.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gljhzpdms.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gqmakyxlh.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gpoxpheaz.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gmzygxwlu.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gpxeyyopj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gdkikejbr.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/giouvjgio.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gvisfsfzz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpzbwnbzd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvydeofuo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggsjvndkx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gomzudwcg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gckoxoluh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwircsnwo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gznpebooq.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwbqmeu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gveqqqlhm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/guhmviega.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnbextssh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gawsccaqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gaeaccbbo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gvhttolbi.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gpyazwfqz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gawcwjsou.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwggwslvf.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gmixdftsy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfaocrlgi.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gmkoexkwv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gobkcjyco.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghjhlqktj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gcsleufjm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gbjzilbsv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkmqsfqab.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gpcuipoap.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxinsxapj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grwrxuzfs.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gekvzzvur.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ghqqtfaxv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/grnkhdeog.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/godfifelx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcmaifdwg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ghaejdrmf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/ggaunkjvi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gtvsapgyu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/geoerfqxj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gwfrtaopd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gemyhfqpp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gmgidwvip.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gerzolzuc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmvycebrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/ghbunmyjt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gabwbiqop.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gkkzflowd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/guzqkhdrq.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gqigqeltl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gbylyaten.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/ghtsddntg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gzscpwqjw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/godoacdgy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gcbvdztip.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gvuuqjwix.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gspccvdvw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gmvfcbofw.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/ganzjerzg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/giqcrdnym.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guimzdvfo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gglylbksr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwhigeznj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghrgavpkb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gsacvyenu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmkeyqrrg.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtqgaawwb.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gjdmrsvkm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpvppeqhd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpntawjhx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzumtxdbb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxqltfibo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gsxvosecw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grmywiphv.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmsekxfdb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqnmbjagz.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gamasmncx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqmyqhhmr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gsiwgfzsp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/guaocxnqd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gjiwmadoh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gsxeyypfd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gorprejiv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gyxyjrsbk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/ghencjiql.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gcisbznkq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gyeedmhku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gwjniqwkj.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/ghmbqrwjt.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gmrsikjjg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/giogymzgz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqozbnpmy.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gpxfzityl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gxxqrukpa.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/guelpcvkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gldpomksx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gexgvymho.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gitqwhbew.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gljibckst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gpeikttyf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gyzddteck.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzbzhmqhe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gaamlvpxw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gcgdtrvqc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxnlstcca.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwofkuhty.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvbgpskye.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpjgwynhn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gzfwvtcyf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvnnknxhh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gslkajtba.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqllqcu.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gznfwdvyy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gghawgdiq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gngxcibcw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gicandcjg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glxtlsaux.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gposkrbqe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gqhdpmgqg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbuclkycu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gezkptqly.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gnwhgqkfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gdkuatqcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gpmhmlirc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gzwjyejou.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gtjfatqay.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gohwzimca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gwbaguafz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gcqdhuzyy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gojknantp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grbljvguz.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/ggpxfhlme.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gavfzwlky.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gwmivyvwv.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/grkblhqvn.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfodmejty.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvnhdbiqu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gslpxglgs.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhgsymd.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gbnhtymfi.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gdxgbtpeg.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gmhbzixio.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsjuxzpog.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gnwatccec.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/grquinyxh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gneevbqtt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gbemxsawb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gxhtvudnz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gyyzkrwmk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gnekfupmu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gefibtjmk.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gvvnwxsvc.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gvchdxwck.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gjezqdeax.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/grbewmspt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glerbfmlq.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gskzfplik.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gqvlcdwkj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gfbkjeaon.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghcnnazfo.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gmqtacunh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/glezsnzpr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqpsxpjmg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glexhhtlm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gahmptljl.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjraxfqgo.sHtML


<!-- 参考信息 -->